# IP2Vec
implementing the concept of Word2Vec to represent relations between Ip addresses in a network traffic dataset

In this project, we applied the concept of Word2Vec to capture relationships between IP addresses within a network traffic dataset, a method we refer to as IP2Vec. By leveraging the Destination Address, Source Address, and Destination Port fields, we constructed pairs of target and context words as follows:

Target             Context 
Source Ip          Destination Ip, Destination port 
Destination port   Destination Ip

Furthermore, we also used the destination port as a target to ensure its representation within the embedding space.

We utilized a Skip-gram model to train on these pairs, extracting the learned weights to obtain representation vectors. This step allowed us to capture meaningful semantic relationships between IP addresses within the network traffic.

The primary objective of this mini-project was to augment another intrusion detection model. By integrating IP2Vec representations, we enhance the capability of the intrusion detection system to utilize the contextual information embedded within IP addresses, thus improving its overall effectiveness in detecting potential threats and anomalies within the network.

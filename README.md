# IP2Vec
implementing the concept of Word2Vec to represent relations between Ip addresses in a network traffic dataset


Explanation: 
We implemented the concept of Word2Vec to represent relations between Ip Adresses.
We used the Destination Address, Source Adress and destination port. 
The target and context words were as follow :

Target             Context 
Source Ip          Destination Ip, Destination port 
Destination port   Destination Ip

we used destination port as target too to have it's representation too. 

we then used a skipagram model to train and then take the weights to be the representation vector. 
This mini-project was done to assist another Intrusion detection model, after this IP2Vec step we are able to use the information in the Ip address to help train the other intrusion detection model. 

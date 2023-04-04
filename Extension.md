## Extension
### How can we add additional features to the protocol without breaking previous functionality?
* Send to any individual on the whole UW campus
  For this part, we can give each individual on UW campus a
  
  
  
  
* Specify whether contents are ASCII text, Unicode text, or binary values

  For this part, the solution that I can think of is to specify the content type when sending the message from the sender. So for the header of the Internet
  protocol (or the corners of the index cards), we can add another field called content type by explicitly specifying its content type. Since it is separate
  from the message, the recipient should be able to take a look at it before seeing the message. 
  
* Keep a record of what nodes the card has passed through

  For this part, we can add another field or section to the header at the beginning of frames or packets called 'passed-nodes'. So each time, if the sender/node
  deliver the packet to a new node, the packet will have a mechanism by appending a new node to the 'passed-nodes' field. Since we want to avoid duplication,
  we can check whether the node that is going to receive the packet has already be on the 'passed-nodes', if it is on there, then we should not pass the 
  packet to the node. 

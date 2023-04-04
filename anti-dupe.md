## Anti-Duplication
### How can we ensure that each card is received once and only once?
For each Intermediary Node, we can use a data structure to store all the cards that the node has received before. If a card is transferred to a node, then we want to check whether the node has received the node before (by looking at its internal data structure such like a set or hash map); if the node found the card has passed to itself before, then it will reject the card so the card can be passed to somewhere else. 

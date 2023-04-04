## Administration
### How can we send commands ("SLEEP", "RESTART", "ARE-YOU-THERE", etc) to individual nodes in the network, rather than treat them as pass-through intermediaries?
I think we can construct some kind of log systems so that each sender can search for relevant entries and analyze them to
determine if the message or event was received and processed successfully by the server. The log entries may contain information
about the status of the message or event, any errors that occurred, and other relevant details. Moreover, if we have recorded all
the intermediary nodes in the process of each protocol, we can send an acknowledgement back through the list so that the sender knows whether
the message got delivered.

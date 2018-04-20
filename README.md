# stop-and-wait
A simple implementation of stop and wait ARQ with timer
Stop and Wait protocol:
Sender:
• A function makeframes() generates 30 frames.
• Number of Frames to be generated is taken as input at Sender Terminal
• A timer is set for 1sec before a send operation 
• The sender sends a frame, wait for acknowledgement for 1sec
• If Ack is not reached, sender retransmits the frame 
• Once ack is received, sender sends the next frame.
• This continues for a fixed number of times as given in input

Receiver: 
• The receiver waits for the frame to be sent 
• Before sending ack, receiver is made to sleep for 5sec to check the retransmission process of sender. 
• Receiver sends the ack and waits for the sender to send a frame.
• Receiver exits when sender does.

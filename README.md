### Web-RTC-Notes

```
NAT - Network Address Translator
STUN - Session Traversal Utilities for NAT
     - Tell me my public ip/port through NAT
     - Free server
     - Doesnt work in Symmetric NAT
     - Work in Full-cone
     - Cheap to maintain
     - Default port 3478, 5349
     
     Example how it work: Computer 1 <--[assigned ip:port]--> STUN Server <--[assigned ip:port]--> Remote Computer 
                          Computer 1 <-- [send Files/Media etc] Remote Computer 1
                          
TURN - Traversal Using Relays around NAT
     - Expensive to maintain
     - Not free
     - Default port 3478, 5349
     - In case of Symmetric NAT we use TURN
     
    Example how it work: Computer 1 <--[assigned ip:port]--> TURN Server <--[assigned ip:port]--> Remote Computer 
                         Computer 1 <-- [send Files/Media etc] TURN Server <-- [send Files/Media etc] Remote Computer 1
         
ICE - Interactive Connectivity Establishment
SDP - Session Description Protocol
    - Format and Describes ICE candidates, networking, media options, security etc.
    - Not a protocol its a format
    - Generated by users and send it to other party
Signaling the SDP - SDP Signaling
                  - Send SDP that was generated to the other party we want to communicate
                  - Signaling can be done via tweet, QR, Web Socket, HTTP Request (doesn't matter just send that large string to other party).
```

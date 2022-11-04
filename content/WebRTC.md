# WebRTC

## Projects

- **Feathers** https://github.com/feathersjs/feathers
    "A framework for real-time applications and REST APIs with JavaScript and TypeScript"
    * [ ] KAITO: What does it do exactly?


## Architecture

TLDR:
- TURN is a relay server


- ICE
https://en.wikipedia.org/wiki/Interactive_Connectivity_Establishment

- STUN
https://en.wikipedia.org/wiki/STUN

- TURN
https://en.wikipedia.org/wiki/Traversal_Using_Relays_around_NAT


## Learning

- [ ] STUDY: https://github.com/tking/JSTUN

- [What are STUN and TURN Servers? (WebRTC Tips from WebRTC.ventures) | YouTube](https://www.youtube.com/watch?v=4dLJmZOcWFc)
    * Opinion: ok


- [STUN/TURN Servers and Private Networks (WebRTC Tips by WebRTC.ventures) | YouTube](https://www.youtube.com/watch?v=N5cqu0kTIsw)
    * Opinion: ok


### NOTES: Servers for WebRTC: It is not all Peer to Peer
Speaker: Chad Hart
Conf: Kranky Geek WebRTC Brazil 2016
Channel: Google Chrome Developers
Link: https://www.youtube.com/watch?v=Y1mx7cx6ckI

_Key Topics: Signaling considerations, ICE, STUN, TURN details, media servers, gateways_

- Call flow diagram
https://youtu.be/Y1mx7cx6ckI?t=104

- SDP = Session Description Protocol
Signaling is transfering SDP (params) between browers.

- There are two types of ICE candidates: `host` (local address), STUN (reflexic), and TURN (relay).

- To solve the "mesh problem", we can use these approaches:
    * Multipoint Control Unit (MCU) https://youtu.be/Y1mx7cx6ckI?t=1806
    * Selective Forwarding Unit (SFU) https://youtu.be/Y1mx7cx6ckI?t=1919
    * SFU with Multicast https://youtu.be/Y1mx7cx6ckI?t=2014
    You send two streams full resolution and a low bitrate stream (thumbnail), since usecases  (as in Discord or Skype) usually there is 1 active talker (the presenter or streamer) and other participants, whom we don't want to watch in full HD.
    This is the state of the art (at least in 2016).

- How to get/use a media server (not categorized by their approaches):
    - Open source:
        * Licode https://github.com/lynckia/licode
        * ...

### NOTES: How to Build an End-to-End WebRTC Service (Kranky Geek WebRTC Brazil 2016)
by Daniel
https://www.youtube.com/watch?v=nPnWIuAlphc
opinion: ok

Talks about:
- Mainly WebRTC Signaling
- Quality of Service (at least once, exactly once, etc.)
- DNS-based system sharding


---

END.

## Encoding Formats
RTMP - Real Time Messaging Protocol
* Dependent on flash plugin. Being phased out *Need to verify*
* Uses Push Model
* Maintains a persistent TCP connection between the client(player) and the server
* Broadcast is split into audio and video streams of 4KB chunks and multiplexed in TCP connection 
* Used in *Live for Facebook Mentions*'s client

MSS - Microsoft Smooth Streaming
    Microsoft's Streaming for xBox mostly for Windows specific apps

HDS - HTTP Dynamic Streaming
    Sucessor of RTMP based on flash. Has adaptive streaming support

HLS - HTTP Live Streaming
    Introduced by apple supported by Android, Desktop and iOS devices. Widely used currently. Supports adaptive streaming
    Pull model

MPEG-DASH
    New kid in the block. Only internationalised solution. Supports adaptive streaming. Codec agnostic; Supports EME and MSE (standards-based API for browser based digital rights management [DRM])

## Streaming Mechanisms

### Live Streaming 
*Examples* Live cricket/soccer matches
*Problems* Thundering Herd
*Potential Solutions*
    * Network of edge distributed caches
    * A proxy in the edge handling the incoming request that transfers to the cache
    * *Request coalescing*, the edge cache upon receiving cache miss requests, lets one request to pass through to the next layer of cache and queues up the rest of the them




Business Models:
    1) Ad based model - Video content is free and ad are used generate revenue. Effective with large user base e.g. YouTube
    2) Pay Per View - Each content is given a price and revenue is based on the content user streams. e.g. iTunes
    3) Subscription Based - Timely fee is applied on a range of content. e.g. Netflix, Amazon Prime


https://bitmovin.com/mpeg-dash-vs-apple-hls-vs-microsoft-smooth-streaming-vs-adobe-hds/


DRM - Digital Rights Management


http://highscalability.com/blog/2016/6/27/how-facebook-live-streams-to-800000-simultaneous-viewers.html

https://engineering.fb.com/ios/under-the-hood-broadcasting-live-video-to-millions/
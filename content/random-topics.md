# Random topics


## Bookmarks

#akaito/pins #insp
- https://github.com/duthaho/bookmark
    * Class-based React.
    * Meh ui design and meh code.

- Shiori https://github.com/go-shiori/shiori
    * "Simple bookmark manager built with Go"
    * Shiori means "bookmark" in Japanese. (https://jisho.org/search/shiori)
    * Features:
        + Local webserver
        + Chrome extension
        + Web UI
        + CLI
        + Can download and update full webpages (think: MHTML)
    * [ ] Why doesn't it use MHTML?


## Heroku alternatives

- [ ] https://www.reddit.com/r/Heroku/comments/wxn5b5/following_herokus_decision_to_remove_free_plans/

- [x] [Heroku to end free tiers, creating platform void for devs](https://www.techtarget.com/searchsoftwarequality/news/252524336/Heroku-to-end-free-tiers-creating-platform-void-for-devs)
    * TLDR: they will cancel Heroku Free next month (Nov. 2022), and there is no good alternative to it.


## Virtual Input Devices
Virtual mic.

- [x] **VB-CABLE** Virtual Audio Device #closedsource
    https://vb-audio.com/Cable/
    * Used with the "Type to Voice Chat" app.

- [ ] **JACK** Audio Connection Kit #opensource
    https://jackaudio.org/

-  [ ] **Carla** #opensource
    https://kx.studio/Applications:Carla


## text-to-mic

- **Type to Voice Chat** https://github.com/rossbreytberg/type-to-voice-chat
    * A UWP app
    * Uses WinJS
    * Relies on `AudioGraph`
    * [AudioGraph Class (Windows.Media.Audio) - Windows UWP applications | Microsoft Learn](https://learn.microsoft.com/en-us/uwp/api/windows.media.audio.audiograph?view=winrt-22621)
    * [ ] [Audio graphs - UWP applications | Microsoft Learn](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/audio-graphs)
    * KAITO: It simply uses TTS to create an audio file and then pipes it to the output device (a virtual mic).
    * They suggest VB-Cable as a virtual microphone.


## Server push

- [ ] [Server-Sent Events explained with use cases | APIfriends](https://apifriends.com/api-streaming/server-sent-events/

- [ ] [Server-Sent Events (SSE) In JAX-RS | Baeldung](https://www.baeldung.com/java-ee-jax-rs-sse

- [ ] [Server-sent events - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events

- [ ] [Using server-sent events - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events

- [ ] [Stream Updates with Server-Sent Events - HTML5 Rocks](https://www.html5rocks.com/en/tutorials/eventsource/basics/

- [ ] [Introducing WebSockets: Bringing Sockets to the Web - HTML5 Rocks](https://www.html5rocks.com/en/tutorials/websockets/basics/

- [ ] [Long Polling vs WebSockets vs Server-Sent Events | by Vivek Kumar Singh | System Design Blog | Medium](https://medium.com/system-design-blog/long-polling-vs-websockets-vs-server-sent-events-c43ba96df7c1


## Handling missed events

- [message queue - How can an event subscriber catch up with missed events? - Software Engineering Stack Exchange](https://softwareengineering.stackexchange.com/questions/393921/how-can-an-event-subscriber-catch-up-with-missed-events)
    * [x] [Ben's answer](https://softwareengineering.stackexchange.com/a/393926)

- [ ] [c# - How to recover from missed integration or notification events in event driven architecture? - Stack Overflow](https://stackoverflow.com/questions/65425071/how-to-recover-from-missed-integration-or-notification-events-in-event-driven-ar)

- [ ] [Push events](https://web.dev/push-notifications-handling-messages/)


## Reverse proxy

- [x] Caddy https://caddyserver.com
    * It still auto redirects to https

- [ ] CoreDNS https://coredns.io
    * As suggested by this reddit comment https://www.reddit.com/r/selfhosted/comments/jpdl7a/comment/gbe5obu/?utm_source=share&utm_medium=web2x&context=3


## Zero config bundlers/servers
#javascript #nodejs
Zero config node bundlers/servers

- Parcel https://github.com/parcel-bundler/parcel

- Zero Server https://zeroserver.io/


## OpenSearch
`.osdx`

- Spec https://github.com/dewitt/opensearch

- [Creating an OpenSearch Description File in Windows Federated Search - Win32 apps | Microsoft Learn](https://learn.microsoft.com/en-us/windows/win32/search/-search-federated-search-osdx-file)

- [OpenSearch description format | MDN](https://developer.mozilla.org/en-US/docs/Web/OpenSearch)

HTML:
```html
<link rel="search" type="application/opensearchdescription+xml" href="opensearch.osdx" title="Kaito">
```

## Markdown parsers

### Java

- **flexmark-java** https://github.com/vsch/flexmark-java
    >
    > **flexmark-java** is a Java implementation of CommonMark (spec 0.28) parser using the blocks first, inlines after Markdown parsing architecture.
    >
    > Its strengths are speed, flexibility, Markdown source element based AST with details of the source position down to individual characters of lexemes that make up the element and extensibility.
    >
    > The API allows granular control of the parsing process and is optimized for parsing with a large number of installed extensions. The parser and extensions come with plenty of options for parser behavior and HTML rendering variations. The end goal is to have the parser and renderer be able to mimic other parsers with great degree of accuracy. This is now partially complete with the implementation of Markdown Processor Emulation

    * Supports Wikilinks with a possible custom link resolver
    
    * [ ] TRY

- **commonmark-java** https://github.com/commonmark/commonmark-java
    * [ ] TRY


## Petri Net Viz
#softviz

- https://github.com/kyouko-taiga/petri-js
    * Uses D3

- http://petrinet.org
    * Uses ???

---

END.

# Random topics


# Design systems

Interesting, web design:
- [Search – Carbon Design System](https://www.carbondesignsystem.com/patterns/search-pattern/)

- Material UI


# React

- https://github.com/enaqx/awesome-react
- https://github.com/brillout/awesome-react-components

### Getting Closure on React Hooks by Shawn Wang | JSConf.Asia 2019
#JSConf #React
* https://www.youtube.com/watch?v=KJP1E-Y-xyo
* opinion:liked

```
The design of React Hooks requires a good understanding of closures in JavaScript. In this talk, we’ll reintroduce closures by building a tiny clone of React! This will serve two purposes – to demonstrate the effective use of closures, and to show how you can build a Hooks clone in just 29 lines of readable JS. Finally, we arrive at how you get Custom Hooks and the Rules of Hooks out of this incredible mental model!

Originally from Singapore, swyx is an Infinite Builder working on Developer Experience at Netlify. In his free time he helps people Learn in Public at Egghead.io and /r/reactjs.


JSConf.Asia - LASALLE College of the Arts, Singapore - 15 June 2019
```

This is not React. What is React? This is my answer:
- [Shawn Swyx Wang - Why React is not Reactive | YouTube](https://www.youtube.com/watch?v=nyFHR0dDZo0)

### Shawn Swyx Wang - Why React is not Reactive | React Rally 2018
* https://www.youtube.com/watch?v=nyFHR0dDZo0
* opinion: ok
* Mentions [`window.requestIdleCallback()` | MDN]https://developer.mozilla.org/en-US/docs/Web/API/Window/requestIdleCallback  


# Parsers

## Markdown parsers

### JavaScript

- https://github.com/markedjs/marked
    * Demo (AST explorer) https://marked.js.org/demo/

    * Used by:
        + DanganFont?

- remark https://github.com/remarkjs/remark
    * AST Exploter: Remark
    https://astexplorer.net/#/gist/0a92bbf654aca4fdfb3f139254cf0bad/ffe102014c188434c027e43661dbe6ec30042ee2

    * Used by:
        + muninn
        https://github.com/szymonkaliski/muninn/blob/master/packages/muninn-lib/src/markdown/index.js

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


## Parser combinators
[Parser combinator | Wikipedia](https://en.wikipedia.org/wiki/Parser_combinator)

- Masala Parser https://github.com/masala/masala-parser
"Masala Parser is inspired by the paper titled: Direct Style Monadic Parser Combinators For The Real World. \
Masala Parser is a Javascript implementation of the Haskell Parsec. It is plain Javascript that works in the browser, is tested with more than 450 unit tests, covering 100% of code lines."


- Arcsecond https://github.com/francisrstokes/arcsecond
"Arcsecond is a zero-dependency, Fantasy Land compliant JavaScript Parser Combinator library largely inspired by Haskell's Parsec."

- https://github.com/microsoft/ts-parsec
"ts-parsec is a parser combinator library prepared for typescript. By using this library, you are able to create parsers very quickly using just a few lines of code. It provides the following features:"


# Search input
Trying to make a Discord-like search input

#interesting #useful
- [ ] https://github.com/zurb/tribute
"ES6 Native @mentions"
Supports multiple collections and different trigger prefixes.

- [ ] https://github.com/signavio/react-mentions

- Tags with misc text:
https://github.com/yairEO/tagify


#design #insp
- Clew: Universal search by Udara Jay on Dribbble
https://dribbble.com/shots/17063596-Clew-Universal-search


# Search engines

- [ ] Lunr https://lunrjs.com
    * "Lunr: A bit like Solr, but much smaller and not as bright"
    * https://github.com/olivernn/lunr.js

#javascript #clientside #searchengine
- [ ] Fuse.js https://fusejs.io
    * "Fuse.js is a powerful, lightweight fuzzy-search library, with zero dependencies."

    * [ ] [Using Fuse.js to add dynamic search to a React app | LogRocket  Blog](https://blog.logrocket.com/fuse-js-dynamic-search-react-app/)
    By Danny Guo, April 5, 2021
    
    * Used by
        https://github.com/tagspaces/tagspaces


## Web frameworks: Blogging

- Eleventy
    - https://github.com/11ty/eleventy-base-blog
    - https://rphunt.github.io/eleventy-walkthrough/template-files.html


## JavaScript: Bundlers

#bundler #javascript
- [x] Browserify
    `npm:browserify`
    https://github.com/browserify/browserify
    https://browserify.org/


- [x] UglifyJS "JavaScript parser / mangler / compressor / beautifier toolkit"
    `npm:uglify-js`
    https://github.com/mishoo/UglifyJS
    https://lisperator.net/uglifyjs/


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


## Petri Net Viz
#softviz

- https://github.com/kyouko-taiga/petri-js
    * Uses D3

- http://petrinet.org
    * Uses ???

---

END.

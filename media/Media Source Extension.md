# Media Source Extension (MSE)

>provides functionality enabling plugin-free web-based streaming media

With Media Source Extensions (MSE), this is changing. <br/>
MSE allows us to replace the usual single progressive src URI fed to media elements with a reference to a MediaSource object, <br/>
which is a container for information like the ready state of the media for being played, <br/>
and references to multiple SourceBuffer objects that represent the different chunks of media that make up the entire stream. <br/>

MSE gives us finer-grained control over how much and how often content is fetched, and some control over memory usage details, such as when buffers are evicted. <br/>
It lays the groundwork for adaptive bitrate streaming clients (such as those using DASH or HLS) to be built on its extensible API.<br/>

<br/>

### [StackOverFlow : Comparing Media Source Extensions (MSE) with WebRTC](https://stackoverflow.com/questions/36416344/comparing-media-source-extensions-mse-with-webrtc) 

>Media Source Extensions is just a **player inside the browser.** <br/>
>You create a MediaSource object https://developer.mozilla.org/en-US/docs/Web/API/MediaSource and assign it to your video element like this <br/><pre><code>video.src = URL.createObjectURL(mediaSource); </code></pre>
>Then your javascript code can fetch media segments from somewhere (your server or webserver) and supply to SourceBuffer attached to MediaSource, for playback.

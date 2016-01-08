# HxAudio.js


__hxaudio.js is a drop-in javascript library that allows HTML5’s `<audio>` tag to look the same in any browser.__


Native AudioElement Google Chrome  
![Audio Google Chrome](bin/img/audio_chrome.png)

Native AudioElement Firefox  
![Audio Firefox](bin/img/audio_firefox.png)

Native AudioElement Safari  
![Audio Safari](bin/img/audio_safari.png)


It uses native `<audio>`. It provides a consistent html player UI to all browsers which can be styled used standard css.

Native AudioElement styled by HxAudio.js  
![Audio Safari](bin/img/audio_hxaudiojs.png)



## Inspired by audio.js

I was inspired by the works of Anthony Kolber: [audio.js](http://kolber.github.io/audiojs/).  
But after a closer look it could use an update:

- no need for flash anymore ([support of audio element](http://caniuse.com/#feat=audio))
- using flat design (make css simpler)
- no need for a initialize script (wait for DOM and just do it)
- use [Haxe](http://www.haxe.org) (Haxe is awesome! One codebase, many targets, no platform specific code.)
- it hasn't been touched in 2 years


###Installation


1. Put `hxaudio.js` and `hxaudio.gif` in the same folder.

```
/hxaudiojs
	/hxadio.js
	/hxaudio.gif
```
3. Include the audio.js file:

```
<script src="/hxaudiojs/hxaudio.js"></script>
```

2. Then you can use `<audio>` wherever you like in your HTML:

```
<audio src="/mp3/juicy.mp3" preload="auto" />
```


###Examples
A series of API tests & examples for using and extending audio.js

- Example: [Multiple players, testing preload, loop & autoplay attributes](http://matthijskamstra.github.io/hxaudiojs/example01.html)


###Browser & format support

It has been verified to work across:

- Safari
- Chrome
- Firefox

###Source code
All efforts have been made to keep the source as clean and readable as possible. Until we release more detailed documentation, the annotated source is the best reference for usage.

[Annotated source](https://github.com/MatthijsKamstra/hxaudiojs/blob/master/src/Main.hx) / [Source](http://matthijskamstra.github.io/hxaudiojs/) on Github

###License
hxaudio.js is released under an [MIT License](https://github.com/MatthijsKamstra/hxaudiojs/blob/master/LICENSE), so do with it what you will.


###Build from source

Use NPM watch for automate build   
`cd ` to the correct folder 

```
npm install
npm run watch
```

or just build it once with

```
haxe javascript.hxml
```

And open `/bin/index.html` in your favorite browser. 





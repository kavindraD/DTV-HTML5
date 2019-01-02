# DTV-HTML5 EventHandler-FlashFallback

Event Handlers HTML5 video player powerd by **DevTrip Video** developers and its' contributers

## Goal

This JS class provide a reusable video player component, which can easily integrated with any HTML based site. It generates/provide default HTML 5 video player with UI implemented with the DOM of user browser.

## Configuration 

It has nominal basic configuration to integrate it with HTML 5 browsers. 

```JS
	var params = {},_devtripVideo = new devtripVideo();
	params.containerId = "playercontainer1";
	params.width = "320";
	params.height = "240";
	params.video = "abc";
	params.autoplay = false;
	params.videoImage = "abc.png";
	function playingHandler(){
		//alert('here');
	};
	_devtripVideo.cllback_playingHandler(playingHandler);
	_devtripVideo.init(params);
```

A detailed use case is available with HTML page (devtripVideo.html) available with release package.

With Event Handlers devtrip video component following methods are available,these parameters are mandatory except [Event Handler Customisation](#event-handler-customisation) which is optional -

1. [Instantiate](#instantiate)
2. [Associate Param](#associate-param)
3. [Set Asset Path](#set-asset-path)
4. [Dispose Internal Listener](#dispose-internal-listener)
5. [Event Handler Customisation](#event-handler-customisation)


#### Instantiate

devtripVideo player component need to be instantiated as follows - 

> `var _devtripVideo = new devtripVideo();`

#### Associate Param

To associate player with a container use 

> `params.containerId = "playercontainer1";`

To set width of the player use

> `params.width = "320";`

To set height of the player use

> `params.height = "240";`

To disable auto play use

> `params.autoplay = false;`

Player will auto detect the extension required for a browser so it is recommended to have [.mp4,.webm, .ogg] format of video file with server.

> `params.video = "abc";`

> .mp4,.webm, .ogg format should be available at asset path.

Poster image can be provided using 

> `params.videoImage = "abc.png";`

> Image should be available at asset path.

call init(param) to initialise player and its object and their associated listeners.

> `_devtripVideo.init(params);`

#### Set Asset Path

To set assets path use 

> `_devtripVideo.setPath("assets/");`

> default path is "".

#### Dispose Internal Listener

call dispose() to remove internal listener of player.

> `_devtripVideo.dispose();`

#### Event Handler Customisation

Below are the events available with this video player component which can be customise as fallows -

**These customisation is optional not maindatory**

Event **error** event handler can be customised as -

> ```JS
>	function errorHandler(){
>	  //do custom code need to execute on "error" event handler.
>  };
>  _devtripVideo.cllback_errorHandler(errorHandler);
```
```JS
```
		
Event **loadedmetadata** event handler can be customised as -

>```JS
>	function loadedmetadataHandler(){
>		//do custom code need to execute on 'loadedmetadata' event handler.
>	};
>	_devtripVideo.cllback_loadedmetadataHandler(loadedmetadataHandler);
```
```JS
```
		
Event **timeupdate** event handler can be customised as -

>```JS
>	function timeupdateHandler(){
>		//do custom code need to execute on 'timeupdate' event handler.
>	};
>	_devtripVideo.cllback_timeupdateHandler(timeupdateHandler);
```
```JS
```
		
Event **pause** event handler can be customised as -

>```JS
>	function pauseHandler(){
>		//do custom code need to execute on 'pause' event handler.
>	};
>	_devtripVideo.cllback_pauseHandler(pauseHandler);
```
		
Event **playing** event handler can be customised as -

>```JS
>	function playingHandler(){
>		//do custom code need to execute on 'playing' event handler.
>	};
>	_devtripVideo.cllback_playingHandler(playingHandler);
```
```JS
```

Event **volumechange** event handler can be customised as -

>```JS
>	function volumechangeHandler(){
>		//do custom code need to execute on 'volumechange' event handler.
>	};
>	_devtripVideo.cllback_volumechangeHandler(volumechangeHandler);
```
```JS
```
		
Event **loadstart** event handler can be customised as -

>```JS
>	function loadstartHandler(){
>		//do custom code need to execute on 'loadstart' event handler.
>	};
>	_devtripVideo.cllback_loadstartHandler(loadstartHandler);
```
```JS
```
		
Event **loadeddata** event handler can be customised as -

>```JS
>	function loadeddataHandler(){
>		//do custom code need to execute on 'loadeddata' event handler.
>	};
>	_devtripVideo.cllback_loadeddataHandler(loadeddataHandler);
```
```JS
```
		
Event **ended** event handler can be customised as -

>```JS
>	function endedHandler(){
>		//do custom code need to execute on 'ended' event handler.
>	};
>	_devtripVideo.cllback_endedHandler(endedHandler);
```
```JS
```
		
Event **emptied** event handler can be customised as -

>```JS
>	function emptiedHandler(){
>		//do custom code need to execute on 'emptied' event handler.
>	};
>	_devtripVideo.cllback_emptiedHandler(emptiedHandler);
```
```JS
```
		
Event **stalled** event handler can be customised as -

>```JS
>	function stalledHandler(){
>		//do custom code need to execute on 'stalled' event handler.
>	};
>	_devtripVideo.cllback_stalledHandler(stalledHandler);
```
```JS
```
		
Event **waiting** event handler can be customised as -

>```JS
>	function waitingHandler(){
>		//do custom code need to execute on 'waiting' event handler.
>	};
>	_devtripVideo.cllback_waitingHandler(waitingHandler);
```
```JS
```
		
Event **progress** event handler can be customised as -

>```JS
>	function progressHandler(){
>		//do custom code need to execute on 'progress' event handler.
>	};
>	_devtripVideo.cllback_progressHandler(progressHandler);
```
```JS
```
		
Event **durationchange** event handler can be customised as -

>```JS
>	function durationchangeHandler(){
>		//do custom code need to execute on 'durationchange' event handler.
>	};
>	_devtripVideo.cllback_durationchangeHandler(durationchangeHandler);
```
```JS
```
		
Event **canplaythrough** event handler can be customised as -

>```JS
>	function canplaythroughHandler(){
>		//do custom code need to execute on 'canplaythrough' event handler.
>	};
>	_devtripVideo.cllback_canplaythroughHandler(canplaythroughHandler);
```
```JS
```


# DTV-HTML5 Simple

> Simple HTML5 video player powerd by **DevTrip Video** developers and contributers

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
	_devtripVideo.setPath("assets/");
	_devtripVideo.init(params);
```

A detailed use case is available with HTML page (devtripVideo.html) available with release package.

With normal devtrip video component following methods are available,these parameters are mandatory not optional -

1. [Instantiate](#instantiate)
2. [Associate Param](#associate-param)
3. [Set Asset Path](#set-asset-path)
4. [Dispose Internal Listener](#dispose-internal-listener)


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




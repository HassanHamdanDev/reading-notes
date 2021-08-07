# Audio, Video, Images


##  Images

```

- You can specify the dimensions of images using CSS. 
- This is very helpful when you use the same sized 
images on several pages of your site.
- Images can be aligned both horizontally and vertically 
using CSS.
- You can use a background image behind the box 
created by any element on a page. 
- Background images can appear just once or be 
repeated across the background of the box.
- You can create image rollover effects by moving the 
background position of an image.
- To reduce the number of images your browser has to 
load, you can create image sprites.


```



## Practical Information 

```

- Search engine optimization helps visitors find your 
sites when using search engines.
- Analytics tools such as Google Analytics allow you to 
see how many people visit your site, how they find it, 
and what they do when they get there.
- To put your site on the web, you will need to obtain a 
domain name and web hosting.
- FTP programs allow you to transfer files from your 
local computer to your web server.
- Many companies provide platforms for blogging, email 
newsletters, e-commerce and other popular website 
tools (to save you writing them from scratch).

```


##  Video and Audio APIs 


```
This creates a video player inside the browser like so

This is not as immediately useful for video playback, but it does have advantages. You can solve both these problems by hiding the native controls , and programming your own with HTML, CSS, and JavaScript.

The HTMLMediaElement API

Play, HTMLMediaElement. Pause, etc. This interface is available to both and elements, as the features you'll want to implement are nearly identical.

Exploring the HTML

The whole player is wrapped in a element, so it can all be styled as one unit if needed.

The controls HTML is probably the most interesting

Each has a class name, a data-icon attribute for defining what icon should be shown on each button , and an aria-label attribute to provide an understandable description of each button, since we're not providing a human-readable label inside the tags. The contents of aria-label attributes are read out by screenreaders when their users focus on the elements that contain them. There is also a timer , which will report the elapsed time when the video is playing.

This is so that, if the JavaScript doesn't load for some reason, users can still use the video with the native controls. We give the controls an opacity of 0.5 by default, so that they are less distracting when you are trying to watch the video. Only when you are hovering/focusing over the player do the controls appear at full opacity.

First of all, at the top of the CSS we use a @font-face block to import a custom web font.

Next we use generated content to display an icon on each button

We use the content property to set the content to be displayed in each case to be equal to the contents of the data-icon attribute. In the case of our play button, data-icon contains a capital «P». We apply the custom web font to our buttons using font-family. In this font, «P» is actually a «play» icon, so therefore the play button has a «play» icon displayed on it.

As the video plays, the width will be increased via JavaScript as the video elapses. The is also absolutely positioned to sit near the left hand side of the timer bar. We also give our inner and the right amount of z-index so that the timer will be displayed on top, and the inner below that.

Implementing the JavaScript

Create a new JavaScript file in the same directory level as your index. Html file. Call it custom-player. Const controls = document.

Const play = document. Const stop = document. Const rwd = document. Const fwd = document.

Const timerWrapper = document. Const timer = document. Const timerBar = document. The play/pause, stop, rewind, and fast forward buttons.

The outer timer wrapper , the digital timer readout , and the inner that gets wider as the time elapses.

Here we use an if statement to check whether the video is paused. Paused property returns true if the media is paused, which is any time the video is not playing, including when it is set at 0 duration after it first loads.

Let's step through mediaBackward the functionality for mediaForward

If active has been set on the rwd button, we remove it using classList. Remove, clear the interval that has been set when the button was first pressed , and use HTMLMediaElement. Play to cancel the rewind and start the video playing normally. If it hasn't yet been set, we add the active class to the rwd button using classList.

Add, pause the video using HTMLMediaElement. Media.

Updating the elapsed time

To do this we'll run a function to update the time displays every time the timeupdate event is fired on the element. The frequency with which this event fires depends on your browser, CPU power, etc . Timer.

First of all, we work out the number of minutes and seconds in the HTMLMediaElement. TextContent value of the timer is set to the time value, so it displays in the UI. The length we should set the inner to is worked out by first working out the width of the outer , and then multiplying it by the HTMLMediaElement. CurrentTime divided by the total HTMLMediaElement.

Duration of the media. We set the width of the inner to equal the calculated bar length, plus «px», so it will be set to that number of pixels.

At this point, you could delete the equivalent lines from the windBackward and windForward functions, as that functionality has been implemented in the stopMedia function instead.

Here are some suggestions for ways you could enhance the existing example we've built up

Because elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an element too. As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect method, and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object.

```

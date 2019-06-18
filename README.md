# Media Styler - Customise your audio and video players!
## Description
A jquery plugin that provides customisation controls for standard audio and video html elements. Optionally ensures that audio and/or video do not play at the same time and (optionally) rewinds and stops other media when a different one starts playing (so you can't get lot's of audio playing at once and go crazy from the noise)!

## What it does
* Lets you customise the controls of video and audio elements using regular CSS.
* Comes with a defualt orange style that you can feel free to modify as much as you want
* Stops other audio / videos from playing when a different one is played - which prevents audio / video from playing at the same time 
* Allows you to decide to let audio / videos play at the same time if you don't like the default option
* Allows you to specify whether you want to rewind other audio or videos when a different one starts playing or just pause them
* Has a customisable restart button
* Has a customisable play button
* Has a customisable pause button
* Has a customisable seek time display
* Indicates loading as it retrieves the media to play
* Very light weight
* Depends on JQuery
* Is very unobtrusive 

## How to use it
The quickest way is to download the plugin and take a look at the demo pages.

If you're after more detail though you basically want to do the following:

1) Download this plugin and add the **mediastyler.js** to your project's scripts folder, and the **stylised.css** to your project's styles folder (or wherever you store these in your project)

2) Make sure you have referenced JQuery in the page you're going to use this. Generally that means putting the following in the same page as the video / audio elements you want to customise:

   **&lt;script src="https://code.jquery.com/jquery-3.4.1.min.js" integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo=" crossorigin="anonymous"&gt;&lt;/script&gt;**

3) Next, reference the awesome plugin. At this point you will want to make sure you're sitting down because it's about to get uber cool.

   **&lt;script src="whereverYouPutThisFile/mediastyler.js"&gt;&lt;/script&gt;**
  
   Keep in mind this needs to point to wherever you actually put the script when you added it to your project.

4) Now add the CSS too:

   **&lt;link href="whereverYouPutThisFile/stylised.css" rel="stylesheet" type="text/css"&gt;**

5) Use the following to define which elements you want to stylise using the plugin. Generally that's going to be something like:

   **&lt;script type="text/javascript"&gt; $(function () { $('audio, video').stylise(); }); &lt;/script&gt;**

Keep in mind these are normal CSS selectors, so if you wanted to only stylise one single element, you could change 'audio, video' above to '#someElementsId' or '.justTheseElements' and as long as they are also either VIDEO or AUDIO elements, they will be the only things that get stylised.

6) Run it! 

7) Follow me on twtter: https://twitter.com/themuradonian and say thanks :p

## Advanced options
There are also three options you can initialise the plugin with:

 1) single-reset - to have a single active player which _resets_ others when played (the default option)
 2) single-pause - to have a single active player which _pauses_ others when played, or
 3) multi - to allow _all_ players to be active simultaneously
 
 To choose one, use the following code in place of the code I provided in step 5, and change 'single-reset' below to the one you want instead:
 
 **&lt;script type="text/javascript"&gt;
    $(function () {
      $('audio, video').stylise({mode:'single-reset'});
    });
 &lt;/script&gt;**
 
Let me know if you find any of this useful!

Nathan Murados 

# mediastyler
<h2>Description</h2>
A jquery plugin that provides customisation controls for standard audio and video html elements. Optionally ensures that audio and video do not play at the same time and (optionally) rewinds and stops other media when a different one starts playing

<h2>What it does</h2>

<h2>How to use it</h2>
The quickest way is to download the plugin and take a look at the demo pages.

If you're after more detail though you basically want to do the following:

1) Download this plugin and add the mediastyler.js to your project's scripts folder, and the stylised.css to your project's styles folder (or wherever you store these thigns in your project)

2) Make sure you have referenced JQuery in the page you're going to use this. Generally that means putting the following in the same page as the video / audio elements you want to customise:

&lt;script
  src="https://code.jquery.com/jquery-3.4.1.min.js"
  integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo="
  crossorigin="anonymous"&gt;&lt;/script&gt;

3) Next, reference the awesome plugin. At this point you will want to make sure you're sitting down because it's about to get very awesome.

  &lt;script src="whereverYouPutThisFile/mediastyler.js"&gt;&lt;/script&gt;
  
  Keep in mind this needs to point to wherever you actually put the script when you added it to your project.

4) Now add the CSS too:

  &lt;link href="css/stylised.css" rel="stylesheet" type="text/css"&gt;

5) Use the following to define which elements you want to stylise using the plugin. Generally that's going to be something like:

 &lt;script type="text/javascript"&gt;
    $(function () {
      $('audio, video').stylise();
    });
 &lt;/script&gt;

Keep in mind these are normal CSS selectors, so if you wanted to only stylise one single element, you could change 'audio, video' above to '#someElementsId' or '.justTheseElements' and as long as they are also either VIDEO or AUDIO elements, they will be the only things that change.

6) Run it! 


<h2>Advance options</h2>


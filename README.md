# Wave.js
audio visualizer library for javascript


<h1>Installation</h1>

<h3>Install With CDN</h3> 
https://cdn.jsdelivr.net/gh/PiethonCoder/wave.js/wave.js

<h3>Or</h3>
download the wave.js file from the root of this repository.

<h1>Setup</h1>
<p>create a new wave object.</p>

<code>
   var wave = new Wave();
</code>


<h1>Usage</h1>

<p>call one of the three main function on the wave object, fromFile, fromStream, fromElement.</p>

<code>
<pre>
var audio = document.getElementById("audio");
wave.fromElement(audio,"canvas_id",{wave:true});
</pre>
</code>


<h3>Documentation</h3>

<h3>Functions</h3>

<ul>
   <li>fromFile(file name,options)</li>  
   <ul>
<!--       <li>file name can be a string of a local or external file, or a data url object.<li>
      <li>options is a object of the options you want rendered.</li> -->
   </ul>
   <br>
   <li>fromElement(element,canvas id,options)</li>
   <ul>
      <li>element is a audio element object, or the id of a audio element as a string.</li>
      <li>canvas id is the id of the canvas you want to use as output. This is where the visualization will appear.</li>
      <li>options is a object of the options you want rendered.</li>
   </ul>
   <br>
   <li>fromStream(stream,canvas id,options)</li>
   <ul>
      <li>stream is a stream object, usually gotten from the getUserMedia() api.</li>
      <li>canvas id is the id of the canvas you want to use as output. This is where the visualization will appear.</li>
      <li>options is a object of the options you want rendered.</li>
   </ul>
   <br>
   <li>stopStream()</li>
   <ul>
      <li>pauses the current visual from the fromStream function.</li>
   </ul>
   <br>
   <li>playStream()</li>
   <ul>
      <li>plays the current stream visual.</li>
   </ul>
</ul>


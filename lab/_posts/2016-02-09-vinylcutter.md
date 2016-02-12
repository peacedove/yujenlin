---
layout: post
title: "Fab: Vinyl Cutter"
categories: lab/artdes217
cover_photo: /assets/img/lab/artdes217/vinylcut/taiwan.jpg
simple: simple
feature-img: "/assets/img/lab/artdes217/vinylcut/nerv.jpg"
---
<p>Feb 10, 2016:</p>
<h2 class="title">Not all Illustrator works</h2>
<p>To use the vinyl cutter our school has, Roland GX-400, we need to use the Illustrator plugin to connect MAC with the machine. Unfortunately, not all version of Illustrator works with that plugin. On my computer, I have tried CS5.1, CS6, CC2014, CC2015, only CS6 works (You can download the trial version on Adobe's website). To install the plugin on CS6, I need to download the Adobe Extension Manager CS6. Adobe discontinues their support of Extension Manager after CS6, so you will need to download an open source 3rd party extension manager to install extensions for newer Illustrator.<a href="https://github.com/nvkzNemo/UberManager">UberManager</a> is the one I used.
</p>
<div class="container">   
  <div class="tile width_two height_one image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/roland_gx.jpg')"> </div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/cs6.jpg')"></div>
  <div class="tile width_one height_one image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/ubermanager.png')"></div>
</div>

<h2 class="title">Illustrator Image Trace and Using Rhino to Remove Duplicate Edge</h2>
<p>Illustrator Image Trace and Using Rhino to Remove Duplicate Edge
Illustrator's Image Trace is a convenient tool to convert a rasterized image to vector graph. At the time I wrote this, I tried to do what I have done before, but sadly I cannot find the perfect parameters I was using at my first try. For the vector graph, we want it have outline only with no fill, and the line width is set to 0.25 pt. These lines are where the cutter is going to cut. The rectangle outside makes the vinyl sticker is easier to peel after the cutting. Since Illustrator's Image Trace usually create a lot of duplicate paths, which will make the cutter cut the same line twice. To avoid this, we import the .ai file to Rhino to remove the duplicate paths. In Rhino, we can use SelDup and SelOpenCrv to identify those duplicate edges. Delete those edges and export it back to Illustrator and we are good to cut it.</p>
<div class="container">   
  <div class="tile width_one height_one image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/dora_color.png')"> </div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/dora_traced.png')"></div>
  <div class="tile width_two height_one image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/dora_rhino.png')"></div>
</div>

<h2 class="title">Vinyl Cutting Sheet Transfer Paper</h2>
<p>The transfer paper can help you keep the sticker intact when you transfer it from the vinyl cutting sheet to the target surface. It is especially useful when your design contains separate fragment. So it won't make your sticker looks like the left one, which I paste every sticker separately by hand since it is the waste material. The right one is the final result.</p>

<div class="container">   
  <div class="tile width_two height_two image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/dora_black.jpg')"> </div>
  <div class="tile width_two height_two image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/dora_finish.jpg')"></div>
</div>

<p>Feb 11, 2016:</p>

<h2 class="title">Illustrator Tips: Text Envelope</h2>
<p>This is a experiment play around with combining text and shape together. I am from Taiwan, so I was thinking to combine the shape of the island and the country name together. The idea is deforming the text to the shape of the island. In Illustrator, there is a useful function called Envelope can help us to do that. First, I need a vector shape of the island, which I use image trace to get it again. And you will need the text. In my first try, I align the text to the orientation of the shape like this. Move the shape to the front, so it will cover the text. Select the two object and chose "Object>Envelope Distort>Make with Top Object", which will create the result like the leftmost picture, and it is not the result I want.</p>

<div class="container">   
  <div class="tile width_one height_one image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_map.png')"> </div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_first1.png')"></div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_first2.png')"></div>
  <div class="tile width_one height_one image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_first3.png')"></div>
</div>

<p>Let's try it again. This time, I rotate the shape to match the orientation of the text. It looks better, but not quiet what we want yet. I think the upper empty space is because lowercase letter is smaller, so I change it to all uppercase, and change the font. And it looks better. So we can expand it and make it to outlines only and cut it using the vinyl cutter.</p>

<div class="container">   
  <div class="tile width_one height_one image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_second1.png')"> </div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_second2.png')"></div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_second3.png')"></div>
  <div class="tile width_one height_one image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_second4.png')"></div>
  <div class="tile width_two height_two image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan_second5.png')"></div>
  <div class="tile width_two height_two image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/taiwan.jpg')"></div>
  </div>

<h2 class="title">Dual-Color Testing</h2>
<p>To experiment the dual-color sticker, I chose Godspeed You! Black Emperor's cover art. I was thinking to make the hand and the background be two different colors. I place the markers at three of the corners, so I can use those markers as references to line up the foreground and background parts later again. Since the background part contains a lot of small fragment, I test cut that part first. During the cutting, some part of the sticker is already peeled off. And since those segments are too small, it is very hard to separate them from the material besides them. It might be useful if I have some tools to separate them, but I don't have it at that time. So I decided to use a more simple design. It is a logo from a Japanese anime called EVA. I separate the maple leaf and the letter part to make them be a different color. Again, I have put markers on three of the corners. To combine the two colors together, I first cut the two part of the design on two different color vinyl sheet, then transfer one part on the transfer paper, and finally, transfer the second part on the same transfer paper and use the marker as matching point. Since the transfer paper is not transparent, so it is a little hard to match the rectangles. It might be easier if we use a clear transfer paper instead.</p>

<div class="container">   
  <div class="tile width_one height_one image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/lift1.jpg')"> </div>
  <div class="tile width_two height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/lift2.png')"></div>
  <div class="tile width_one height_one image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/lift3.jpg')"></div>
  <div class="tile width_one height_one image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/nerv1.png')"></div>
  <div class="tile width_two height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/nerv2.png')"></div>
  <div class="tile width_one height_one image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/nerv3.jpg')"></div>
  <div class="tile width_one height_one image alpha" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/nerv4.jpg')"></div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/nerv5.jpg')"></div>
  <div class="tile width_one height_one image" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/nerv6.jpg')"></div>
  <div class="tile width_one height_one image omega" style="background-image: url('/yujenlin/assets/img/lab/artdes217/vinylcut/nerv7.jpg')"></div>
</div>



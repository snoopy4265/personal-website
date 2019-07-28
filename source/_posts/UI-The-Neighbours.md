---
title: Rethink of digital intimacy with the Neighbours
date: 2019-05-24 12:34:44
categories: portfolio
tags:
  - portfolio
cover_image: /images/neighbours.JPG
---
<p style="color:#aaa;">Master Project | Year: 2018</p>

### Project Description
This work is an interactive project developed from two of New-Cybernetics core concepts: Feedback loop and Self-organisation. The visitor can stand in front of the computer and liberately choose a grid to shoot a GIF image. The captured GIF image will be projected on the corresponding grid point on the wall in real time. The only rule when shooting GIF image is, the visitor must do something related to its neighbour. The expectation is to see strangers who don’t know each other, or not even present at the same time, create virtual interactions through digital technology.

The appearance of this work was intentionally designed like windows of skyscraper. Questioning the meaning of the neighbours. Technology gives us the possibility to become neighbour with people of different time and space. However, are these real interactions? Are we the neighbour close enough or simply far away?

In this work, you will find multiple interactions between “human and machine”; “human who present at the same time or not”. How they interact with each other? What kind of behaviour they made? How one’s behaviour influences others? Through what kind of way, they organize their interaction? These are questions I wish to observe and explore in this project.

### Hardware Installation
The whole installation contains two parts. 1 MacBook Air and 1 projector.

MacBook :
A MacBook Air placed in front of a clean background with webcam turned on acts as a photo booth which is used for letting visitors to interact and shoot GIF image with.

Projector :
A projector projecting 8*5 grids on the wall. Once visitor shot a GIF image on MacBook Air, it shows the created GIF image on the wall simultaneously.

<div style="text-align:center;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1IpuVMuNk-YYeMvYdMzdyt2bU5WqW8GRZ" width="100%" height="auto" />
</div>

### Software Method
For Software implementation, I created server and client two repositories. Server is based on Node.js and is locally put on the Macbook Air. I chose React.js as frontend framework for client side. The logic of how it functions can be divided into three levels: input, display and control. Following I will describe each level in detail:

**Input :**
The first page of input side shows 8*5 grids with 85px width and height as well as an instruction below telling visitors that they should shoot image related to its neighbors. Visitor can click on one of the grids and start to shoot their own GIF.

<div style="text-align:center;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1AWiDE0oPXcM4cZxPcVLY45BbilHFZClD" width="100%" height="auto" />
</div>

**Display :**
Display side was projected on the wall showing 8*5 grids with 150px width and height. These grids have same ids as grids on input side. Therefore, once visitor chose a grid on input side and shot a GIF, the image will be displayed on the corresponding grid. The communication is control by Socket.IO, which will be explained in the following section.

<div style="text-align:center;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1FLRjTq0h1oJJJG7RSTs1EjuumWVkTv3q" width="100%" height="auto" />
</div>

**Control :**
In order to connect input and display, I took advantage of socket.IO. It listens on the channel, once a GIF image was shot on input side, socket.IO emits the image to grid with same id on display side.

<div style="text-align:center;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1vBsZkVVxncruWt0jGioDsA0bhF2woS8z" width="100%" height="auto" />
</div>

### Note:
This project was invited to exhibit in [MINT-Tag 2019](https://www.minttag-bremen.de/events/die-nachbarn/) in Bremen Universum.
<div style="text-align:center;margin-bottom:40px;">
<video id="video" width="640" height="auto" controls poster="/images/neighbors-2.png" preload="auto">
<source id="mp4" src="/images/universum-minttag-eventfilm-720p.mp4" type="video/mp4">
</video>
</div>
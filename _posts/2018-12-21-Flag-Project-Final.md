---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of Malaysia

## Describe your program

I designed this flag for Malaysia.
I expect either a 3 or a 4 because I tried using variables and scaling and making the flag as close as possible to the real flag. i tried my best to sclae the flag but I was not able to complete this task fully due to the fact my canton was made using the base layer.

## Current output

* * *
![download](/images/malaysianflag.png)
* * *

## Describe your process.

First I started out by making a collage of the flag I had to make. Then I moved on to making the program, first I made a scrap flag that had all the sizes and the layout of the flag planned out making it easier to define the variable and decide on sizes for the stripes. I had to create a flag base large enough to hold 14 stripes evenly accounting for the hieght of the flag. This is the process I went through to make the flag the way it is now.


## Explain your code.

The first argument I wrote is for the base of my flag which holds all the other images on top of this base. Next I made a short red stripe to fit with the canton and I made a short white one as well to make the red and white stripes. Then I made a red and white long line to make the rest of the flag. Then I made two circles one blue and one gold to make the cresant shape for the canton of my flag. Then I made a radial star for the star in the canton making my flag definitions complete.

Each function in this peice fo code does one think to make the whole flag come together as a whole image. Such as the stripes which makes the stripes of the flag and the base which holds all the images on top of it. 

* * *

```
(define base (rectangle 500 280 "solid" "blue"))
(define shortred (rectangle 280 stripe-height "solid" "red"))
(define longred (rectangle 1000 stripe-height "solid" "red"))
(define shortwhite (rectangle 280 stripe-height "solid" "white"))
(define longwhite (rectangle 1000 stripe-height "solid" "white"))
(define bluecircle (circle 40 "solid" "blue"))
(define goldcircle (circle 40 "solid" "gold"))
(define goldstar (radial-star 14 15 40 "solid" "gold"))
```

* * *
This code is all the definitions I used to make my flag and how these peices together make every part of my flag possible making it a essential part of my code to make this flag.


## Program code

```(define width 500)
(define height 280)
(define stripe-height (/ height 14))

(define base (rectangle 500 280 "solid" "blue"))
(define shortred (rectangle 280 stripe-height "solid" "red"))
(define longred (rectangle 1000 stripe-height "solid" "red"))
(define shortwhite (rectangle 280 stripe-height "solid" "white"))
(define longwhite (rectangle 1000 stripe-height "solid" "white"))
(define bluecircle (circle 40 "solid" "blue"))
(define goldcircle (circle 40 "solid" "gold"))
(define goldstar (radial-star 14 15 40 "solid" "gold"))



(define flag (put-image goldstar 120 210
             (put-image bluecircle 80 210
             (put-image goldcircle 60 210
             (put-image longwhite 360 10
             (put-image longred 360 (* 1.5 stripe-height)
             (put-image longwhite 360 50
             (put-image longred 360 70
             (put-image longwhite 360 90
             (put-image longred 360 110
             (put-image shortwhite 360 130
             (put-image shortred 360 150
             (put-image shortwhite 360 170
             (put-image shortred 360 190
             (put-image shortwhite 360 210
             (put-image shortred 360 230
             (put-image shortwhite 360 250 
             (put-image shortred 360 270 base))))))))))))))))))



(define outline (rectangle width height "outline" "black"))

(overlay outline flag)
```

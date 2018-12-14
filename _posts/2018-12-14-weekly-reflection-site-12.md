---
layout: post
title: "Evan Espina's Twelfth Weekly Reflection"
date: 2018-12-14
---

```
(define base (rectangle 500 280 "solid" "blue"))
(define shortred (rectangle 280 20 "solid" "red"))
(define longred (rectangle 1000 20 "solid" "red"))
(define shortwhite (rectangle 280 20 "solid" "white"))
(define longwhite (rectangle 1000 20 "solid" "white"))

(put-image shortred 360 230
 (put-image shortwhite 360 250 
  (put-image shortred 360 270 base)))
```

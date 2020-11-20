---
title: "Digital Image Correlation using Fast Fourier Transform (MATLAB and Python)"
layout: post
date: 2020-11-17 18:00
image: /assets/images/markdown.jpg
headerImage: false
tag:
- digital image correlation
- FFT
- Python
- MATLAB
category: blog
author: jarlathdolan
description: DIC using FFT
---

At its core, my graduate research project relied on one solitary software process: 2D cross-correlation.

The project itself involved the capturing of extremely minute eye movements using an optical sensor, but in order to actually *measure* this movement, some sort of function was required that would take a series of captured images as inputs and spit out a quantitative value of movement.

As expected, MATLAB's Signal Processing Toolbox already has a 2D cross-correlation function, [`xcorr2`](https://uk.mathworks.com/help/signal/ref/xcorr2.html). Computationally however, this method is rather cumbersome, particularly if large datasets of images are involved. A much quicker way to achieve 2D cross-correlation is through the application of the Fast Fourier Transform (FFT).

 

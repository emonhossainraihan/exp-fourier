# Exp Fourier Transformation

## The Tricky Part:

- **The blue graph measures the real part of the cycle**. Another lovely math confusion: the real axis of the circle, which is usually horizontal, has its magnitude shown on 
the vertical axis. You can mentally rotate the circle 90 degrees if you like.
- **The time points are spaced at the fastest frequency**. A 1Hz signal needs 2 time points for a start and stop (a single data point doesn't have a frequency). 
The time values `[1 -1]` shows the amplitude at these equally-spaced intervals.

`[0 1 1]` means "Nothing at 0Hz, 1Hz of amplitude 1, 2Hz of amplitude 1"

 With 3 cycles defined `(0Hz, 1Hz, 2Hz)`, each dot is 1/3 of the way through the signal. In this case, cycles `[0 1 1]` generate the time values `[2 -1 -1]`, 
 which starts at the max (2) and dips low (-1).
 
 Use `magnitude:angle` to set the phase. So `[0 1:45]` is a 1Hz cycle that starts at 45 degrees.
 
 [Here](https://betterexplained.com/articles/an-interactive-guide-to-the-fourier-transform/) is the original blog. 

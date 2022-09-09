---
title: Trigonometry
layout: page
menuInclude: yes
menuLink: yes
menuTopTitle: Precalculus
menuSubs:
- title: Trigonometry
  index: 2
excerpt: "Discussing trig"
terms:
  - ['Radian', 'A unit of measurement for an angle, with one degree equal to \(\frac{\pi}{180}\) radians. 180° is equal to \(\pi\) radians and 360° is equal to \(2 \pi\) radians.']
  - ['Unit Circle', 'The circle with radius 1 centered at (0,0). It is very helpful when working with trigonometric functions.']
  - ['Period', 'How long it takes for a curve to repeat its pattern']
---


<h1>Precalculus</h1>

<h2>Trigonometry</h2><br>

In geometry, you learned about the three common trigonometric functions: sine, cosine, and tangent. Let's do a little bit of review:

To get the sine of an angle, take the length of the side opposite the angle and divide that by the length of the hypotenuse. Cosine and tangent work the same, except cosine is adjacent divided by hypotenuse and tangent is opposite divided by adjacent.

(images)

Before moving forward, it's important to have a firm understanding of <b>radians</b>. A degree is a unit measurement for an angle, with 360° being a full circle and 180° being a straight line. A radian is a similar measurement for a degree, except it is in terms of \\(\pi\\).

0 degrees corresponds to 0 radians. While 360 degrees is a full circle, 2pi radians is also a full circle. From those two facts, we can fill in the blanks. A right angle in degrees is \\(\frac{360}{4}\\), and a right angle in radians is \\(\frac{2\pi}{4} = \frac{\pi}{2}\\). The formula for converting degrees to radians is

$$\text{radians} = \text{degrees} \cdot \frac{\pi}{180}$$

The formula for converting radians to degrees is

$$\text{degrees} = \text{radians} \cdot \frac{180}{\pi}$$

(table for degrees and radians)

Now, let's look at sine, cosine, and tangent as functions instead of geometrically. Let's look at the sine function. The sine function takes in an angle measurement (usually in radians) and will output a number between \\(-1\\) and \\(1\\). That number is the ratio of the opposite side to the hypotenuse. To find out the shape of this graph, it is helpful to look at a circle. Take a look at the following circle with radius 1 (known as a <b>unit circle</b>, with triangles within it:

(image)

No matter the angle \\(\theta\\), line ????? stays at a length of 1. This is because of the nature of equidistance in circles. However, line ????? varies in length. Let's zoom into one instance of this circle:

(image)

It seems like a right triangle just pops out of nowhere. Labeling the sides, we have:

(image)

Now, using our definition from earlier, we can clearly see that \\(\sin(\theta) = \frac{\text{length of line ????}}{\text{length of line }?????}\\). Because the length of line ????? is always 1, we can say that \\(\sin(\theta) = \frac{\text{length of line }????}{\text{length of line }?????}\\). This is an important discovery - it shows us that \\(\sin(\theta)\\) is directly equal to the height of line ??????.

Using this information, we can follow \\(\theta\\) around the full \\(2pi\\) radians to see the following:

(image)

This gives us the shape of \\(\sin(\theta)\\).

<center><video width="450" height="370" autoplay loop muted>
  <source src="/videos/sine_curve_circle.mp4" type="video/mp4" />
</video></center>

Now, let's do a similar process for cosine.

Here, we can see that \\(\cos(\theta)\\) is equal to the length of line ???? divided by the length of the hypotenuse. Again, because the length of the hypotenuse is always \\(1\\) no matter the value of \\(\theta\\), \\(\cos(\theta)\\) is equal to the length of line ?????

This gives us the shape of the cosine curve:

(image)

Something to notice is how the graphs of sine and cosine will repeat. Because the unit circle has a circumference of \\(2\pi\\), it means that the values for sine and cosine will repeat every \\(2\pi\\) units. This is known as the <b>period</b> of the curve. The period is how long it takes for the curve to repeat its pattern.

  

Now, let's talk about tangent. \\(\tan(x)\\) is defined to be \\(\sin(x)\\) divided by \\(\cos(x)\\). This is why the tangent of an angle is equal to opposite over adjacent.

$$\begin{align*}
\sin(x) &= \frac{\text{Opp}}{\text{Hyp}}\\
\cos(x) &= \frac{\text{Adj}}{\text{Hyp}}\\
\tan(x) &= \frac{\sin(x)}{\cos(x)}\\
\tan(x) &= \frac{\frac{\text{Opp}}{\text{Hyp}}}{\frac{\text{Adj}}{\text{Hyp}}}\\
\tan(x) &= \frac{\text{Opp}}{\cancel{\text{Hyp}}}\cdot\frac{\cancel{\text{Hyp}}}{\text{Adj}}\\
\tan(x) &= \frac{\text{Opp}}{\text{Adj}}
\end{align*}$$

This is the graph of \\(\tan(x)\\) overlaid over the graphs of \\(\sin(x)\\) and \\(\cos(x)\\). You can see how when \\(\sin(x)\\) is 0, \\(\tan(x)\\) is 0 (because 0 divided by anything is 0), and when \\(\cos(x)\\) is 0, \\(\tan(x)\\) has no value (because anything divided by 0 is undefined).

  

(image)

  

There are three other functions to know: \\(\csc(x)\\), \\(\sec(x)\\), and \\(\cot(x)\\). They are fairly simple:

  

$$\csc(x) = \frac{1}{\sin(x)}$$

$$\sec(x) = \frac{1}{\cos(x)}$$

$$\cot(x) = \frac{1}{\tan(x)}$$

  

Here are their graphs:

  

(image)

  

And here are the graphs of all 6 functions overlaid:

  

(image, use matplotlib legend)

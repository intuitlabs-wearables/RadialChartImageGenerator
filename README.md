# RadialChartImageGenerator
A simple tool that generates images for animating radial progress charts for the Apple Watch and WatchKit.

![animation1](docs/animate1.gif) ![animation2](docs/animate2.gif) ![animation3](docs/animate3.gif)

## Overview

#### Why care about radial progress charts?
* Clearly, Apple likes radial progress charts which are used in their activity monitor health watch app ([Apple Health & Fitness Watch App](https://www.apple.com/watch/health-and-fitness/)).

* Radial charts are just the right way to display a large amount of data on such a small screen size.

* We as humans have been trained to read radial progress charts from a very young age - clocks. That's why it makes a lot of sense to use them on a watch.

#### Why use the RadialChartImageGenerator?

* The Apple WatchKit SDK does not have a built-in tool or library to create these charts or any visualization.

* The way Apple WatchKit SDK allows animations or visualizations is to use a sequence of static images ([WatchKit Design Guidlines](https://developer.apple.com/library/prerelease/ios/documentation/UserExperience/Conceptual/WatchHumanInterfaceGuidelines/Animation.html#//apple_ref/doc/uid/TP40014992-CH7-SW1)). In fact, Apple's own WatchKit sample app called [Lister](https://developer.apple.com/library/prerelease/ios/samplecode/Lister/Introduction/Intro.html) does animations of this radial progress chart using 360 different static images of the chart. Good luck creating hundreds of images by yourself.

* The RadialChartImageGenerator comes in to the rescue. With a few clicks, you can select whether you want a single, double, or triple arc radial chart (images shown above), customize the colors and text, and choose how many values or capacity the chart should have. The generator will finally generate every permutation of the radial progress chart and download a zip file with all the images. The alternative is to create these images manually in an image editor program like Photoshop, which would require a lot of effort and time. The RadialChartImageGenerator is a very simple tool that saves so much time with minimal effor. 

## How To Use

#### Instructions

1. Go to http://hmaidasani.github.io/RadialChartImageGenerator/ or open index.html.

2. Decide on whether you need a single, double, or triple arc radial chart.
![animation1](docs/how-to-2.png)

3. Choose the max value or the capacity of the appropriate arc.
![animation2](docs/how-to-3.gif)

4. Choose the arc background color.
![animation3](docs/how-to-4.gif)

5. Decide the color scheme for each appropriate arc. If you would like a gradient color scheme, choose three different colors for the foreground start, mid, and end colors. In order to see how this looks, choose the current value to be equal to the max value to see the full arc gradient. **Note: the current value has no effect on the output of the images - it is merely there to see how the arc would look at a given value.**
![animation4](docs/how-to-5.gif)

6. For the single arc, you may select if text should appear in the center. You may also select the text color and the units of the subtext.
![animation5](docs/how-to-6.gif)

7. Once you have modified each arc to your preference, click the Generate Images button to generate each permutation of images for the given arc structure. Enter the filename prefix of your choice and click on Continue.
![animation6](docs/how-to-7.gif)

8. The images should download in a zip file.

9. Repeat for all the other arcs if needed.

#### Examples

Coming soon - sample WatchKit instructions/app using the images generated using the RadialChartImageGenerator.

## Questions & Feature Requests

Report all of your questions and feature requests to the issues section of git repository.

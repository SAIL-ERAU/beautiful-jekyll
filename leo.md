---
layout: page
title: LEO SmallSats and Debris
subtitle: Tracking and photometry of low Earth orbit satellites
css: "/css/index.css"
bigimg:
    - "/img/popacs3-1-20-i1180_new.png" : "POPACS-3 (Jan 20, 2016)"
---
<!-- js: "/js/plotly.js" -->

## Bringing small satellites to light

OSCOM's primary focus is _characterization_ and _operational mission support_ of CubeSats, nanosats, and small debris. Precision photometry of these objects in low Earth orbit (LEO) is difficult not only because of the high angular rate as these objects pass over the observatory site, but even with accurate timekeeping and telescope pointing, the accuracy of source orbital elements for small resident space objects is often lacking. These challenges drive several considerations in OSCOM's electro-optical and tracking system design---mainly a fairly wide field of view and the ability to dither the telescope along the satellite track during a pass.

An example of testing acquisition and tracking controls of NRL's SpinSat small satellite through a small Borg refractor is shown below. At the beginning of the video, the telescope is staring at a star field and waiting for SpinSat to enter the field of view. When it enters, the telescope begins tracking the satellite, which is now visible as a dot while the stars streak by. The dot moves SpinSat is  moved left/right and up/down in the field of view as the mount controls are tested during tracking.

<iframe width="90%" height="400px" src="https://www.youtube.com/embed/KZGikQRROiQ" frameborder="0" allowfullscreen></iframe>

## Temporally resolved observations

An additional challenge for OSCOM is capturing multi-hertz photometry of these small, dim objects. To accomplish this, we most often deploy the optically fast [11" RASA telescope]({{site.baseurl}}/facilities-and-equipment/#equipment-rasa). Over the past two years, the OSCOM system has recorded several terabytes of raw photometric images of nearly every kind of satellite in LEO. Our ability to record temporally resolved photometry of even small satellites is demonstrated in the extinction and range normalized light curves below:

#### CanX-6
<img style="float: right; margin: 0px 0px 15px 15px;" src="..\img\canx6.jpg" width="20%" />

[CanX-6](http://utias-sfl.net/?page_id=205) is a 6.5 kg nanosatellite built by the University of Toronto Institute for Aerospace Studies Space Flight Laboratory (UTIAS-SFL). It's primary mission is a demonstration of space-based automatic identification system (AIS) detection technology. The satellite uses the 20 cm cube Generic Nanosatellite Bus and is in a 630 km orbit.

<script src="/beautiful-jekyll/js/plotly.js"></script>
{%include canx6.html %}

#### CanX-3a
<img style="float: left; margin: 0px 0px 15px 15px;" src="..\img\canx-3a.jpg" width="20%">

CanX-3a, also known as [UniBRITE](http://utias-sfl.net/?page_id=407), uses the same Generic Nanosatellite Bus (GNB) as CanX-6 with 4 UHF wire antennae and a magnetometer, but with the notable absence of CanX-6's VHF payload antenna. CanX-3a has a small telescope for obtaining exoplanet photometry measurements, and therefore requires accurate 3-axis attitude control. OSCOM has observed most of the CanX satellites on many occasions. Below is a typical lightcurve from an observation of CanX-3a.

<script src="/beautiful-jekyll/js/plotly.js"></script>
{%include canx3a.html %}

<!-- #### DICE -->
<!-- TODO: Include video because it flashes -->

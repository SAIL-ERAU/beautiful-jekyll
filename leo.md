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

OSCOM's primary focus is **characterization** and **operational mission support** of CubeSats, nanosats, and small debris. Precision photometry of small objects in low Earth orbit (LEO) is difficult not only because of the high angular rate as they pass over the observatory site, but even with accurate timekeeping and telescope pointing, the accuracy of source orbital elements for small resident space objects is often lacking. These challenges drive several considerations in OSCOM's electro-optical and tracking system design---mainly a fairly wide field of view and the ability to dither the telescope along the satellite track during a pass.

A test of acquisition and tracking of NRL's SpinSat 22 inch diameter satellite through a small Borg refractor is shown below. At the beginning of the video, the telescope is fixed staring at a star field and waiting for SpinSat to enter the field of view. When it enters, the telescope begins tracking the satellite, which is now visible as a dot while the stars streak by. SpinSat is  moved left/right and up/down in the field of view as the mount controls are tested during tracking.

<iframe width="90%" height="400px" src="https://www.youtube.com/embed/KZGikQRROiQ" frameborder="0" allowfullscreen></iframe>

## Temporally resolved observations

An additional challenge for OSCOM is capturing multi-hertz photometry of these small, dim objects. To accomplish this, we often deploy the optically fast [11" RASA telescope]({{site.baseurl}}/facilities-and-equipment/#equipment-rasa). Over the past two years, the OSCOM system has recorded several terabytes of raw photometric images of nearly every kind of satellite in LEO. Our ability to record temporally resolved photometry of even small satellites is demonstrated in the light curves below.

OSCOM has built a multi-threaded Python package called the Optical Satellite Analysis Toolkit (OSAT) which performs image reduction, processing, photometry, satellite magnitude corrections, and time series analysis. Typical processing of small satellite photometry consists of conventional bias and flat field image reduction and aperture photometry with robust background fitting.

### Sample Light Curves

Below are several sample light curves showing the brightness of small satellites over time as recorded by OSCOM. Each of these light curves are corrected for first order atmospheric extinction and normalized for satellite slant range to the observer. The peak magnitude values roughly correspond to the apparent magnitude at which they would be observed by eye in the sky.

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

#### DANDE
<img style="float: right; margin: 0px 0px 15px 15px;" src="..\img\dande.png" width="20%">

DANDE, the [Drag and Atmospheric Neutral Density Explorer](http://spacegrant.colorado.edu/boulderstudents/boulderprojects/dande), is a 46 cm diameter spherical microsatellite built by University of Colorado at Boulder for characterizing atmospheric drag in low Earth orbit. DANDE is covered in flat solar cells and attitude controlled to spin at 10 rpm with the spin axis aligned cross-track. Contact was lost with the satellite in early 2014.

<script src="/beautiful-jekyll/js/plotly.js"></script>
{%include dande.html %}

<!-- #### DICE -->
<!-- TODO: Include video because it flashes -->

# Near Earth Objects Sample Capstone
Sample Capstone Project analyzing data from NASA about Near-Earth Comets (NECs) and Asteroids (NEAs).
<br >

## About the Data

This dataset is from NASA ([accessible here](https://data.nasa.gov/dataset/wise-nea-comet-discovery-statistics)). It contains information about Near-Earth Comets (NECs, perihelion distance < 1.3 au*) and Asteroids (NEAs, perihelion distance < 1.3 au*) discovered recently. The data contains 202 rows of unique Near-Earth Objects (NEOs, inclusive of both asteroids and comets). Each record has:
* **Designation:** The name/number of the NEO
* **Discovery Date:** The date the NEO was first discovered
* **H (mag)/Magnitude:** Absolute magnitude, which is the intrinsic brightness of a celestial body, measured in magnitudes, computed as if viewed from a distance of 10 parsecs, or 32.6 light years
* **MOID (AU):** Minimum Orbit Intersection Distance, defined as the distance between the closest points of the orbits of two bodies, in this case the Earth and the NEO, measured in Astronomical Units (au)*
* **q (AU)/Perihelion:** Perihelion distance, which is the point in the orbit of an object where it comes closest to the sun, measured in Astronomical Units (au)*
* **Q (AU)/Aphelion:** Aphelion distance, which is the point in the orbit of an object where it is farthest from the sun, measured in Astronomical Units (au)*
* **period (yr)/Period:** The sidereal orbital period of the NEO, or the amount of time it takes the object to complete one orbit around the Sun, measured in Earth years
* **i (deg)/Inclination:** The angle of the object’s orbit, with respect to the x-y ecliptic plane (what we would consider “flat”), measured in degrees
* **PHA:** Binary classification of whether or not the object is a Potentially Hazardous Asteroid (PHA), defined as NEAs with MOID<=0.05 au* and absolute magnitude (H)<=22.0
* **Orbit Class:** The object’s classification based on its orbital characteristics. NEAs are divided into groups (Atira, Aten, Apollo and Amor) according to their perihelion distance (q), aphelion distance (Q) and their semi-major axes (a). NECs are classified as Encke-type Comet, Jupiter-family Comet, Halley-type Comet, or Comet, based on their orbital period and inclination.
    * **Atira:** NEAs whose orbits are contained entirely with the orbit of the Earth; a<1.0 au, Q<0.983 au
    * **Aten:** Earth-crossing NEAs with semi-major axes smaller than Earth's; a<1.0 au, Q>0.983 au
    * **Apollo:** Earth-crossing NEAs with semi-major axes larger than Earth's; a>1.0 au, q<1.017 au
    * **Amor:** Earth-approaching NEAs with orbits exterior to Earth's but interior to Mars'; a>1.0 au, 1.017<q<1.3 au
    * **Encke-type Comet:** Short-period comets (<200 year orbit) with orbits that do not reach the orbit of Jupiter
    * **Jupiter-family Comet:** Short-period comets with orbital periods less than 20 years and low inclinations (up to 30 degrees)
    * **Halley-type Comet:** Short-period comets with orbital periods of between 20 and 200 years and inclinations extending from 0 to more than 90 degrees
    * **Comet:** Long-period comets with an orbital period of 200+ years

\* The Astronomical Unit (au) is a unit of length defined to be exactly equal to 149,597,870,700 meters, approximately the average distance between the Sun and Earth.
<br ><br >

## Project Overview

**Problem Statement:** We want to be able to understand the patterns in the NEO data, so we can predict potential hazards and be better equipped to identify additional NEOs in the future.

**Business Questions:**
* Were there certain years where more PHAs were discovered?
* Is there a relationship between Aphelion distance and Perihelion distance (in other words, are orbits roughly similar in shape or proportion regardless of scale)?
* What proportion of NEOs discovered recently are PHAs?
* What is the range of orbital periods?
* Are certain classes of NEOs more likely to be PHAs?

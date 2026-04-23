(light-diffraction-lasers-and-geometric-optics-imaging-overall)=
# 1146L-ONLY | Light – Geometric Optics and Imaging

<!--- # 1146L-ONLY | Light – Diffraction with Lasers & Geometric Optics and Imaging


```{danger}
**⚠️ LASERS IN USE TODAY ⚠️**

**DO NOT SHINE THE LASER INTO ANYONE'S EYES**

**YOU AND OTHERS CAN GO BLIND**
```


## Background – Part I – Multiple Slit Diffraction

### Overall goals and overview

- Investigate diffraction of light and its relation to multiple-slit spacings and light wavelength with a monochromatic laser.
- Investigate reflected light diffraction and its relationship to size of the reflective object's topography, again with a monochromatic laser.
- Investigate light refraction through lenses, both unfiltered and chromatically or spherically filtered by determining focal lengths with image and object distances.
- In today's lab, you will complete three experiments:
  - **Experiment 1**: Shine a laser through multiple slits of known spacing, creating a diffraction pattern on a far wall. Tape a piece of paper centered on the pattern, trace the pattern, then measure the spacing between the dots. Determine the wavelength and compare to the actual value of the laser.
  - **Experiment 2**: Shine a laser on a music CD to create a reflected diffraction pattern. Using the spacing of the diffraction pattern and wavelength determined in Experiment 1, determine the spacing between the physical tracks (pits) indented in the plastic of the CD. Compare to the known value given in the procedure. Consider how the diffraction spacing relates to the topography of the CD.
  - **Experiment 3**: Determine focal lengths of the lens first unfiltered at various distances, then chromatic filtering through red and blue filters, then spherical aberration near center and edge of the lens; consider the physical reasoning for longer or shorter focal lengths depending on differences in the filtering or refracting of the light source. Plot image vs. object distance pairs for the unfiltered distances and investigate the convergence point; compare that value to your average of focal lengths from the unfiltered portion of this experiment.

Multiple slit diffraction will be used first to find the wavelength of a laser light source. Having determined the wavelength of the laser light, that combined with the reflected diffraction pattern will be used to determine the spacing between the tracks of a standard music CD (compact disc).

To understand diffraction, we will consider the interference of various parts of a wavefront as they emerge from a transmission diffraction grating. The transmission grating is much like the openings formed by partially open window blinds. The diffractive effects result from the interference of the various portions of the same wavefront as they are formed by passing the wavefront through the diffraction grating. 

The number of slits that are actually used in the experiment is very large. To quickly understand diffraction from multiple slits, we will consider the pattern of constructive interference of the portions of the wavefront that emerge from two, narrow slits, spaced a distance $d$ apart as illustrated in {numref}`Figure {number} <fig-two-slit-wavefronts>`.

```{figure} OpticsFigures/Figure01.jpg
:name: fig-two-slit-wavefronts
:alt: Two-slit wavefront diagram showing interference patterns
:width: auto
:align: center

Two-Slit Wavefronts
```

The analysis of the resulting diffraction pattern after the light passes through the slits rests on two fundamental principles. The first, Huygen's principle, states that each portion of a wavefront can be considered a separate radiating source. The second is linear superposition; that is, the total field vector at any given position is the vector sum of the individual field vectors simultaneously present.

The portion of the wavefronts that are present in the slits are considered Huygen sources of radiating spherical wavelets. The wavelets then interfere with each other to form new wavefronts. (If a plane wave were radiating unimpeded in free space, each of these wavelets would interfere to form additional plane waves propagating in the same direction as the original wavefront.) However, when portions of a wave-front are deleted as they are here, the interference will form a diffraction pattern that is very different from the plane wave that would have been formed (see example in {numref}`Figure {number} <fig-double-slit-diffraction>`).

```{figure} OpticsFigures/Figure_10_diffraction_v02.png
:name: fig-double-slit-diffraction
:alt: Double slit diffraction pattern showing constructive and destructive interference
:width: auto
:align: center

Double Slit Diffraction. (A) Light spreads out (diffracts) from each slit, because the slits are narrow. These waves overlap and interfere constructively (bright spots) and destructively (dark regions). We can only see this if the light falls onto a screen and is scattered into our eyes. (B) When light that has passed through double slits falls on a screen, we see a pattern such as this.
```

Consider the schematic in {numref}`Figure {number} <fig-double-slit-diagram>`; when the path length difference is equal to an **integral number of wavelengths** of the light, then the wavelets from each of the slits will **constructively interfere** and produce a bright spot. Notice that this condition occurs at angles when

```{math}
:label: eq-sin-theta
d \sin\theta_{n} = n \lambda
```

where $n$ is an integer ($\pm$) and $\lambda$ is the wavelength of the light.

Thus we can expect to see bright spots on the wall/paper/board, when the angle from the initial direction of the laser beam satisfies the above criterion. For the small angles we are dealing with here, the distance from the initial bright spot, when $n$ = 0, and therefore $\theta$ = 0, to each of the diffracted spots is given by

```{math}
:label: eq-y-distance
y_{n}= X \tan\theta_{n} \simeq X \sin\theta_{n}
```

where $X$ is the distance to the screen, and $n$ is the order number.

Combining these two equations

```{math}
:label: eq-y-combined
y= m X \lambda /d
```

For small angles, $\sin\theta_{n} \sim \theta_{n}$ (in radians). For the small angles we are dealing with here, the distances $y$ are very small with respect to $X$. Under these conditions, you can measure the distance between neighboring spots and then average all of these measurements to get a reasonably good number to use for $\Delta y$. From {eq}`eq-y-combined`, $\Delta y = X \lambda / d$, or

```{math}
:label: eq-wavelength
\lambda=\Delta y d / X
```

The slit spacing $d$ is given, you determine laser wavelength, and you can compare your results with the known wavelength of the HeNe (Helium Neon) laser you are using.

```{figure} OpticsFigures/Figure02.jpg
:name: fig-double-slit-diagram
:alt: Double slit diffraction geometry showing path difference and angle relationships
:width: auto
:align: center

Double Slit Diffraction
```




### Equipment

**Experiment I**

The setup will appear in similar form to that seen in {numref}`Figure {number} <fig-experimental-setup>` with laser pointed towards the diffraction grating which creates the diffraction pattern as seen earlier in {numref}`Figure {number} <fig-double-slit-diffraction>` right.

```{figure} OpticsFigures/Figure_20_experimentalSetup.png
:name: fig-experimental-setup
:alt: Laser mounted on black optics track pointed towards diffraction grating
:width: auto
:align: center

Left) Laser mounted on black optics track pointed towards the diffraction grating as seen on the right.
```

- Diffraction grating with multiple slits of spacing $d=0.20\,\text{mm}$
- Red HeNe laser with known value $\lambda_{\text{HeNe}}=632.8\,\text{nm}$ and power source
- Black optics track to mount everything
- 30 m long metric tape measure
- White paper and tape

**Experiment II**, discussed further after experiment I.

- Music CD with $\sim 1.6 \times 10^{-6}\,\text{m}$ track spacing (see close-up example in {numref}`Figure {number} <fig-cd-tracks>` left)
- Red HeNe laser with known value $\lambda_{\text{HeNe}}=632.8\,\text{nm}$ and power source
- Black optics track to mount everything
- Metric ruler vertically mounted with hole to allow laser to pass through

--->




<!---
**Experiment III**, discussed further after experiment II.

- Black optics track to mount everything
- Light box with image on it (position of image noted by indented metal aligned with the ruler on the optics track) with power brick
- Convex lens in lens holder (position of the lens in the holder is noted by a small plastic protrusion on the side of the holder to be lined up with the ruler on the optics track)
- Red and blue filter -- attaches to light box
- Disk and annulus mask filters -- attached to lens holder
- White viewing screen (movable along the optics track)

--->




<!---


## Experimental Procedure – Part I: Multiple Slit Diffraction Grating

```{danger}
**DO NOT SHINE THE LASER INTO ANYONE'S EYES**

**YOU AND OTHERS CAN GO BLIND**
```

1. Turn on the laser and allow the beam to pass through the diffraction grating and form the diffraction pattern on the far wall. Tape a white sheet of paper on the wall at the position of the pattern. You should see a center bright spot with a series of evenly spaced diffraction spots above and below the center bright spot.

2. **WHILE BEING CAREFUL NOT TO LOOK BACK INTO THE LASER**, mark the location of each spot on the paper by carefully circling each spot on the paper.

3. Using the steel metric tape measure, measure the distance from the diffraction grating to the paper screen on the blackboard.

4. Remove the paper. Measure and record in a data table the coordinate of the center of each spot relative to the bottom edge of the paper (to have a consistent spot to measure from). Calculate and record in the data table the center to center distances between each spot and its nearest-neighbor spot by subtracting their coordinates. Calculate and record the average and standard deviation of these distances. As you can see from {eq}`eq-y-distance`, the spacing should not be exactly the same. However, for the very small angles and range of angles we have here, they can be considered evenly spaced. This is of course the small angle approximation of the sine function.

5. Calculate the wavelength of the laser using {eq}`eq-wavelength` and compare it to the known value $\lambda_{\text{HeNe}}=632.8\,\text{nm}$. The diffraction grating spacing is $d=0.20\,\text{mm}$, $200\,\mu\text{m}$, many times larger than the spacings of the CD tracks you will see in Part II.




--->


<!---

## Background – Part II – Reflected Diffraction Pattern

For the second part of the diffraction experiment, we will use the **now known wavelength** of the light source to measure the spacing of an unknown array of slits. The unknown slits are the tracks of a CD (compact disc) with a zoomed in example shown in {numref}`Figure {number} <fig-cd-tracks>`.

```{figure} OpticsFigures/Figure_11_diffraction_v02.png
:name: fig-cd-tracks
:alt: Topography of CD ROM showing track spacing
:width: auto
:align: center

Topography of a CD ROM. Lower capacity music CD on left, higher capacity DVD on right where the tracks are more closely packed together.
```

Regarding a CD, before data is written to it, you would have just a flat surface. During manufacturing, for data to be written to the CD, a long, spiral track containing all the data (songs in the case of a music CD) is stamped into the plastic. This process creates little divots, called pits, into the plastic substrate; that surface is later metalized with aluminum to create a shiny, reflective surface. The spiral track is made to be a consistently spaced, spiral line of pits and flat surfaces that are $\sim 1.6 \times 10^{-6}\,\text{m}$ or $1.6\,\mu\text{m}$ apart (see {numref}`Figure {number} <fig-cd-tracks>`). To a laser, these pits act like slit-shaped mirrors that can reflect the laser light back at different angles, effectively creating the sources a new spherical wavelets. The subsequent reflected wavelets will interfere either constructively or deconstructively and create a reflected diffraction pattern whose characteristics depend on the wavelength of the laser and spacing the of CD tracks. Thus the analysis is the same as the transmission slits we used in part I, except we will reflect the laser beam from the CD rather than transmit it through as we did before. Because the spacing of the tracks of the CD are very small, the diffraction angles are large and small angle approximations cannot be used.

```{figure} OpticsFigures/Figure03.jpg
:name: fig-reflection-diffraction
:alt: Reflection diffraction pattern from CD ROM
:width: auto
:align: center

Reflection Diffraction of CD ROM
```

```{figure} OpticsFigures/Figure_21_experimentalSetup.png
:name: fig-cd-setup
:alt: Laser setup for CD reflection experiment
:width: auto
:align: center

Left) Laser mounted on black optics track pointed towards the CD. Center) Laser light passes through the ruler and reflects off the CD to create the diffraction pattern in (right).
```


The experiment is configured as illustrated in {numref}`Figure {number} <fig-reflection-diffraction>` and an example of the setup is in {numref}`Figure {number} <fig-cd-setup>`.

The spacing of the tracks of a CD are so small that you will see only the first order diffraction spots, i.e. $n = \pm 1$. With the large angle $\Theta$ expected, the distance $X$ can be about 30 cm and a standard sheet of graph paper can be used for the paper screen. From your measurements of $X$ and $\Delta y$, determine the diffraction angle $\Theta$ from the tangent relation. Using {eq}`eq-y-distance`, we can solve for the track spacing, $d$, as

```{math}
:label: eq-track-spacing
d=\lambda / \sin\theta
```


--->


<!---

## Experimental Procedure – Part II: Reflection Diffraction Grating

```{danger}
**DO NOT SHINE THE LASER INTO ANYONE'S EYES**

**YOU AND OTHERS CAN GO BLIND**
```


1. Turn off the laser before moving it. Set up the laser and CD ROM as shown schematically in {numref}`Figure {number} <fig-reflection-diffraction>`. Turn on the laser and adjust the apparatus so the bright, center spot is directly back towards the laser. You should see the first order diffraction spots, one above and one below the center bright spot and a second order diffraction spot above the center spot.

2. Using the scale, measure and record the distances $\Delta y_{1}$, $\Delta y_{-1}$ and $\Delta y_{2}$.

3. Average the $\Delta y_{1}$ and $\Delta y_{-1}$ and record the value.

4. Calculate the track spacing for each first-order diffraction spot and average the two determinations. Compare your calculated track spacing with the microscopically determined track spacing $1.6 \times 10^{-6}\,\text{m}$.

5. Calculate the angle of the second-order diffraction spot using {eq}`eq-sin-theta`. Compare the height $\Delta y_{2}$ of the second-order diffraction spot with the calculated height from {eq}`eq-y-distance`. Notice that you cannot use the small angle approximation here.


%\subsection{\textbf{OVERALL GOALS:}}
%\begin{itemize}
%    \item Understand fluid-flow continuity through different constrictions.
%    %\item Assume \textbf{we know the resistance} of your resistors, but \textbf{we don't know the capacitance} of the capacitors, and we need to determine those C values.
%    \item Determine flow-rate of our system using the Continuity Equation.
%    \item Understand Bernoulli's Principle of fluid flow at a constant height to investigate the Venturi effect and determine the pressure of a fluid at a constriction point (in a Venturi tube).
%    %\item Understand  \textit{DISCUSSION POINT}: 
%\end{itemize}




--->




## Background

### ● Background Overview

```{admonition} OVERALL GOALS
:class: note
Use an object, thin-lens approximation, image screen on an optics track to:
- Investigate light refraction, focal length, and magnification through lenses for light that is:
    - Unfiltered
    - Chromatically aberrated by narrow color filters
    - Spherically aberrated by lens shape
```

<!---
\section{Background~\textendash~Part III~\textendash~Geometric Optics \& Single Element Imaging}
--->
In today's experiment, the behavior of a simple, bi-convex (symmetric, oval shaped), converging lens will be investigated with the setup of an illuminated object whose light will pass through a thin, converging (convex) lens and be projected onto a white screen (example in {numref}`fig_optics_00_setup_equip`).

```{figure} OpticsFigures/Figure_00_InitialSetupExample_v03small.png
:width: auto
:name: fig_optics_00_setup_equip

Light box, converging lens, screen mounted on optics track.
```


### ● Light Rays, Lenses, Focal Lengths (Part I)


Under many circumstances, the behavior of light can be analyzed by assuming that light travels in straight-line paths called **light rays**. Light rays are a representation of what is actually a very narrow beam of light. Using this representation of light, the behavior of many optical elements such as lenses and mirrors, and optical instruments such as telescopes, microscopes, and projectors can be analyzed. The use of the ray model draws heavily on geometry, and is called **geometric optics**.

A convex or converging lens is shaped so that all light rays that enter it parallel to its optical axis intersect (or *focus*) at a single point called the **focal point** $F$ on the optical axis on the opposite side of the lens (shown in {numref}`fig_optics_02_ThinLensFocalLength`) at a distance along the optical axis from the center of the lens called the **focal length** $f$ of the lens. Look closely at the top ray that goes through the converging lens. Because the index of refraction of the lens is greater than that of air, Snell’s law tells us that the ray is bent toward the perpendicular to the interface as it enters the lens. Likewise, when the ray exits the lens, it is bent away from the perpendicular. The overall effect for a converging lens is that light rays are bent toward the optical axis. To reiterate, the point at which the rays cross is the focal point $F$ of the lens; the distance from the center of the lens to its focal point is the focal length $f$ of the lens.


```{figure} OpticsFigures/Figure_02_ThinLensFocalLength_v02.png
:width: auto
:name: fig_optics_02_ThinLensFocalLength

All object light rays that are parallel to the optical axis will focus to a single point $F$ at a distance from the center of the thin converging lens equal to the focal length $f$.
```



**Ray tracing** is the technique of determining or following (tracing) the paths taken by light rays. The rules for ray tracing for thin converging lenses are:

1. A ray entering a lens parallel to the optical axis passes through the focal point on the other side of the lens (ray 1 in {numref}`fig_optics_03_ThinLensTracingDistance`).
2. A ray passing through the center of either a converging or a diverging lens is not deviated (ray 2 in {numref}`fig_optics_03_ThinLensTracingDistance`).
3. A ray that passes through the focal point exits the lens parallel to the optical axis (ray 3 in {numref}`fig_optics_03_ThinLensTracingDistance`).


#### ○ Thin-lens Approximation

In addition to using the ray model of light, the lens that will be used will be analyzed under the **thin-lens approximation**. This approximation will assume that the thickness of the lens is very small compared with the focal length. The result of this assumption is that the bending of the rays as they pass through the lens is considered to have occurred at a plane surface through the mid-line of the lens, perpendicular to the principal axis (see example approximation illustrated in {numref}`fig_optics_03_ThinLensTracingDistance`). As mentioned earlier, the bending (refraction) actually occurs at both the entrance and exit surfaces separated by a finite distance (illustrated again later in {numref}`fig_optics_04_magnification`). Additionally, the paths of light rays are exactly *reversible*. This means that the direction of the arrows could be reversed for all of the rays in {numref}`fig_optics_03_ThinLensTracingDistance` and other ray diagrams shown throughout today's manual.


<!---
```{figure} OpticsFigures/Figure_01_ObjectImageOverview_v01.png
:width: auto
:name: fig_optics_01_objectImagePlane

Ray tracing light from object to inverted image. Red dots represent focal length from center of lens. Top ray from object parallel to axis will pass through focal length on image side towards image. Middle ray from object passing through center of lens takes a straight path towards image. Bottom ray passing through focal length on object side will become parallel to axis after lens.
```
--->

```{figure} OpticsFigures/Figure_03_ThinLensRayTracingDistance_v02.png
:width: auto
:name: fig_optics_03_ThinLensTracingDistance

Ray tracing light from object to inverted image. Red dots at focal points $F$ (symmetric about symmetric lens) represent distance from lens where parallel rays from one side of the lens will pass through on the opposite side. E.g. ray 1, parallel ray from the object crosses at $F$ on the image side after refraction. Middle ray (2) from object passing through center of lens takes a straight path towards image. Bottom ray (3) passing through focal point on object side becomes parallel to optical axis after lens. Object distance to lens is $s_\text{o}$, image distance to lens is $s_\text{i}$.
```





The relation of the focal length and the object and image distances under the assumption of a thin lens is given by the **thin-lens equation**:


```{math}
:label: eq-W2Beq1
\frac{1}{f}=\frac{1}{s_\text{object}}+\frac{1}{s_\text{image}}
```

where $s_\text{object}$ and $s_\text{image}$ are the object and image distances respectively. Imaging a very distant object can reasonably approximate the focal length of a converging lens. From {eq}`eq-W2Beq1`, if the object distance is very large $(s_\text{object} \rightarrow \infty)$ compared to the focal length of the lens, the image distance is essentially the focal length. That is to say, the image of a very distant object is essentially at the focal point. Very convenient distant point sources of light are stars whose images are indeed at the focal point. For our laboratory, if available, sunlight will do just fine. Closer "distant" objects in the laboratory will give reasonable approximations to the focal length of the lens used in this laboratory.


To properly use the thin-lens equation, the following **sign conventions** must be obeyed:
  - object distance $s_\text{o}$ is:
    - $+$ positive for real object (today's use)
    - $-$ negative for virtual object
  - image distance $s_\text{i}$ is:
    - $+$ positive for real image (i.e. if the image is on the side opposite the object, today's use)
    - $-$ negative for virtual image (i.e. if on the same side as the object)
  - focal length $f$ is:
    - $+$ positive for a converging lens
    - $-$ negative for a diverging lens

<!---
  - $R$ is positive for a surface convex toward the object, and negative for a surface concave toward object.


, sign conventions, definitions of object/image distances and focal lengths of converging and diverging lenses. 

--->


#### ○ Image Formation & Magnification

We can use ray tracing to investigate different types of images that can be created by a lens. For today, our converging lens will form a **real image**, such as when a movie projector casts an image onto a screen. In other cases (not explored today), the image is a virtual image, which cannot be projected onto a screen. Using ray tracing for thin lenses, we can illustrate how they form images and develop equations from that to analyze properties of thin lenses.

In {numref}`fig_optics_04_magnification`, we again have three rays from the object (tip of the red-arrow) that enter the lens, are refracted, and intersect at a single point on the opposite side of the lens. The image (tip of the arrow) is located at this point. Several important distances appear in the figure. We see $s_\text{o}$ as object distance, $s_\text{i}$ as image distance, $h_\text{o}$ and $h_\text{i}$ as the heights of the object and images respectively. Images that appear upright relative to the object have *positive* heights, and those that are inverted have *negative* heights.


```{figure} OpticsFigures/Figure_04_ThinLensRayTracingMagnification_v02.png
:width: auto
:name: fig_optics_04_magnification

For magnification, the height of the object and the height of the image are indicated by $h_o$ and $h_i$, respectively. Ray tracing is used to locate the image formed by a lens. Rays originating from the same point on the object are traced, each following one of the rules for ray tracing, so that their paths are easy to determine. The image is located at the point where the rays cross. In this case, a real image (projectable onto a screen) is formed and is inverted. Assuming scale is accurate, magnification is negative and $|m| \lt 1$ as image is smaller than object.
```

The linear **magnification**, $m$, produced by a lens is defined as the ratio of the height of the image, $h_\text{image}$, to the height of the object, $h_\text{object}$ and is dimensionless. If $m$ is positive, the image is upright, and if $m$ is negative, the image is inverted. If $|m| \gt 1$, the image is *larger* than the object, and if $|m| \lt 1$, the image is smaller than the object. With this definition of magnification, and through geometrical analysis not shown here, we can also find the following relation between the vertical and horizontal object and image distances: 


```{math}
:label: eq-magnification
m=\frac{h_\text{image}}{h_\text{object}}=-\frac{s_\text{image}}{s_\text{object}}
```



The minus sign accounts for the orientation of the image (upright or inverted with respect to the object) and the sign convention of the object and image distances.
Another result of the thin lens approximation is the result shown in {eq}`eq-W2Beq2` which relates the effective focal length $f$ of the combination of two thin lenses in very close proximity (perhaps in contact). The focal lengths of the individual lenses are $f_{1}$ and $f_{2}$.

```{math}
:label: eq-W2Beq2
\frac{1}{f}=\frac{1}{f_{1}}+\frac{1}{f_{2}}
```

Expanding beyond the scope of today's lab: since diverging lenses cannot form real images, the imaging of a distant object as a method of measuring the focal length is not possible. However {eq}`eq-W2Beq2` can be used to approximate the focal length of a diverging lens by measuring the effective focal length of a known converging lens and the unknown diverging lens. Notice, the converging power of the positive lens (measured by the reciprocal of the focal length) must be greater in absolute value than the strength of the diverging lens since the effective focal length would need to be positive. This measurement of the strength of the lens by the reciprocal of the focal length is the dioptic power of the lens, measured in $\text{m}^{-1}$.



### ● Lens Effects

There are two common lens effects or aberrations (sometimes treated as a defect in high quality camera lenses or optics systems) of the simple lens we will investigate today.

#### ○ Chromatic Aberration (Part II)

The first common lens effect, chromatic aberration, results from the wavelength dependence of the index of refraction of the glass from which the lens is made. The change in index of refraction results in a focal length dependence on the wavelength, or color, of the light. This dependence is illustrated by the different angles by which red, green, and blue light bends in the ray diagram in {numref}`fig_optics_06_chromaticAberration`-center. Images formed from white light illumination of an object will produce colored images, each one formed at a slightly different image distance. If such an image were produced on a screen or a piece of film, you see an image whose edges were multicolored lines ({numref}`fig_optics_06_chromaticAberration`-left). We see that red light bends or scatters less than the blue light, so we find the focal length of the red light is longer than that of the blue light. This effect must be corrected in most optical instruments designed to be used with white light. Binoculars, for example, can become totally useless without correcting for this chromatic aberration. A ray diagram showing a lens without chromatic aberration is illustrated in {numref}`fig_optics_06_chromaticAberration`-right; notice how all three colors' rays intersect at the same focal point.



```{figure} OpticsFigures/Figure_06_chromaticAberration_v05.png
:width: auto
:name: fig_optics_06_chromaticAberration

Left) Example of today's experimental image on the screen impacted by chromatic aberration. Notice how the image further from center (top of the line) is bluer, while the image closer to center (bottom of line) is redder. Center) Wavelength-dependent (red, green, blue) light rays through lens with chromatic aberration and different focal points (and thus focal lengths) depending on wavelength. Right) Wavelength-dependent (red, green, blue) light rays through lens without chromatic aberration and a single focal point (and thus focal length) independent of wavelength.
```


#### ○ Spherical Aberration (Part III)

The second lens effect, spherical aberration, results from the spherical shape of the lens surfaces. The result is that rays near the edge of a lens are refracted or bent more than those near the principal axis. The effective focal length of the outer rays is then smaller than the focal length of the rays closer to the center of the lens ({numref}`fig_optics_07_sphericalAberration`-center). This so-called spherical aberration causes a large diameter beam to focus over a range of focal lengths; the edges of images can become be somewhat fuzzy as compared to when the center of the image is in focus (e.g. {numref}`fig_optics_07_sphericalAberration`-left). By combining multiple lenses or non-spherical, correcting, and higher quality lenses, this effect can be corrected to bring the whole image back into focus ({numref}`fig_optics_07_sphericalAberration`-right).

```{figure} OpticsFigures/Figure_07_sphericalAberration_v03.png
:width: auto
:name: fig_optics_07_sphericalAberration

Left) Image impacted by spherical aberration. Notice how image center is crisp and in focus while edges are blurry. Center) Light rays through lens with spherical aberration and different focal points (and thus focal lengths) depending on distance from optical axis. Right) Light rays through lens without spherical aberration and a single focal point (and thus focal length) across the whole lens.
```

#### ○ Aberration Experiments

Today's lab will examine both the chromatic and spherical aberrations of a simple, converging lens. The chromatic aberration will be investigated by using color filters to permit the focal length measurement for specific colors (red and blue). For the spherical aberration, the focal length will be determined by measuring the focal length of the lens when only certain rays are allowed through the lens. In one case, an outer-annulus (donut-shaped) light-blocking mask will allow only light rays through a central-aperture near the center of the lens. The second case will then have an inner-disk mask placed over the center of the lens that will allow only light rays through the edge-ring near the outer edge of the lens.




### ● Equipment

<!---
The following equipment is shown in {numref}`fig_optics_022_setup_equip`.
- 1.2 m black optics track to mount everything with built-in ruler
- Light box with illuminated **object** on it (position along track ruler noted by indented metal aligned with the ruler on the optics track) with power brick
- Convex lens in lens holder (position of the lens in the holder is noted by a small plastic protrusion on the side of the holder to be lined up with the ruler on the optics track, basically centered in the holder)
- White viewing screen for displaying **image**
- Red and blue filter --- attaches to light box (not shown)
- Outer-annulus (donut-shaped) and inner-disk light-blocking masks ({numref}`fig_optics_023_setup_equip`) --- attaches to lens holder
- Additional rulers as needed (see table at front of room)
--->

The following equipment is shown in {numref}`fig_optics_00_setup_equip` and {numref}`fig_optics_022_setup_equip`.

```{table} Equipment
:name: optics-equipment-table

| Category | Items |
|---|---|
| **Optical Track System** | • 1.2 m black optics track with built-in ruler for positioning all components |
| **Object Source** | • Light box with illuminated **object** mounted on track<br>• Position indicated by indented metal edge aligned with track ruler<br>• Includes power brick; plugs into bracket axle that holds light box |
| **Lens System** | • Convex lens in lens holder<br>• Lens position marked by small plastic protrusion on holder (align with track ruler; lens centered in holder) |
| **Image Screen** | • White viewing screen for displaying **image** |
| **Filters** | • Red and blue filters (attach to light box; {numref}`fig_optics_024_setup_equip`) |
| **Aperture Masks** | • Outer-annulus (donut-shaped) mask ({numref}`fig_optics_023_setup_equip`-E)<br>• Inner-disk light-blocking mask ({numref}`fig_optics_023_setup_equip`-F)<br>• Both attach to lens holder |
| **Measurement Tools** | • Additional rulers as needed (see table at front of room) |
```

```{figure} OpticsFigures/Figure_22_experimentalSetup_v02.png
:width: auto
:name: fig_optics_022_setup_equip

A) Light box and lens mounted on optics track. B) Object on the light box. C) Refracted image through the lens on the white screen. D) Lightpath through lens onto the white screen.
```

```{figure} OpticsFigures/Figure_24_colorFilters_v02smaller.png
:width: auto
:name: fig_optics_024_setup_equip

Left) Red and blue filters. Right) Filters taped over illuminated object on light box.
```



```{figure} OpticsFigures/Figure_23_experimentalSetup_v01.png
:width: auto
:name: fig_optics_023_setup_equip

E) Outer-annulus mask to allow light only through center of lens. F) Inner-disk mask to allow light only through edges of lens.
```


<!---
## Experimental Procedure – Part III – Geometric Optics & Single Element Imaging
--->

## Experimental Procedure

### ● Preview

```{admonition} PROCEDURE OVERVIEW
:class: note
Investigate light refraction and geometric optics by measuring object (object-to-lens) and image (lens-to-image) distances to determine focal lengths and magnification. Do so with:
  - Part I: Unfiltered light for a range of object distances
    - Object distances $s_\text{object} = \infty, 11, 13, 25, 40, 55, 70, 85\,\text{cm}$
  - Part II: Chromatic aberration (color filters)
    - Red filter
    - Blue filter
  - Part III: Spherical aberration (lens shape)
    - Edge-ring of light rays passing through edge of lens using an inner-disk light-blocking mask
    - Central-aperture of light rays passing through center of lens using outer-annulus light-blocking mask
  - For each of the 12 cases today (summarized in {numref}`optics-cases-table`), the object and image distances are determined, and the focal length determined via {eq}`eq-W2Beq1`. The linear magnification from {eq}`eq-magnification` will be determined by both measuring the image and object heights and comparing that ratio to the ratio of the image amd object distances.
```

<!---
    by determining focal lengths with image and object distances.
- In today's lab, you will complete three experiments:
  - Determine focal lengths of the lens first unfiltered at various distances, then chromatic filtering through red and blue filters, then spherical aberration near center and edge of the lens; consider the physical reasoning for longer or shorter focal lengths depending on differences in the filtering or refracting of the light source. Plot image vs. object distance pairs for the unfiltered distances and investigate the convergence point; compare that value to your average of focal lengths from the unfiltered portion of this experiment.

--->

```{table} Experimental Cases
:name: optics-cases-table

| Part | Case | Object Distance<br>$s_\text{object}$ (cm) | Filter / Mask | Notes |
|---|---|---|---|---|
| I.1 | 1 | $\infty$ | None | Unfiltered light |
| I.2 | 2 | 11 | None | Unfiltered light |
| I.2 | 3 | 13 | None | Unfiltered light |
| I.2 | 4 | 25 | None | Unfiltered light |
| I.2 | 5 | 40 | None | Unfiltered light |
| I.2 | 6 | 55 | None | Unfiltered light |
| I.2 | 7 | 70 | None | Unfiltered light |
| I.2 | 8 | 85 | None | Unfiltered light |
| II | 9 | 13 | Red filter | Chromatic aberration |
| II | 10 | 13 | Blue filter | Chromatic aberration |
| III | 11 | 13 | Inner-disk mask | Edge rays only (spherical aberration) |
| III | 12 | 13 | Outer-annulus mask | Central rays only (spherical aberration) |
```

### ● Part I: Unfiltered, Varied Object Distances

#### ○ Part I: Preliminary Setup

1. Create a common data table including the expected focal length as written on the lens holder, object position on the optics track, object position uncertainty on the optics track, object height and its uncertainty. 

2. Record the expected focal length. Prepare the light box on the optics track similar to {numref}`fig_optics_00_setup_equip`. The illuminated object position is set by placing the notch on the light box bracket to 0.0 cm on the optics track. Record this as the object position and estimate its uncertainty; this will be used for all trials today except the first for a distant object.

3. Notice the horizontal arrow on the object has a mm-scale ruler ({numref}`fig_optics_022_setup_equip`-B). Using the outer circle as the object, determine and record its height $h_\text{object}$ (or width, just be consistent for comparative height measurements later) and estimate its uncertainty $\delta h_\text{object}$. Use a ruler as necessary to confirm size.

#### ○ Part I.1: Distant Object

4. **Case 1:** Using a distant object that you can assume to be effectively at 'infinity', use the lens (in lens holder) to focus the object's image onto the white screen and determine the len's focal length. A distant object might be the sun, a tree outside the laboratory window, the windows on the other end of the atrium, or at worst a light as distant as possible in the laboratory.
    - Take the lens and screen from the optics track, go find your distant object.
    - Estimate the object distance $s_\text{object}$, especially if it is not a very distance object. 
    - Measure and record the image distance $s_\text{image}$, and estimate its uncertainty ($\delta s_\text{image}$) as accurately as possible. 
    - Calculate the len's focal length $f$ using {eq}`eq-W2Beq1`.
    - Calculate the uncertainty $\delta f$ by maximizing and taking the difference (e.g. $\delta f = 1/(1/(s_\text{image} + \delta s_\text{image})) - f$).
    - Compare your experimental $f \pm \delta f$ to the expected focal length on the lens holder by calculating the difference between the two (**not** percent difference, just actual magnitude of the difference).


#### ○ Part I.2: Objects at Finite Distances

5. **Cases 2 -- 8:** Create a data table for finding focal lengths and magnification with columns for (but not limited to):
    - lens position and its uncertainty
    - image position minimum and maximum
    - image position and its uncertainty
    - object distance and its uncertainty
    - image distance and its uncertainty
    - focal length and its uncertainty
    - difference between experimental and expected focal lengths
    - image height minimum and maximum
    - image height and its uncertainty
    - magnification and its uncetainty as calculated from image & object heights
    - magnification and its uncertainty as calculated from image & objects distances
<!---
    - lens position
    - lens poisiton uncertainty
    - image position minimum and maximum
    - image position
    - image position uncertainty
    - object distance
    - object distance uncertainty
    - image distance
    - image distance uncertainty
    - focal length
    - focal length uncertainty
    - difference between experimental and expected
    - object height
    - object height uncertainty
    - image height minimum
    - image height maximum
    - image height
    - image height uncertainty
    - magnification calculated from heights
    - magnification from heights uncertainty
    - magnification calculated from distances
    - magnification from distances uncertainty
--->


6. On the optical bench, used for this and all succeeding steps, construct the setup to be similar to {numref}`fig_optics_00_setup_equip` with the lens and screen back on the optics track. 

7. Starting with case 2 in {numref}`optics-cases-table`, place the lens at the stated distance from the object (if object is at 0.0 cm, then lens position is same as object distance). Record the lens position and estimate its uncertainty.

8. Move the screen to a position that produces the sharpest possible image. Determine the image position and its uncertainty by:
    - shifting the screen closer to the lens until you are no longer confident the image is in focus. Record the minimum image position.
      - before moving the screen away from this position, use a ruler to measure and record the minimum image height.
    - shifting the screen further away from the lens until you are again no longer confident the image is in focus. Record the maximum image position.
      - before moving the screen away from this position, use a ruler to measure and record the maximum image height.

9. Determine the object distance $s_\text{object}$ (from illuminated object to lens) as the difference between the lens and object positions. Also determine the object distance uncertainty $\delta s_\text{object}$ as the sum of these two position's uncertainties (why does it make sense to add these; what is the largest range?).

10. Similarly determine the image distance $s_\text{image}$ (from lens to image on screen) as the difference between the image and lens positions. Also determine the image distance uncertainty $\delta s_\text{image}$ as the sum these two positions' uncertainties. 

11. Calculate the focal length $f$ using {eq}`eq-W2Beq1` and its uncertainty $\delta f$ by maximizing and taking the difference (e.g. $\delta f = 1/(1/(s_\text{object} + \delta s_\text{object}) + 1/(s_\text{image} + \delta s_\text{image})) - f$).

12. Compare your experimental $f \pm \delta f$ to the expected focal length on the lens holder by calculating the difference between the two (**not** percent difference, just actual magnitude of the difference). Is it also consistent with the focal length measured with a distant object?

13. Using the min and max image heights (based on the min and max image positioning), determine the image height and its uncertainty by:
    - $h_\text{image} = (h_\text{image,max} + h_\text{image,min}) / 2$
    - $\delta h_\text{image} = (h_\text{image,max} - h_\text{image,min}) / 2$
    - IF $\delta h_\text{image}$ as calculated above is less than the precision of your measurement tool (likely a ruler), treat $\delta h_\text{image} = \text{precision}$

14. Using **image and object heights**, calculate the image magnification $m$ with {eq}`eq-magnification` (left side of equation). Also calculate the uncertainty $\delta m$ by maximizing and taking the difference (e.g. $\delta m = ((h_\text{image} + \delta h_\text{image}) / (h_\text{object} - \delta h_\text{object})) - m$).

15. Using **image and object distances**, similarly calculate the image magnification $m$ with {eq}`eq-magnification` (right side of equation). Also calculate the uncertainty $\delta m$ by maximizing and taking the difference (e.g. $\delta m = (-(s_\text{image} + \delta s_\text{image}) / (s_\text{object} - \delta s_\text{object})) - m$). Do the two magnification methods agree; if not, why?


<!--- 
4. Only for non-filtered cases, measure the length of one of the arrows or circles on the object and measure the length of the same arrow or circle on the image and record them as $h_\text{object}$ and $h_\text{image}$ respectively. Calculate the resulting magnification with {eq}`eq-magnification`. 
5. Create a data table with columns for object distance, image distance, and focal length from {eq}`eq-W2Beq1`. Include rows for the red filter, the blue filter, the disk and the annulus. The lenses have only a little chromatic aberration and spherical aberration, so you will need to be careful locating the screen at the best focus.

--->

16. Repeat steps 7 -- 15 for the rest of the unfiltered cases ({numref}`optics-cases-table`).

17. Determine the average focal length and average of the uncertainties. Do all unfiltered cases agree? Any that do not?


18. ***PLOT*** Object vs. Image distances:
    - Construct a graph where one axis is the object distances and the other is their related image distances. 
    - It is suggested to do this by hand; graph paper is available at front of room. Mini example at bottom of {numref}`optics_whiteboard_01`.
    - For each of Case 2 -- 8, plot the object distance on the object axis, its the image distance on the image axis. Connect the two points with a straight line. 
    - In the ideal case, all of the lines should intersect at the point $(f,f)$. Visually estimate the point $(s_\text{object,plot},s_\text{image,plot})$ closest to the intersections, estimate the focal length by $f=(s_\text{object,plot}+s_\text{image,plot})/2$. Then, draw a circle around the intersection, and use its radius to estimate $\delta f$. Compare this determination to your average $f$ from cases 2 -- 8.

<!---
18. ***PLOT*** Object vs. Image distances:
 Set up a series of object and image distances and record the data points.  Since the object and image can always be interchanged, each measurement of an object-image distance pair represents two data trials.
    - Construct a graph where one axis is the object distances and the other is their related image distances.
    - For each of Case 2 -- 8, plot the object distance on the object axis, its the image distance on the image axis. Connect the two points with a straight line. 
Repeat this process for each of your object-image data trials.
In the ideal case, all of the lines should intersect at the point $(f,f)$. Visually estimate the point $(s_\text{object},s_\text{image})$ closest to the intersections and estimate the focal length by $f=(s_\text{object}+s_\text{image})/2$. Compare this determination of the focal length with the values from steps 8, 1 and 3.
 --->



### ● Part II: Chromatic Aberration

<!---
6. Repeat step 3 using first the red and then the blue filter in front of the object. While leaving the lens fixed at an $s_\text{object} = 13\,\text{cm}$, move the screen to produce the best focused image. Carefully record only the object and image distances and determine the 'red focal length' and the 'blue focal length.'
--->

19. Repeat steps 7 -- 15 for Cases 9 and 10 with the lens placed at a 13 cm object distance $(s_\text{object} = 13\,\text{cm}).$ Use the two color filters, red and blue, to determine the focal lengths and magnification of red and blue light. 
    - Case 9: Hang/tape the red filter directly in front of the light-box object so all light used to form the image is red. Move the screen until the image is focused. Carefully measure the object and image distances and uncertainties, and calculate the focal length and magnifications and their uncertainties.
    - Case 10: Same thing, but now blue.
    - Compare both, is one $f$ longer than the other? Physically, why might you expect that? What about $m$?




### ● Part III: Spherical Aberration


20. Repeat steps 7 -- 15 for Cases 11 and 12 with the lens still placed at a 13 cm object distance $(s_\text{object} = 13\,\text{cm})$. Use the two light-blocking masks, inner-disk and outer-annulus, to determine the focal lengths and magnification of the edge-ring and central-aperture light rays.
    - Case 11: Center the inner-disk mask in front of the lens so only rays near the outer edge of the disk are being used to form the image. Move the screen until the image is focused. Carefully measure the object and image distances and uncertainties, and calculate the focal length and magnifications and their uncertainties.
    - Case 11: Same thing, but with outer-annulus mask allowing only rays near the center of the lens to form the image.
    - Compare both, is one $f$ longer than the other? Physically, why might you expect that? What about $m$?



## Post-Lab Submission --- Interpretation of Results

### ● Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
  - Please include concise summary table.
  - Please include plot:
    - One plot, ***preferrably hand-drawn***, with all non-$\infty$, object distances paired with respective image distances from Part I (unfiltered Cases 2 -- 8).



### ● Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be both qualitative and quantitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting precision) errors?
  - What are your measurement uncertainties, and, based on these uncertainties, how do your final results change? I.e. do your different measurement uncertainties make your final results larger or smaller, by how much?


- In a **paragraph**, summarize the results you have determined for all cases. Consider:
  - What was the point of today's lab; what did we aim to discover?
  - How do your focal lengths from each set compare? Do they agree based on your uncertainties? Are there any outliers, why/why not?
    - Object distance of distant object ($\infty$) vs. 13 cm case?
    - Object distance: All non-$\infty$ unfiltered cases?
    - Object distance of 13 cm for unfiltered vs. red vs. blue vs. disk vs. annulus?
  - For chromatic aberration (Part II): physically, why should the focal length from the red or blue filter be shorter or longer?
  - For spherical aberration (Part III): Physically, why does the disk or annulus filtered light produce a shorter or longer focal length?
  - For your plot of image vs. object distances, where do the lines from each object/image pair converge?
    - Does that plot-derived value $\pm$ your estimated uncertainty from the plot agree with your average value for unfiltered focal lengths (Part I)?
    - On the plot, why do the lines converge?
  - With regards to magnification:
    - How does the image height relate to object distance? 
    - Did your magnification values from height measurements agree with those expected from object & image distances? How does magnification relate to object and image distances?




<!---
## Post-Lab Submission — Interpretation of Results

- Make sure to submit your finalized data sheet with summarized data and cleaned-up plots (Excel sheet)

- Paragraph of your results +/- uncertainties from your data. Make sure to include discussion of the following:
  - **For Diffraction:** Does your value for laser wavelength agree with the accepted value for a HeNe laser ($\lambda_{\mbox{HeNe}}=632.8$ nm)?
  - Does your value for CD track spacing (of the spiral of data pits) agree with the accepted value of CD track spacings ($\sim1.6\times 10^{-6}$ m)?
  - How does the diffraction pattern spacing depend on the laser's wavelength and the diffraction grating spacing?
  - **For Optics:** How do your focal lengths from each set compare (distant object vs. 13 cm, red vs. blue, disk vs. annulus?
  - Do they agree based on your uncertainties?
  - Physically, why is the focal length from the red or blue filter shorter or longer; what would cause that?
  - Physically, why does the disk or annulus filtered light produce a shorter or longer focal length; what would cause that?
  - For your plot of image vs. object distances, where do the lines from each object/image pair converge; does that value ± your estimated uncertainty from the plot agree with your average value for focal lengths for the variety of image/object distances?
  - On the plot, why do the lines converge?

- Paragraph of your errors and estimated measurement uncertainties. Be quantitative. Make sure to include discussion of the following:
  - Where might systematic (affecting accuracy) and/or random (affecting precision) errors be coming from?
  - What are your measured uncertainties, and, based on these uncertainties, how do your final results change? I.e. do your different measurement and slope uncertainties make your final results larger or smaller?
  - Change different variables by your best estimation of measurement uncertainties in your Excel sheet; what variables affect the accuracy of your final results the most?
  - If larger or small, are they more or less accurate to expected values?
  - How could you improve your random errors?
  - Were your systematic errors significant; how could this be improved if you were to re-run this experiment?

- Reflect on this week's lab; what did you learn?
--->



## The Whiteboard

```{figure} OpticsFigures/optics_2025_Spring_01_v03.jpg
:name: optics_whiteboard_01
:width: auto
:align: center

Overview. ---- NOTE: Order of parts have changed, but on the whole, this is what you're doing.
```


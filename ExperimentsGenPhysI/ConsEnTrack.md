(cons-energy-glider-track-lab-overall)=
# Conservation of Energy with Glider on Tilted Air Track

## Background

**Energy cannot be created nor destroyed.** All that can really happen is a change in its form. We shall consider the conservation of mechanical energy, in particular, the sum of the kinetic energy and potential energy of a mass. The kinetic energy is due to the motion of the mass and the potential energy is due to the relative position of the mass in the earth's gravitational field. This total mechanical energy can only change if nonconservative forces are acting on any part of the system. We will examine the exchange of kinetic and potential energy and the conservation of mechanical energy under the presumption of no nonconservative forces acting. If the mechanical energy is not conserved we will attempt to determine potential sources of nonconservative work being done that would change the mechanical energy.

The **work** done by a force acting on a mass is the magnitude of the force acting in the direction of motion times the distance the mass moves. Work is only done when the mass moves. (In other words, you can push as hard as you like on a brick wall, but if the wall doesn't move, you didn't do any work!) Assume for the moment that we have a mass $m$ moving on a frictionless, horizontal surface. Assume a force acts on the mass from the position $x = 0$ to $x = x_1$ as illustrated in {numref}`M05Fig01`. At position $x = 0$ it is moving with a velocity $v_{0}$ and at $x = x_1$ the velocity is $v_1$.

```{figure} ConsEnTrackFigures/Figure01.jpg
:name: M05Fig01
:width: 500px
:align: center

Explanation of the variables needed to calculate the amount of work done on a mass
```

The work done by the force is $W_F = \vec{F} \cdot \vec{x_1}$. Using Newton's second law it can easily be shown that the work done by the force changes a quantity we call the *kinetic energy*, $K = \frac{1}{2} m v^2$. Using the example illustrated in {numref}`M05Fig01`,

```{math}
\vec{F} \cdot (\vec{x}_1 - \vec{0}) = \frac{1}{2} m v_1^2 - \frac{1}{2} m v_0^2
```

In this case, the force is acting in the direction of the motion and thereby increases the kinetic energy. If the force were acting in the direction opposite to the motion, then the kinetic energy would be decreased. If friction were present, it would act in the direction opposite to the direction of motion and thereby reduce the kinetic energy. In this simple analysis, we have made no assumption as to the nature of the force.

A force like friction is a non-conservative force. The work done by it not only depends upon the path the mass takes but is also not completely recoverable. However, the work done on a mass by a conservative force can be completely returned to the mass as mechanical energy. Thus work done by a conservative force can be represented by a potential energy function and depends only on the end points of the process. The gravitational force is a conservative force and is assumed constant in the vicinity of the surface of the earth. The potential energy function is merely the work done by gravity on the way up or the way down and is equal to the gravitational force (the weight $m g$) times the change in height, $h$. The gravitational potential energy, $U$, is given by

```{math}
U = m g h
```

The work done by this conservative force, like all conservative forces, only depends on the end-points of the path. The gravitational potential energy is a relative quantity, i.e., it is a change in energy because of a change in elevation. Thus we can choose a zero level arbitrarily.

If there are no non-conservative forces acting, then a mass moving only under the influence of gravity merely exchanges its kinetic and potential energy while the total energy remains constant. For a mass stationary at some height, $h$, above the ground, all of its energy is potential energy of value $mgh$ with respect to the ground. As the mass begins to fall under the influence of gravity, it loses $U$ and gains $K$. When it reaches the ground, the $U$ is zero with respect to the ground and the $K$ is a maximum, equal to the original $U$ at the top. If the mass were a roller coaster, the coaster could climb back up to its original height where all the energy would be $U$ at which point it would momentarily stop, i.e., no $K$. This assumes that neither friction nor any other nonconservative force is acting. In general, we have

```{math}
W_{N.C.} = \Delta K + \Delta U
```

where $W_{N.C.}$ is the work done by non-conservative forces. If there are no non-conservative forces acting, then

```{math}
:label: eq:total-energy
\Delta K + \Delta U = 0
```

In this experiment, we will use an air track to provide a nearly frictionless surface. The track will be tilted at a measurable angle. A glider will be released from rest at the top of the track and allowed to slide down and collide with a spring at the bottom. If the force of the spring on the glider is conservative, then the kinetic energy of the glider at the bottom is converted to potential energy in the compressed spring. This potential energy is given back to the glider in the form of kinetic energy as the spring expands. The glider bounces off and goes back up the track to its original height where the energy is again all $U$. If no energy is lost in the collision at the bottom, we say that the collision is completely elastic, implying that the forces involved in the collision are conservative. After the collision, the glider will rebound up the track. Getting back to its original height therefore implies no mechanical energy is lost during the entire path. If it does not, we have to look for an energy loss mechanism and some non-conservative forces acting.

The change in height from the top to the bottom is measured allowing the change in $U$ to be calculated. We will set the zero level for the potential energy at the bottom of track, at the position, $s_0$, in {numref}`M05Fig02`.

A measurement of the transit time from the top to the bottom will allow the calculation of the velocity at the bottom and therefore the $K$ at the bottom. Finally, measuring the maximum height achieved on the rebound will yield a second value of $U$.

The $K$ at the bottom of the track can be determined by measuring the average velocity from the release point at the top, $s_1$, to the collision point at the bottom, $s_0$, and then using {eq}`eq:total-energy`. From a measurement of the transit time from $s_1$ to $s_0$, the velocity of the glider at the moment of collision at the bottom, $v_b$, can be determined by using the definition of average velocity, $v_{\text{avg}}$, thus:

```{math}
\frac{\Delta s}{\Delta t}  = v_{\text{avg}} = \frac{1}{2} (v_{b}+v_1)
```

where the initial velocity, $v_1 = 0$, $\Delta s$ is the distance traveled down the track, and $\Delta t$ is the transit time of travel.

Rearranging terms we have the velocity at the bottom in terms of measurable quantities

```{math}
:label: eq:velocity-bottom
v_b = 2 v_{\text{avg}} = 2 \left(\frac{\Delta s}{\Delta t}\right)
```

Using the definition of $K$, the $K$ at the bottom is then

```{math}
:label: eq:kinetic-bottom
K_b = \frac{1}{2} m v_b^2
```

In order to calculate the potential energy, $U$ at any point, along the track we must determine the change in height between $s_1$ and $s_0$. The potential energy at any position along the track is measured with respect to the collision point at the bottom, $s_0$, which is arbitrarily assigned a value of zero potential energy. The $U$ is given by the weight of the glider, $mg$, times the change in vertical height.

{numref}`M05Fig02` is a simplified diagram of the inclined track. The distance $s$ is measured along the track by the scale attached to the side of the track. The change in elevation, $\Delta h$, of any other point $s$ along the track can now be determined from the distance $s$ and the incline angle of track, $\theta$. The incline of the track is produced by placing a spacer of known height under a leg at one end. With the height of the spacer and the distance between the legs, $D$, the angle can be calculated (See {numref}`M05Fig03`).

```{figure} ConsEnTrackFigures/Figure01_v2025-01.png
:name: M05Fig02
:width: 450px
:align: center

Schematic Drawing explaining the relationship between the track elevation $\Delta h$ and the distance $\Delta s$ for the Conservation of Energy experiment.
```

At $s_0$, $U_{b} = 0$, therefore $U_{s} = mg\, \Delta h = mg\, \Delta s \sin(\theta)$.
Referring to {numref}`M05Fig03`, the $\tan(\theta) = \text{(height of the spacer)} / \text{(distance between legs)}$ or

```{math}
\tan(\theta) = \frac{H}{D}
```

With the very small angles of incline being used, we can safely assume that

```{math}
\tan(\theta) \sim \sin(\theta)
```

therefore the potential energy, $U$, at some position, $s$, along the track is finally given by measurable quantities as

```{math}
:label: eq:potential-energy
U_s = mg \, \Delta s \frac{H}{D}
```

## Experimental Procedure

<iframe width="560" height="315" src="https://www.youtube.com/embed/CINQAbvNFPw?si=srqk4862Gp_MHdzu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

```{figure} ConsEnTrackFigures/Figure02_v2025-02.png
:name: M05Fig03
:width: 90%
:align: center

Experimental setup for the Conservation of Energy experiment.
```

- Turn on the air and allow it to run a couple of minutes before proceeding. It is very important that the track is clean and free of dirt. This will prevent any damage to the very expensive air track and will keep friction to an absolute minimum. Do not put a glider on the track without air flowing.

- Measure and record the mass of both a large and a small glider.

- Without the spacer present and the air track resting directly on the tabletop, place one of the gliders on the track and note any preferential drift of the glider. Adjust the height of the single leg until the air track is level, as indicated by no preferential drift. Check both orientations of the glider on the track to check if the car is asymmetric and has a significant preferential drift on an otherwise level track. If this occurs, use another glider.

- Measure and record the distance $D$. This is the center-to-center distance between the legs.

- Measure and record the heights $H$, of each of the two spacers. Use a Vernier caliper for maximum accuracy. See the instructions at Fig. VernierFig02 for using the Vernier caliper.

- Four cases will be performed, two gliders for two spacers. Determine a convenient point on the glider to use with the scale attached on the side of track. It doesn't matter what point you choose, only that you use the same point for all $s$ determinations for that glider. A convenient point is the lower front or rear corner of the glider since it will be very close to the scale.

- For each case, perform the following steps and record the data appropriately in your spreadsheet:

  1. Raise the single leg side of the track by placing a spacer under the knob.

  2. Place the glider at the bottom of the track resting against the bumper. Record $s_0$. (Note: With the car at this position, the red light on the bottom photogate should be lit. Moving the glider to the right the slightest distance should put the light out. If this is not the case, adjust the position of the photogate.)

  3. Next, place the glider near the top of the track. Move it slowly as you approach the top photogate. Stop the glider at the exact location when the red light comes on. Record $s_1$.

  4. Before you take the recorded data in the next step, take some practice runs. Your subsequent data will be much improved by your training!

     - Position the glider so it is blocking the top photogate and the red light is on. Place one finger on the track in front of the glider and gently push the glider to the right until the red light on the photogate just goes out.

     - Press record in **Capstone** to start the timer. *NOTE:* **Capstone** may take a few seconds to start displaying times, once it's going, it will display the time whenever a photogate beam is broken; the time at the higher (start) photogate $t_1$ as well as the time at the lower (end) photogate $t_0$. Total transit time $\Delta t$ will be the difference of the start and end times.

     - Release the glider by quickly pulling your finger away from the track. After the glider bounces off the lower bumper, you can calculate the time of travel from top to bottom $\Delta t$.

  5. For each of the five trials, release the glider from the $s_1$ point and measure and record the following:

     - The transit time $\Delta t$ from release at the top to the collision at the bottom. Release the glider very carefully to insure that the initial velocity is zero.

     - Allowing the glider to rebound off the bumper, record the rebound position $s_2$. As the glider slows to a stop, capture the glider by gently pressing your finger near a lower corner of the glider just as it comes to a stop and then read $s_2$ off the scale. Use the same point on the glider to read $s_2$ that you used to read $s_1$ and $s_0$.

**Data Table:**

- Create a table of the common data including the masses of the gliders, the distance $D$ between the legs of the air track and the heights of the two spacers.

- Create a table for each case with rows for each of the five trials including:

  - The starting point $s_1$ at the top
  - The stopping point $s_0$ at the bottom
  - Start time at the top $t_1$
  - End time at the bottom $t_0$
  - The time $\Delta t$ (s) for each of the five trials
  - The rebound position $s_2$ at the top
  - Initial distance, $\Delta s_1=s_1-s_0$
  - Initial potential energy at top, $U_{\text{top}}$
  - The speed at the bottom, $v_{\text{b}}$
  - Kinetic energy at the bottom, $K_{\text{b}}$
  - Final distance, $\Delta s_2=s_2-s_0$
  - Final potential energy at the rebound position, $U_{\text{rebound}}$

- Create a summary table of the analysis with a row for each case including the following data:

  - The average and standard deviation of the time, $\Delta t$, for the five trials
  - The average and standard deviation of the speed at the bottom, $v_{\text{b}}$
  - The average and standard deviation of the kinetic energy at the bottom, $K_{\text{b}}$
  - The average and standard deviation of the final potential energy at the rebound position, $U_{\text{rebound}}$
  - % change from initial potential energy to kinetic energy at the bottom
  - % change from initial potential energy to final potential energy

Calculate the following:

- For each case, calculate the initial potential energy at $s_1$. Average the transit times, $\Delta t$, and calculate the velocity $v_b$ and the $K_b$.

- For each case, average the rebound position, $s_2$. Using this averaged value, calculate the final $U_2$.

- Calculate the percent change in mechanical energy from the top to the bottom.

- Calculate the percent change in mechanical energy from the initial release point $s_1$ to the final rebound point $s_2$.




## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet). 
- In a **paragraph**, summarize the results you have determined in each case. Consider
	- Arguing your responses with your data ± standard deviation:
	    - Is kinetic plus potential energy conserved going from the top to the bottom?
		- Is kinetic plus potential energy conserved between the top and the rebound position?
	- Why is there a difference in energy conservation between the top/bottom and top/bottom/rebound?
- In a **paragraph**, summarize your error analysis. Be qualitative not only quantitative.
	- What is the precision of your equipment?
	- What are the effects of measured uncertainties on your determined energies?
	- What are possible systematic errors for today’s experiments?
	- How could one gain energy between top and bottom?

## The Whiteboard

```{figure} ConsEnTrackFigures/ConsOfEnergyTrack_2024_Fall_01.jpg
:name: consE
:width: 600px
:align: center

```
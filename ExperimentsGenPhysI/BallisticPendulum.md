(ballistic-pendulum-lab-overall)=
# Conservation of Energy & Linear Momentum with Ballistic Pendulum & Projectile Motion

## Background

```{admonition} OVERALL GOALS
:class: note
Use a ballistic pendulum to:
- Determine initial exit velocities of a projectile to investigate and compare two different techniques:
   - Motion explained by conservation of linear momentum and mechanical energy
   - Motion explained by kinematics
```

Two techniques will be employed today.

In the first, a ballistic pendulum, a device designed to capture a projectile in an initially stationary pendulum, will be used.  The conservation principles are used to analyze the collision and the subsequent motion of the pendulum.  The completely inelastic collision associated with the capture of the projectile in the pendulum and the subsequent motion of the pendulum provide the data necessary for the determination of the initial velocity.

In the second technique, the measured parameters of the trajectory of a horizontally launched projectile are used to determine the initial velocity.  With the projectile moving in a free-fall trajectory, constant acceleration kinematics will be used to determine the initial velocity from measurements of the horizontal range and vertical drop.

In each case, the projectile will be launched with the same device allowing a comparison of the initial velocity determinations of the two techniques.

### Ballistic Pendulum Review

The ballistic pendulum is so named because it was originally used to measure the velocity of high-speed projectiles such as bullets long before electric and electronic timers made the procedure unnecessary. It remains, however, as a simple and demonstrative device for understanding the conservation principles of energy and momentum. In analyzing the problem, the system will consist of the projectile and the more massive pendulum (see {numref}`M06Fig03`). 


```{figure} BallisticPendulumFigures/M06_fig03_v2025-01.png
:name: M06Fig03
:width: 100%
:align: center

Left) Ballistic pendulum apparatus showing path of the rotating arm during the pendulum experiment. Right) Arm with metal bob that catches the projectile (metal ball with hole, not shown) when launched from the spring-powered gun of the apparatus.
```




As illustrated in the left image in {numref}`M06Fig01`, before the collision, the projectile is in motion horizontally towards the stationary pendulum. After the collision, the projectile is imbedded in the pendulum and the pendulum is moving along the arc as shown in the right image of {numref}`M06Fig01`.

```{figure} BallisticPendulumFigures/M06_fig01_v2025-02.png
:name: M06Fig01
:width: 100%
:align: center

Ballistic Pendulum before (left) and after the collision (right)
```

The horizontally launched brass ball collides rather violently with and is captured by the more massive bob of the pendulum, initially at rest. The violent collision is totally inelastic as the ball is captured by the pendulum with much of the initial kinetic energy of the ball lost through a variety of energy conversions, mostly heat.

During the collision of the ball with the pendulum, no external forces are acting on the system. Newton's third law demands that the forces of the ball on the pendulum and the pendulum on the ball are equal and opposite. These two, always equal and opposite, internal forces are acting for the same time and therefore produce equal and opposite impulses on the two bodies. Thus the change in momentum of one body is equal and opposite to the change in momentum of the other. If the momentum changes of the two colliding bodies are equal and opposite, then the total linear momentum of the system cannot change and the total momentum is conserved.

Notice that there has been no assumption on the nature of the internal forces acting. They do not have to be elastic, i.e. conservative. As such, the conservation of momentum does not imply anything about the conservation of kinetic energy in the collision. Linear momentum is conserved regardless of the nature of the interaction of the two bodies during the collision. Only when the interactive forces are completely elastic, i.e. conservative, will the kinetic energy of the collision be conserved.

Momentum, like force and velocity, is a vector quantity. The conservation of momentum of a system therefore implies the conservation of the total vector momentum of the system. In our case, the initial momentum of the system is the initial momentum of the brass ball, which is only in the horizontal direction. Therefore the momentum after the collision can only be in the horizontal direction and they must be equal.

Thus we can write

```{math}
:label: eq-M06momentum
m \vec{v}_0 = (m + M) \vec{V},
```

where $m$ is the mass of the ball, $M$ is the mass of the pendulum, and $\vec{V}$ is the velocity of the pendulum and ball together. If we can measure or determine $\vec{V}$, we can determine $\vec{v}_0$. The determination of $\vec{V}$ can be made by examining the motion of the pendulum after the collision.

After the collision, the pendulum swings upward until it momentarily comes to rest at the top of its swing where the vertical height of the system has been increased from $y_1$ to $y_2$ (right image of {numref}`M06Fig01`). We will now make some assumptions. We will assume that there are no friction losses in the motion of the pendulum and that no collisions take place that might otherwise cause a loss of mechanical energy. In other words, we are assuming that the total mechanical energy of the system is conserved after the collision. By equating the kinetic energy of the system just after the collision at the bottom of the swing to the potential energy at the top, we can write

$$\frac{1}{2}(m+M) V^2 = (m+M) g \left(y_2 - y_1\right).$$

Solving this expression for $V$ we have

$$V = \sqrt{2 g \left(y_2 - y_1\right)}.$$

Substituting in {eq}`eq-M06momentum` above, we have finally an expression for the initial velocity of the ball in terms of the measurable change in height of the pendulum and the respective masses, i.e.

```{math}
:label: eq-M06v0
v_0 = \left( \frac{m+M}{m} \right) \sqrt{2 g \left(y_2 - y_1\right)}.
```

### Projectile Motion Review

When a projectile is moving solely under the influence of the force of gravity, we say that the projectile is in free-fall. Consider the launching of the same ball used in the ballistic pendulum. In this case, the pendulum will be swung up out of the way so the flight of the ball will continue off the edge of the table, eventually hitting the floor some distance away. This situation is illustrated in {numref}`M06Fig02`.

```{figure} BallisticPendulumFigures/M06_fig02_v2025-02.png
:name: M06Fig02
:width: 100%
:align: center

Projectile Motion. Note $X$ and $Y$ are broken down into easier-to-measure quantities.
```

Once the ball leaves the spring gun used to launch the ball, the ball is in free-fall. The vertical and horizontal motions are completely independent. We assume that once the ball leaves the gun, there are no energy loss mechanisms during the flight of the ball.

In the vertical direction, the initial velocity is zero and the ball is accelerated downward by its weight, finally hitting the floor some time, $t$, later, dropping a vertical distance of $Y$, measured from the bottom of the ball to the top of the landing pad.
In the horizontal direction, the ball has a constant velocity of $v_0$ during the entire flight over the horizontal distance $X$, measured from the bottom of the ball to the center of the impact mark on the landing pad.

Using our kinematic expressions for constant acceleration motion, we have

$$Y = \frac{1}{2} g t^2$$

and

$$X = v_0 \, t.$$

Eliminating the time $t$ from these two expressions, we obtain

```{math}
:label: eq-M06v0pro
v_0 = X \sqrt{\frac{g}{2 Y}}.
```

## Experimental Procedure

```{admonition} OVERVIEW
:class: note
- Experimentally determine initial exit velocity of the metal ball (projectile) with two different experiments.
- Ballistic Pendulum - Investigate how energy is converted and momentum is conserved:
  - Potential energy at the top and kinetic energy at the bottom.
  - Momentum after the collision and momentum before the collision.
- Projectile Motion - Investigate kinematic motion for comparison.
- Each experiment will have a total of 15 trials:
    - Groups of 2 students, each student will launch the projectile for 7 -- 8 trials.
    - Groups of 3 students, each student will launch the projectile for 5 trials.
```




(demo-video-ballisticPendulum_overall)=
### Demo Video: Ballistic Pendulum & Projectile Motion Experiment

<div style="text-align: center;">
   <iframe width="560" height="315" src="https://www.youtube.com/embed/OjMF7Z2Pe6U?si=j9aSi4RHe3IBDj4R" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  <figcaption>First half covers the measurements necessary for the ballistic pendulum experiment. Second half covers the measurements necessary to the projectile motion experiment. Reminder, the ball will need to be marked up significantly with a dry-erase marker to show impact location on the landing board due to the rifling that can happen -- see high-speed at end of the video.</figcaption>
</div>











### Ballistic Pendulum Procedure

1. **Data table:**
   - Create a table of the common data for the ballistic pendulum experiment including the mass of the ball $m$, the mass of the pendulum $M$, the initial pendulum height $y_1$ and any other common data needed for calculations.
   - Create a table with a row for each trial in the ballistic pendulum part of this lab including the trial number, lab member's initials, the pendulum height $y_2$, the change in height $y_2-y_1$, the calculated velocity of the pendulum $V$, and the calculated initial velocity of the ball $v_0$.
   - Create a table to summarize the experiment including the average pendulum height $y_2$, the average change in height $y_2-y_1$, the average velocity of the pendulum $V$, the average initial velocity of the ball $v_0$, the standard deviation of $v_0$.

2. Measure and record the mass of the brass ball projectile.

3. Record the mass of the pendulum that is ***indicated*** on the apparatus (***DO NOT REMOVE THE ARM***).

4. Practice the following procedure before actually taking data.

5. The pointer on the side of the bob indicates the center of mass of the pendulum. With the pendulum hanging motionless, measure the height of the metal pointer on the pendulum from the base plate as illustrated in {numref}`M06Fig01`. This value is $y_1$. Record the value in meters.

6. Place the brass ball on the pin of the gun, and press the ball so the spring of the gun is compressed until the trigger catches and holds the compressed spring.

7. Fire the gun by squeezing the trigger with ***CONVICTION*** (quickly) to ensure more consistent firings. The ball will be captured by the bob and the pendulum will swing upwards.

8. A small ratchet engaging a rack will capture the maximum upswing position of the pendulum. Measure the height to the tip of the metal pointer on the pendulum as illustrated in {numref}`M06Fig01`.

9. Carefully release the ratchet so the pendulum can swing back to its equilibrium position. **Do not twist or slide the pendulum off the rack, use the little handle on the spring loaded ratchet beneath the brass bob.**

10. Release the ball from the bob of the pendulum by pushing it with your finger, a pencil, or other short cylinder.

11. Fire the ball 15 times with ***CONVICTION*** (quickly), and record the pendulum height $y_2$ for each shot (trial).

12. Calculate the average $y = y_2-y_1$ and the average $v_0$ from {eq}`eq-M06v0`.

13. Record your data and calculations on your spreadsheet.

### Projectile Motion Procedure

1. **Data table:**
   - Create a table of the common data for the projectile motion experiment including the distance to the landing pad $x_1$, the vertical distance $Y = y_1 - y_2$ and any other measurements.
   - Create a table with a row for each of the 15 trials in the projectile motion part of this lab including the trial number, lab member's initials, the inidividually measured $x_2$, the calculated horizontal distance $X=x_1+x_2$, and the calculated initial velocity of the ball $v_0$.
   - Create a table to summarize the experiment including the average and standard deviation of the distance on the landing pad $x_2$, average and standard deviations of the initial velocity $v_0$ of the ball.

2. Set up the projectile motion experiment as shown in {numref}`M06Fig02`.

3. Fire the ball 15 times with ***CONVICTION*** (quickly), and record the measurements of $x_2$. Be careful that the gun is in the same position for each measurement.

4. Calculate the initial exit velocity $v_0$.

5. Calculate the average and standard deviations for the $n=15$ measurements of $x_2$ and $v_0$.

## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet). 
- In a **paragraph**, summarize your error analysis. Be qualitative not only quantitative.
	- What is the precision of your equipment?
   - What are possible random errors for today's experiment?
   - What are possible systematic errors for today’s experiments?
	- What are the effects of your measurement uncertainties on your determined exit velocities for both experiments?
      - Use error propagation to defend your results; look back at {eq}`eq-M06v0` and {eq}`eq-M06v0pro` as needed.
- In a **paragraph**, summarize the results you have determined in each case. Consider:
   - What were your initial (exit) velocity results for both pendulum and projectile experiments? Treat your standard deviations as your uncertainty of their average values.
   - Do the initial velocities from both experiments agree with one another?
      - How and why are they (or could be more) different regarding physical concepts?
   - Considering both experiments and their sources of error, which experimental exit velocity do you trust more? Explain your answer using both physical concepts and your error propagation.
   - Suppose you would have used a more massive marble in the projectile motion portion of the experiment. How would this affect your result? Explain your answer using a physics argument.


   
   



## The Whiteboard

```{figure} BallisticPendulumFigures/ConsEnergyMomentumBallistic_2024_Fall_02.jpg
:name: ballist
:width: 100%
:align: center

```
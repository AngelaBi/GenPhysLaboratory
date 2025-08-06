# Conservation of Energy & Linear Momentum with Ballistic Pendulum & Projectile Motion

## Background

Conservation of energy and linear momentum will be used to measure the initial velocity of a projectile.  Two techniques will be employed.

In the first, a ballistic pendulum, a device designed to capture a projectile in an initially stationary pendulum, will be used.  The conservation principles are used to analyze the collision and the subsequent motion of the pendulum.  The completely inelastic collision associated with the capture of the projectile in the pendulum and the subsequent motion of the pendulum provide the data necessary for the determination of the initial velocity.

In the second technique, the measured parameters of the trajectory of a horizontally launched projectile are used to determine the initial velocity.  With the projectile moving in a free-fall trajectory, constant acceleration kinematics will be used to determine the initial velocity from measurements of the horizontal range and vertical drop.

In each case, the projectile will be launched with the same device allowing a comparison of the initial velocity determinations of the two techniques.

### Ballistic Pendulum

The ballistic pendulum is so named because it was originally used to measure the velocity of high-speed projectiles such as bullets long before electric and electronic timers made the procedure unnecessary. It remains, however, as a simple and demonstrative device for understanding the conservation principles of energy and momentum. In analyzing the problem, the system will consist of the projectile and the more massive pendulum. As illustrated in the left image in {numref}`M06Fig01`, before the collision, the projectile is in motion horizontally towards the stationary pendulum. After the collision, the projectile is imbedded in the pendulum and the pendulum is moving along the arc as shown in the right image of {numref}`M06Fig01`.

```{figure} ExperimentBallisticPendulumFigures/Figure01a.jpg
:name: M06Fig01
:width: 600px
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

### Projectile Motion

When a projectile is moving solely under the influence of the force of gravity, we say that the projectile is in free-fall. Consider the launching of the same ball used in the ballistic pendulum. In this case, the pendulum will be swung up out of the way so the flight of the ball will continue off the edge of the table, eventually hitting the floor some distance away. This situation is illustrated in {numref}`M06Fig02`.

```{figure} ExperimentBallisticPendulumFigures/M06_fig02.jpg
:name: M06Fig02
:width: 700px
:align: center

Projectile Motion
```

Once the ball leaves the spring gun used to launch the ball, the ball is in free-fall. The vertical and horizontal motions are completely independent. We assume that once the ball leaves the gun, there are no energy loss mechanisms during the flight of the ball.

In the vertical direction, the initial velocity is zero and the ball is accelerated downward by its weight, finally hitting the floor some time, $t$, later, dropping a vertical distance of $Y$.
In the horizontal direction, the ball has a constant velocity of $v_0$ during the entire flight over the horizontal distance $X$.

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

### Ballistic Pendulum Procedure

<iframe width="560" height="315" src="https://www.youtube.com/embed/OjMF7Z2Pe6U?si=j9aSi4RHe3IBDj4R" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


1. **Data table:**
   - Create a table of the common data for the ballistic pendulum experiment including the mass of the ball $m$, the mass of the pendulum $M$, the initial pendulum height $y_1$ and any other common data needed for calculations.
   - Create a table with a row for each of the ten trials in the ballistic pendulum part of this lab including the trial number, the pendulum height $y_2$, the change in height $y_2-y_1$, the calculated velocity of the pendulum $V$, and the calculated initial velocity of the ball $v_0$.
   - Create a table to summarize the ten trials including the average pendulum height $y_2$, the average change in height $y_2-y_1$, the average velocity of the pendulum $V$, the average initial velocity of the ball $v_0$, the standard deviation of $v_0$.

2. Measure and record the mass of the brass ball projectile.

3. Record the mass of the pendulum that is indicated on the apparatus.

4. Practice the following procedure before actually taking data.

5. The pointer on the side of the bob indicates the center of mass of the pendulum. With the pendulum hanging motionless, measure the height above the base plate of the pointer. This value is $y_1$. Record the value in meters.

6. Place the brass ball on the pin of the gun and press the ball so the spring of the gun is compressed until the trigger catches and holds the compressed spring.

7. Fire the gun by squeezing the trigger. The ball will be captured by the bob and the pendulum will swing upwards.

8. A small ratchet engaging a rack will capture the maximum upswing position of the pendulum. Measure the height to the tip of the metal pointer on the pendulum which represents the center of mass of the pendulum with ball.

9. Carefully release the ratchet so the pendulum can swing back to its equilibrium position.

10. Release the ball from the bob of the pendulum by pushing it with your finger or a short cylinder.

11. Fire the ball ten times, and record the pendulum height $y_2$ for each shot.

12. Calculate the average $y = y_2-y_1$ and the average $v_0$ from {eq}`eq-M06v0`.

13. Record your data and calculations on your spreadsheet.

### Projectile Motion Procedure

1. **Data table:**
   - Create a table of the common data for the projectile motion experiment including the distance to the pad $x_1$, the vertical distance $Y$ and any other measurements.
   - Create a table with a row for each of the ten trials in the projectile motion part of this lab including the trial number, the measured $x_2$, the calculated horizontal distance $X=x_1+x_2$ and the calculated initial velocity of the ball $v_0$.
   - Create a table to summarize the ten trials including the average initial velocity $v_0$ of the ball, the standard deviation of $v_0$.

2. Set up the projectile motion experiment as shown in {numref}`M06Fig02`.

3. Perform $n=10$ measurements of $x_2$. Be careful that the gun is in the same position for each measurement

4. Calculate the standard deviation for the $n=10$ measurements of $x_2$.

## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet)
- What is the range of your measurements for both pendulum and projectile? Do the initial velocities agree within the ranges when treating your standard deviations as your uncertainty of average values?
- How and why are they (or could be) different.
- Which of the two results for the value of $v_i$ do you trust more? Explain your answer using a Physics argument.
- Suppose you would have used a more massive marble in the projectile motion portion of the experiment. How would this affect your result? Explain your answer.
- What are the effects of measured uncertainties on your determined velocities?
- What are possible systematic errors for today's experiments?

## The Whiteboard

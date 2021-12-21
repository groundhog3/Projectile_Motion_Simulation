# Projectile_Motion_Simulation
This Projectile Motion Simulation was coded in Vanilla JS with the p5 library used for 2d animation along with HTML + Bootstrap. 

# p5 JS
p5 is a JavaScript library for drawing that comes with many different features.
<br>This library has two main features which were useful for this simulation:
1. Drawing Function – With `setup()` and `draw()` functions, the library can automatically initialize an HTML canvas with some features, and draw frames at a specified `frameRate()`. The `loop()` and `noLoop()` features were used to control this process. 
2. Vector Arithmetic – Although vector arithmetic wasn't necessary for simulation, I stored both the position and velocities as `Vector` objects which cut down on code and made it easier to perfom calculations. 
3. Key Press – The library comes with two functions built-in: `keyPressed()` and `keyReleased()` which made it easy to use the spacebar to pause the animation. 

# Limits
Because this simulation used a drawing library that is known for being slow, this simulation has two drawbacks:
1. Lag – Depending on what settings are used, the projectile lags as its being drawn.
2. Precision – Because of `performance.now()` used for timing, and rounding errors with `Vector` objects in the p5 library, the distances and speeds displayed are not very accurate in the simulation.

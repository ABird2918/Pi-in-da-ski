# Pi-In-Da-Sky

## Table Of Contents
[Planning](#Planning)

## Planning

### Final Function
The final function of our project will consist of a Pico suspended safely within a soccer ball that collects acceleration and rotation data while it’s being kicked around. The ball will be in two halves and lock into place to make retrieving and replacing the Pico easy. If we have extra time we’d like to model the path of our ball in a 3D space.

### Diagrams
<img src="https://github.com/ABird2918/Pi-in-da-ski/assets/91289646/fcd7e84f-b6c8-408e-a637-fcff89d3e4c5" width="600"/>
<img src="https://github.com/ABird2918/Pi-in-da-ski/assets/91289646/def695e8-ccb8-4d83-b86b-26c83e6c8851" width="600"/>

### Materials
PLA, Foam, Pico, Elastic Bands, Popped Soccer Ball, Pico Breadboard, and Accelerometer
PLA: $6
Pico and breadboard: $6
Bands: $5
Soccer ball: bring from home
Accelerometer: $25 assuming we might need 2 throughout the project

### What To Learn:
How to do Dead Reckoning, how to specifically lock the ball, how we seamlessly assemble the two balls, and how to prevent the ball from breaking after being kicked. 

### Definition of Success
We will be successful when we are able to report and graph the acceleration of the ball after it is kicked which will allow us to determine velocity and position of the ball too. We also require 100% survivability of the device so we won’t be successful unless the ball remains intact completely and the pico undamaged.

### Safety Concerns
P: The ball shattering on impact and sending shrapnel everywhere.
S: We make our ball strong enough to withstand a kick and we pad the PLA part so that it will remain contained if it breaks
P: Someone getting hit with the ball and getting hurt
S: We will not kick the ball toward any person unless passing in a very controlled manner with confirmation of active participation from all parties.
P: Our Pico lighting on fire in our ball and creating a big blaze.
S: We will do our best to mitigate fire concerns such as creating a fireproof prototype but we will also have potential fire protocols in place as reactive measures…worst case scenario we make smores.

### Schedule
Jan week 1: Create CAD prototype, start code and testing for accelerometer.  
Jan week 2: Edit CAD prototype, get all outside materials, finish basic accelerometer code.  
Jan week 3: Print and create physical prototype, use accelerometer to initiate dead reckoning.  
Jan week 4: Iterate physical prototype after it inevitably not working properly, continue dead reckoning testing.  
Jan week 5: Relatively finalize physical prototype, code dead reckoning to report results to driver.  
Feb week 1: One week of leeway for testing code and adjusting together.  
Feb week 2: Test code on physical prototype inside in ideal conditions gently.  
Feb week 3: Test code a little less gently and adjust code and iterate prototype.  
Feb week 4: Move outside to test and iterate.  
Mar week 1: Work on tweaking accuracy on dead reckoning and what it delivers to us.  
Mar week 2: Test and tweak.  
Mar week 3: Finalize ball and use for testing code.  
Mar week 4: Leeway for whatever needs done.  
Apri week 2, 3, 4: shoot the ball and track it.  
May week 1: Document successes/failures/project and use data to create a super cool training interface.  
May week 2: Document, work on data display.  
May week 3: Finish documentation and data display video.  
May week 4&5: Leeway time.  

### Code
We have anticipated some problems regarding the various forces acting on our soccer ball and how we will be able to successfully track its movement using just an accelerometer so the code will have to be a potentially dynamic plan but I will do my best to show the gist.

  #### Pseudo-Code
  Set up accelerometer
  Add up the net x translation changes accounting for any tipping or rotating
  Print total x value
  Add up the net y translation changes accounting for any tipping or rotating
  Print total y value
  Add up net z translation changes accounting for any tipping or rotating
  Print total z value
  Triangulate the values to map the position of the ball at time t
  Derive velocity at any given t from the position
  Derive acceleration at any given t from velocity
  Graph position, velocity, and acceleration of the ball throughout its travels
  ***IF WE HAVE TIME create a 3d representation of how the ball moved on a real field including bounces etc


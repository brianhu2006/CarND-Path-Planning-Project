# The Goal of this Project
 The goal is to design a path planner that is able to create smooth,
  safe paths for the car to follow along a 3 lane highway with traffic. 
  A successful path planner will be able to keep inside its lane, avoid hitting other cars,
   and pass slower moving traffic all by using localization, sensor fusion, and map data.

#Model
 1. use Frent coordinate and keep car in middle of road to keep in road center
 2. set velocity as zero at first and increase car velocity by ref_vel (0.224) if there no car in front
    or decrease car by  ref_vel (-0.224)
 3. use spline to make the tranjectory smooth
 4. use the sensor fusion data to cehck if there is car in lane and decide if make lane change
 
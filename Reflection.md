# Reflection

## Maneuver Decisions

The maneuvers done are decided as follows:

If there is a car ahead in the same lane and within a distance of 40 points. The right and left lanes are checked for an available lane change maneuver. The restrictions are as follows, if there is a car within 20 points backwards or 40 points ahead on the desired lane, a lane change can not happen. So we slow down according to the velocity of the car ahead.

## Path Generation
Initially, I started with adding the previous path to the spline, if exists. Otherwise, I start adding the car coordinates and calculate a previous point in respect to the car. Then I start getting 3 points ahead according to the path decided above and add them to the spline x and y, , then I called the spline.set_points() to generate a smooth path for the next movemenent. 


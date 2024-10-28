---
tags:
reference:
  - "[[railway system]]"
---

When there is no signal in a railway network, automated trains travel freely on the rail without avoiding others, which causes them to collide. To avoid collisions, it is essential to deploy **railway signals** properly to direct the trains.

# Railway Blocks
Railway blocks are connected components seperated by railway signals. They are the smallest units of a signaling railway system, that can hold at most one automated train simutaneously.

Two pieces of railway are defined to be (topologically) connected, if one of the following holds:
1. they connect with each other by their ends, such that trains can travel directly from one to another;
2. they branch from the same end of another piece of railway;
3. they cross each other;
4. they are too close to each other.
The last three condition can be concluded 

When a block signal or a path signal is attached to the railway, the railway splits into two pieces at the attaching point, and the connectivity

# Block Signals


block signal causes collisions

# Behaviours of Trains
## Path Selection
Trains always travel on shortest paths from stations to stations, so they do not alter routes according to signals, but just brake and accelarate on previously routes.

In a self driving routine, when the automated train is stopped and ready to depart for the next station, it searchs for a shortest valid path.
That means, the train finds a shortest path such that all of the following hold:
1. the locomotives of the train can lead it to the next station along the rail without backing;
2. focusing on the path, all the railway blocks, until the next station, have a exit signal on the direction of the train.
When all conditions are satisfied, the train determines its path until it stops, regardless of any

## Interactions with Signals
Trains can foresee red signals ahead on their routes, no matter how many green signals are between. They brake at a distance to stop before red signals.

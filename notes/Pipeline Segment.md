---
tags:
reference:
  - "[[pipeline system]]"
---

A bare **pipeline segment** is refered to a single piece of pipeline without any objects attached to it, including other pipelines, pumps, floor holes, etc.

Here we introduce some concepts to illustrate how it works.

# Endpoint
The two **endpoint**s of a bare pipeline segment locate at the centers of its both ending cross-sections.

# Length
The **length** of a pipeline segment is the distance between its two endpoints, regardless of its shape.

# Max Volume
## Displayed Max Volume
The **displayed max volume** is given by $\max\{5,~0.65^2\pi\times length\}$ cubic metres.
## Actual Max Volume
The **actual max volume** is 1.4 times of the displayed max volume.

# Current Volume
## Displayed Current Volume
The **current volume displayed** by the terminal is a mean value of volume since one opens the terminal or some ticks before current time, whichever is the later.

# Head Lift Pressure
Liquid inside a pipeline segment can provide **head lift pressure**, due to Pascal's principle.
The head lift height provided by the segment is mainly linear to the current volume inside the segment.
## Range
To be explicit, the **lowest** height of head lift is the height of the lower endpoint of the segment.
The **highest** height of head lift is given by:
$$height~of~the~higher~endpoint + 1.3 \cos\theta$$
, where $\theta$ denotes the angle between the horizontal plane and the line determined by the two endpoints of the segment.
## Max Head Lift Volume
The **max head lift volume** is the same as the **displayed max volume**, that is $\max\{5,~0.65^2\pi\times length\}$ cubic metres.
When the **current volume** is slightly larger than 0, the provided head lift is at the lowest height. **(What about 0?)**
When the current volume is not less than the max head lift volume, the provided head lift is at the highest height.
Between them, the head lift is linear to the current volume.

# Pressure Transmission
When volume is more than the max head lift volume,

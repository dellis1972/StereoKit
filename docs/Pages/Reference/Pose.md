---
layout: default
title: Pose
description: Pose represents a location and orientation in space, excluding scale!
---
# Pose

Pose represents a location and orientation in space, excluding scale!


## Instance Fields and Properties

|  |  |
|--|--|
|[Quat]({{site.url}}/Pages/Reference/Quat.html) [orientation]({{site.url}}/Pages/Reference/Pose/orientation.html)|Orientation of the pose, stored as a rotation from Vec3.Forward.|
|[Vec3]({{site.url}}/Pages/Reference/Vec3.html) [position]({{site.url}}/Pages/Reference/Pose/position.html)|Location of the pose.|


## Instance Methods

|  |  |
|--|--|
|[Pose]({{site.url}}/Pages/Reference/Pose/Pose.html)|Basic initialization constructor! Just copies in the provided values directly.|
|[ToMatrix]({{site.url}}/Pages/Reference/Pose/ToMatrix.html)|Converts this pose into a transform matrix, incorporating a provided scale value.|


## Static Fields and Properties

|  |  |
|--|--|
|[Vec3]({{site.url}}/Pages/Reference/Vec3.html) [Forward]({{site.url}}/Pages/Reference/Pose/Forward.html)|Calculates the forward direction from this pose. This is done by multiplying the orientation with Vec3.Forward. Remember that Forward points down the -Z axis!|
|[Vec3]({{site.url}}/Pages/Reference/Vec3.html) [Right]({{site.url}}/Pages/Reference/Pose/Right.html)|Calculates the right (+X) direction from this pose. This is done by multiplying the orientation with Vec3.Right.|
|[Vec3]({{site.url}}/Pages/Reference/Vec3.html) [Up]({{site.url}}/Pages/Reference/Pose/Up.html)|Calculates the up (+Y) direction from this pose. This is done by multiplying the orientation with Vec3.Up.|


## Static Methods

|  |  |
|--|--|
|[Lerp]({{site.url}}/Pages/Reference/Pose/Lerp.html)|Interpolates between two poses! t is unclamped, so values outside of (0,1) will extrapolate their position.|


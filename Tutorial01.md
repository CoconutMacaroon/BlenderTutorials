# Tutorial One - UFO

Here, we will be making a UFO coming to earth in Blender.

## Step One

Delete the default cube. We don't need it.

## Step Two

Change the render engine to Cycles. If you have a GPU, set device to GPU Compute. If you have an Nvidia RTX, set the feature set to Experimental. I am using Blender 2.90.0.

## Step Three

Download [this city](https://free3d.com/3d-model/sci-fi-downtown-city-53758.html), and extract the download. Back in Blender, do `File > Import > Wavefront (obj)`, and select the city. It will take a moment to think, as it is a big file. Blender imported it huge. Oh no. Set the scale (for X, Y, and Z) to 0.1.

## Step Four

Time to make the UFO. I used Fusion 360, but I won't be covering much about how to do it, so I would advise just downloading the `UFO.stl` from this GitHub repo. Import it into Blender by doing `File > Import > STL`, and select the UFO, and import it. Uh oh. It is big and sideways. Set its `Rotation X` to 90. Set its scale for X, Y, and Z to 0.05. Now, lets put the UFO somewhere useful. You can put it where-ever you want, but I put it at X=10, Y=1, Z=17. Alright. It is inside a building, but we can fix that. This is a problem with the city. Right click on the city, and do `Set Origin > Origin to Center of Mass (Surface)`. Now set the city's Location X, Y, and Z to 0. Done.

## Step Four

We could just render now, but it wouldn't look very good. We need textures and materials. Go to the Shading tab in Blender. Click on the UFO, and then click `New`. In the nodes menu, there should be a green node that says `Principled BSDF`. Click on base color, and make it black. The UFO in the viewport might not look black, but if Base Color is black, you are fine.

## Step Five

This looks good, but the UFO needs a light beam. Go back into the Layout tab, and to Shift A, and do Mesh > Cone. Set its scale to 5, 5, and 15 for X, Y, and Z, respectablly.  Set its location X and Y to the same as the UFO's, and set the Z to whatever you think looks good. I choose 1.75.
## Texturing the light beam.
So, the light needs to look better.
Create this shader ![shader preview](Screenshot%202020-09-19%20081259.png) Feel free to tweak the values, but I liked these.

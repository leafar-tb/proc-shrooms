# Procedural Mushrooms
This Blender plugin adds operators for creating procedural mushroom meshes.
The operators are explained in more detail below.
To install the addon simply point Blender to a [zip](https://github.com/leafar-tb/proc-shrooms/archive/master.zip) of this repo.
<p align="center"><img height="200px" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/mushroom.png"></p>

## Installation and Usage
If you are familiar with Blender, you can probably skip this.

To install the addon, open the User Preferences via *File->User Preferences* (*Ctrl+Alt+u* should work, too).
There go to the *Add-ons* tab and on the bottom click *Install from File*.
Now simply point Blender to the [zip](https://github.com/leafar-tb/proc-shrooms/archive/master.zip).
Finally, you have to activate the addon (still in the *Add-ons* tab).
Just find it in the *User* category or using the search bar on the top-left and activate the check box.

To call an operator, hit space in the 3D view and start typing its name, then select it from the the shown suggestions.
(Operator names are highlighted in *italics* in the following sections.)
The operator panel will probably appear towards the left.
There you'll find the settings affecting the operator.
When the name of a setting is not helpful, try hovering the mouse over a value for a longer explanation.
Your changes to the settings are directly applied, so you can also play around with them to see what they do.
(It will use a fresh random seed with each change, so generated results will vary.)

## Generation
The first operator is named *Generate Mushroom(s)*.
You can choose how many and what style of mushroom you want to generate.
You can also specify how fine you want the mesh to be.
<p align="center">
  <img width="45%" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/generate3.png">
  <img width="45%" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/generate4.png">
  </br><sup>Examples of generated Mushrooms</sup>
</p>
You can also add some noise, to let the mushrooms appear more naturally grown.
<p align="center"><img width="40%" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/noise.png"></p>

## Mutation
When invoking the *Mutate Mushroom* operator on a selected mushroom a number of variations is produced based on it.
The amount of change is controlled by a 'radiation' parameter.
<p align="center">
  <img width="80%" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/mutate1.png">
  <img width="80%" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/mutate2.png">
  </br><sup>A base Mushroom(left) with four 'mutated' Variants</sup>
</p>

## Procreation
The *Combine Mushrooms* operator allows you to merge the features of two or more selected mushrooms.
The features of the created mushrooms are either inherited from one parent directly or averaged over the gene pool.
<p align="center">
  <img width="45%" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/combine1.png">
  <img width="45%" src="https://raw.githubusercontent.com/leafar-tb/proc-shrooms/master/images/combine2.png">
  </br><sup>Two parent Mushrooms(top) and three Offspring</sup>
</p>

## Fine Tuning
With the *Edit Mushroom* operator you create a copy of a mushroom and get to modify all of the parameters used in its generation.
You can also use this operator to recreate a mushroom with higher/lower detail or add/remove the noise effect.

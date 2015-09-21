# Sounthar Manickavasagam
# Assignment 2 - Freestyle Visualization

["Periodic Table and Reactions"](http://msounthar.github.io/02-Freestyle/index.html).

# Purpose

Main pupose of this visualization is to illustrate the periodic table with atomic structure of various elements with ease and to see the changes to the electron configuration when two elements react with each other.

I wanted to make the periodic table interactive and show the electons in action along with how the electrons move from one element's orbit to another's orbit.

# Data & Transformations

I got the periodic table as a json file online. Each element has the following properties,

group,
position,
name,
number,
small,
molar,
electrons,
children

I have used all the properties available in this json in this visualization. 

I also created my own data set called "Reactions.json" which has the reactants and products information for each compound with information about their transformations after the reaction.I came up with the fields and structure which are compatible with my code for the periodic table.


# Visual Encodings

I have maintained the precise ordering of the periodic table. Electon configuration of each element is accurate.

I have also visualized the changes to the atomic structure after a reaction through different colors for Reactant 1 and Reactant 2 , so the users can clearly see from which element the electron jumped and to where.

# Technical Achievements

I have heavily modified the d3.layouts.orbit library to make it work with this data set. 
Code is written in a dynamic way, so any number of elements and reactions can be added in the future.
Extensive data processing like dynamicly creating children array for each element is done as its a required format expected by the library.
I have done extensive css to come up with this look and feel.

# Design Achievements

I wanted to have atomic animation has a background for each element in the periodic table, but it became very slow when all the elements animation are shown at once. So I redesigned to this design of clicking the element to view its structure along with its group,name,symbol,molar value.

I was able to show the foriegn electron in an element after the reaction by changing its color which makes it very easy to preceive. 

I have also clearly shown the notations for the reaction and ability to see different reactions using a dropdown.


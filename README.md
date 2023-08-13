#### DAE-project (in progress)

I will use this repository for my learning project from the Data Analytics Essentials course of Cisco Skills For all course.

Currently I have data about size of proteins and different transitions between protein classes.
I have a tree of the proteins where each branch represents that two proteins are _very_ similar, at least in a certain representation of their structure.
Maybe in the future I could put online the tree, for everyone to search an specific protein an the proteins that are related with it, following that criteria.
For now, I have no demo and a lot of the data is private, sorry for not sharing it.

## Table of Contents
For now there is only a README file, but wait for updates.

## Current goals

For this little project, I will concentrate on two questions:
How big are the proteins that can do a transition?
Is there a rise in the capability to transition that could be related to the size of the proteins?

This is a good project to link this exersice with my PhD project. It could give me insight as to where to look.

## Data understaing

As I said, I have data for a representation of proteins. That representation depends of a _contact distance_, the distance between two atoms in the protein, and we can define vecinities for each _contact distance_:
Two atoms are neighbors if the distance between each other is equal or less than a _contact distance_.
Two atoms are neighbors if there is a real chemical bond between them.
We count a _cluster class_ of size N, if all N atoms are neighbors of the other N-1 atoms in the _cluster class_.
Each protein with a stable configuration has a count of _cluster classes_.
Under this representation, two proteins are similar if they have similar count of more or less the same _cluster classes_.

## Screenshot of the tree
![zoom](https://github.com/nitramnauj/DAE-project/assets/141964349/f286812e-0782-407e-8294-95d3903f6fd8)
Here I share you a zoom screenshot of one of my trees.
This is for a _contact distance_ of 9 Ångström.
Each node is a protein. Each color is a protein class, as in CATH database.
The size of the nodes is proportional to the size of the protein.

## Technologies

Java was used for the counting of _cluster classes_, using concurrent computing due the large size of the Protein Database.
For looking for pairs of similar proteins, I used Python3. Also the graph in the screenshot was generated with using Python3.
I want use data analysis tools for answer the two questions in this repository.

## Setup
In the near future, maybe I will share one or two programs for that specific analysis.

## Approach
Obtaining data:
Data preparation:
Testing outcomes:

## Credits
I will share it soon.

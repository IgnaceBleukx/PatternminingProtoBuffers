# Toy datasets of Protobuffers
**DISCLAIMER** These datasets are generated automatically and are for educational use only!

This repository contains the datasets for the thesis of Ignace Bleukx regarding recognizing protobuffer classes from binary data.

## Dataset structure
Every dataset in this repository has the same structure.
The datasets are strucutred as follows:
1. *binary*: The serialized version of the class
2. *n_att*: The number of attributes (primitives) in the class
3. *n_obj*: The number of nested objects at this level of the class
4. *depth*: The maximum depth of recursive objects in the class
5. *cname*: The class name
6. *children*: A nested list containing the class names of the classes children (subclasses) (see next paragraph)
7. *begin_end*: A list with the same shape as *children* with the begin and en index of each child in the binary string (see next paragraph)

## Nested list structure
The nested lists containing the children and start and end positions are structured as follows:
``` 
[curr_objct [child1 [child1.1 ...]][child2 [...]]...[childn[...]]]
``` 
So if a class has no children, the result is still a list containing 1 item: the class itself.

## Dataset titles
The datasets all have the same structured file name:

## Generation process
The files are generated using the following algorithm:
TODO: insert screenshot of algorithm 4

## File name structure
<img src="https://bit.ly/34m4Oaw" align="center" border="0" alt="dataset\_[n_{decl}]c\_[n_{inst}]inst\_fprob[probability]\_depth[depth].pickle" width="592" height="19" />

## Link to datasets
All datasets can be downloaded via the following [link]{https://www.dropbox.com/sh/4wc3dqwl2bko447/AACaBql3TYvxtHgsdH15ntPwa?dl=0}

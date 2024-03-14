# 3DPass Node official upgrade version
This is an official [3DPass Node](https://github.com/3Dpass/3DP) release created especially to ensure the network stability, while delpoying the fix for the [issue 71](https://github.com/3Dpass/3DP/issues/71). 

The upgrade includes the object validation check on new block import:

1. Vertex {} points to an invalid halfedge
2. Halfedge {} pointed to by vertex {} does not start in that vertex, but instead in {}
3. Vertex {} does not point to a halfedge
4. Halfedge {} points to an invalid twin halfedge {}
5. Halfedge twin pointed to by halfedge {} does not point back to halfedge
6. Invalid orientation: The halfedge {} and its twin halfedge {} points to the same vertex {}
7. Halfedge {} does not point to a twin halfedge
8. Halfedge {} points to an invalid vertex {}
9. Halfedge {} does not point to a vertex
10. Halfedge {} points to an invalid face {}
11. Halfedge {} points to a face but not a next halfedge
12. Halfedge {} points to an invalid next halfedge {}
13. Halfedge {} points to a next halfedge but not a face
14. Halfedge next pointed to by halfedge {} does not point back to halfedge
15. Length of edge {} is too small
16. Face {} points to an invalid halfedge {}
17. Halfedge pointed to by face {} does not point to back to face
18. Face {} does not point to a halfedge
19. Area of face {} is too small ({})
20. Vertex {} and Vertex {} is connected one way, but not the other way
21. Vertex {} and Vertex {} is connected by multiple edges
22. volume > 0.1 * bound_volume
  
## This is a major upgrade, which is mandatory for everyone! 
 
- The upgrade period: 2 days (by Mar 16th, 2024)
- All the nodes ignoring the upgrade will not be able to overpass the migration
- All the validators ignoring the upgrade will be removed out of the validator set with the penalty of 20000 P3D
- The sourcecodes will be released after the migration is completed

We hope, 3DPass community will support this important security upgrade.

## Upgrade your nodes! 

Sincerely, 
3DPass team

The file should be moved as below:
C:\Users\Username\AppData\Local\Autodesk\webdeploy\production\..\Applications\Electron\LibEagle\examples\ulps\examples

The location can be checked via ULP tool in Fusion360.
![Untitled](https://github.com/user-attachments/assets/fe4592ce-9ac4-42b5-8e57-5c1a4f439f4c)
![Untitled](https://github.com/user-attachments/assets/3e8fd79c-2df9-4a65-8c72-a716156bf808)

The program is based on the CCW spiral pattern in the default program. The changed points are below.
237:         sprintf( s, "ARC '%s' (%6.3f %6.3f) (%6.3f %6.3f) (%6.3f %6.3f);\n",
238:                      direction, endarc + offx, Y + offy, startarc + offx, Y + offy, startarc + offx, Y + offy);

242:        sprintf( s, "ARC (%6.3f %6.3f) (%6.3f %6.3f) (%6.3f %6.3f);\n",
243:                      end2arc + offx, Y + offy, endarc + offx, Y + offy, endarc + offx, Y + offy);

The pattern start point and end point were flipped.

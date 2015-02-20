OpenTelemac
===========

"The mathematically superior suite of solvers"

# Telemac


# STBTEL

## Algorithm to interpolate bathymetry on a mesh
For each mesh point, the space is divided into four quadrants (depends on the horizontal and vertical). For each quadrant, the software identifies the nearest bathymetry point, then a balance is done using the found points. Near the boundary or on the island case, it could be important to ignore the points too close from the boundary.
Indeed, the information found on these points could not be considered. The user is helped with the keyword MINIMUM DISTANCE AT BOUNDARY. When the mesh point are interpolated, this keyword dimensions the minimal distance below which a bathymetry points should be ignored

# Links
* opentelemac.org

OPquad.h
=========

Globals
----------------
Functions
----------------
- OPmesh OPquadCreate (  )

.. epigraph::
	.. raw:: html

		OPmesh OPquadCreate(OPint features, OPvec2 size);<br />

- OPmesh OPquadCreate ( OPfloat width, OPfloat height )
- OPmesh OPquadCreate ( OPfloat width, OPfloat height, OPvec2 offset )
- OPmesh OPquadCreate ( OPfloat width, OPfloat height, OPvec2 texcoordStart, OPvec2 texcoordEnd )
- OPmesh OPquadCreate ( OPfloat width, OPfloat height, OPvec2 offset, OPvec2 texcoordStart, OPvec2 texcoordEnd )
- OPmesh OPquadCreateZPlane (  )
- OPmesh OPquadCreateZPlane ( OPfloat width, OPfloat depth )
- OPmesh OPquadCreateZPlane ( OPfloat width, OPfloat depth, OPvec2 texcoordStart, OPvec2 texcoordEnd )
- OPmeshPacked OPquadCreatePacked (  )
- OPmesh OPquadNormCreate (  )
- OPmeshPacked OPquadNormCreatePacked (  )
- void OPquadDestroy ( OPmesh* quad )
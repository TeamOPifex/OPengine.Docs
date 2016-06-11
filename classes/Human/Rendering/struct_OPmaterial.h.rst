OPmaterial.h
=========

OPmaterialParam
----------------
-  type
- const OPchar* name
- void* data
- ui8 count
OPmaterial
----------------
- OPeffect* effect
-  params
- OPuint paramIndex
- ui64 id
- i8 depth
- i8 cull
- i8 alpha
Globals
----------------
Functions
----------------
- void OPmaterialClearParams ( OPmaterial* material )
- void OPmaterialInit ( OPmaterial* material, OPeffect* effect )
- OPmaterial* OPmaterialCreate ( OPeffect* effect )
- void OPmaterialAddParam ( OPmaterial* material,  paramType, const OPchar* name, void* data, ui8 count )
- void OPmaterialAddParam ( OPmaterial* material, const OPchar* name, OPtexture* data )
- void OPmaterialAddParam ( OPmaterial* material, const OPchar* name, OPvec3* data )
- void OPmaterialAddParam ( OPmaterial* material, const OPchar* name, OPvec4* data )
- void OPmaterialAddParam ( OPmaterial* material, const OPchar* name, OPmat4* data )
- void OPmaterialAddParam ( OPmaterial* material, const OPchar* name, OPmat4* data, ui8 count )
- void OPmaterialAddParam ( OPmaterial* material, const OPchar* name, f32* data )
- void OPmaterialBind ( OPmaterial* material )
- void OPmaterialBind ( OPmaterial* material, ui32 stride )
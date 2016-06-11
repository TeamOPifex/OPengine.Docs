OPvertexLayout.h
=========

OPvertexLayout
----------------
- ui16 count
- OPshaderAttribute* attributes
- ui32 stride
OPvertexLayoutBuilder
----------------
- ui32 index
-  names
-  types
-  counts
Globals
----------------
Functions
----------------
- void OPvertexLayoutInit ( OPvertexLayout* layout, ui16 count, OPchar* names,  types, ui8* counts )
- void OPvertexLayoutInit ( OPvertexLayout* layout, OPshaderAttribute* attributes, ui16 count )
- void OPvertexLayoutBuilderInit ( OPvertexLayoutBuilder* builder )
- OPvertexLayout OPvertexLayoutBuilderBuild ( OPvertexLayoutBuilder* builder )
- void OPvertexLayoutBuilderAdd ( OPvertexLayoutBuilder* builder,  attribute )
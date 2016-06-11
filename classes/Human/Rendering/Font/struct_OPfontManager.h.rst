OPfontManager.h
=========

OPfontTextNode
----------------
- OPchar* Text
- OPint Width

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

OPfontManager
----------------
- OPfontUserTextNode dummyMesh
- OPfont* _font
- OPvec4 _color
- OPfontAlign _align
- OPvector* currNodes
- bool isBuilt
- OPhashMap* builtNodes
- OPmeshPacker meshPacker
- OPint pixelated
- OPmat4 proj
- OPfloat scale
Globals
----------------
- OPfontManager* OPFONTMANAGER_ACTIVE
- OPeffect* OPFONTMANAGER_EFFECT_ACTIVE
- OPeffect* OPFONTMANAGER_EFFECT2D_ACTIVE
Functions
----------------
- OPfontManager* OPfontManagerCreate ( OPfont* font )
- OPfontManager* OPfontManagerSetup ( const OPchar* font, const OPchar* text, ui16 count )
- void OPfontManagerAddText ( const OPchar* text )
- void OPfontManagerBuild (  )
- void OPfontManagerDestroy ( OPfontManager* font )
- void OPfontManagerSetColor ( OPfontManager* manager, f32 r, f32 g, f32 b, f32 a )
- void OPfontManagerSetColor ( f32 r, f32 g, f32 b, f32 a )
- void OPfontEffectBind ( OPeffect* effect )

.. epigraph::
	.. raw:: html

		TODO: Refactor<br />

- void OPfontManagerBind ( OPfontManager* manager )
- void OPfontManagerSetAlign ( OPfontManager* manager, OPfontAlign align )
- void OPfontManagerSetAlign ( OPfontAlign align )
- void OPfontManagerSetColor ( OPfontManager* manager, OPvec3 color )
- void OPfontManagerSetColor ( OPfontManager* manager, OPvec4 color )
- void OPfontManagerSetColor ( OPfontManager* manager, f32 r, f32 g, f32 b )
- void OPfontManagerSetColor ( OPvec3 color )
- void OPfontManagerSetColor ( OPvec4 color )
- void OPfontManagerSetColor ( f32 r, f32 g, f32 b )
OPfont.h
=========

OPfont
----------------
- OPvector* glyphs
- OPfontAtlas* atlas
- OPtexture* texture
- OPfloat size
- OPint hinting
- OPint outlineType
- OPfloat outlineThickness
- OPint filtering
-  lcdWeights
- OPint kerning
- OPfloat height
- OPfloat lineGap
- OPfloat ascender
- OPfloat descender
- OPfloat underlinePosition
- OPfloat underlineThickness
OPfontBuiltTextNode
----------------
- OPmeshPacked* packedMesh
- OPfloat Width
OPfontUserTextNode
----------------
- OPmesh mesh
- OPfloat Width
Globals
----------------
Functions
----------------
- OPint OPfontLoad ( OPstream* str, OPfont* data )
- OPint OPfontUnload ( OPfont* font )
- OPfontGlyph* OPfontGetGlyph ( OPfont* font, OPchar charcode )
- OPmesh OPfontCreateText ( OPfont* font, OPchar* text )
- OPfontBuiltTextNode OPfontCreatePackedText ( OPfont* font, const OPchar* text )
- OPfontBuiltTextNode OPfontCreatePackedText ( OPfont* font, const OPchar* text, OPfloat scale )
- OPfontUserTextNode OPfontCreateUserText ( OPfont* font, const OPchar* text )
- OPfontUserTextNode OPfontCreateUserText ( OPfont* font, const OPchar* text, OPfloat scale )
- OPvec2 OPfontGetSize ( OPfont* font, const OPchar* text, OPfloat scale )
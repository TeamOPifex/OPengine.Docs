OPfontGlyph.h
=========

OPfontGlyph
----------------
- OPchar charcode
- OPint width
- OPint height
- OPint offsetX
- OPint offsetY
- OPfloat advanceX
- OPfloat advanceY
- OPvec4 textureCoordinates
- OPvector* kerning
- OPint outlineType
- OPfloat outlineThickness
Globals
----------------
Functions
----------------
- OPfontGlyph* OPfontGlyphCreate (  )
- void OPfontGlyphDestroy ( OPfontGlyph* glyph )
- OPfloat OPfontGlyphGetKerning ( OPfontGlyph* glyph, OPchar charcode )
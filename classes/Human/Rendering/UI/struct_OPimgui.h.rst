OPimgui.h
=========

OPimguiVertex
----------------
- OPvec3 Position
- OPvec4 Color
OPimgui
----------------
- OPrenderBuffer buffer
- OPmat4 proj
- OPvec4 primaryColor
- OPvec4 secondaryColor
- OPvec4 hoverColor
- OPvec4 borderColor
- OPvec4 padding
- OPvec4 margin
- OPuint borderSize
- OPfontManager* fontManager
- OPeffect* effect
Globals
----------------
- OPimgui* OPIMGUI_ACTIVE
Functions
----------------
- OPimgui* OPimguiCreate ( OPeffect* effect, OPfontManager* fontManager )
- void OPimguiBegin (  )
- void OPimguiEnd (  )
- OPint OPimguiRadio ( OPvec2 pos, OPvec2 size, OPvec4 color, OPvec4 selected )
- OPint OPimguiCheckbox ( OPint state, OPvec2 pos, OPvec2 size, OPvec4 color, OPvec4 selected, OPvec4 hover )
- OPint OPimguiButton ( OPvec2 pos, const OPchar* text, OPvec4 color, OPvec4 selected, OPvec4 hover )
- OPint OPimguiTextbox ( OPvec2 pos, const OPchar* text, const OPchar* placeholder, OPint active, OPint showCursor )
- void OPimguiLabel ( OPvec2 pos, const OPchar* text )
- void OPimguiLabel ( OPvec2 pos, OPvec2 size, const OPchar* text, OPvec4 bg, OPvec4 color, OPint fill )
- void OPimguiLabel ( OPvec2 pos, OPvec2 size, const OPchar* text, OPvec4 color )
- OPint OPimguiCheckbox ( OPint state, OPvec2 pos, OPvec2 size )
- OPint OPimguiButton ( OPvec2 pos, const OPchar* text )
- void OPimguiBind ( OPimgui* imgui )
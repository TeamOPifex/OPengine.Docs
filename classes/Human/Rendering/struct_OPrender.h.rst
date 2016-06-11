OPrender.h
=========

Globals
----------------
- i8 OPRENDER_INITIALIZED
- ui32 OPRENDER_WIDTH
- ui32 OPRENDER_HEIGHT
- ui32 OPRENDER_SCREEN_WIDTH
- ui32 OPRENDER_SCREEN_HEIGHT
- ui32 OPRENDER_SCALED_WIDTH
- ui32 OPRENDER_SCALED_HEIGHT
- f32 OPRENDER_SCREEN_WIDTH_SCALE
- f32 OPRENDER_SCREEN_HEIGHT_SCALE
- i8 OPRENDER_FULLSCREEN
- i8 OPRENDER_HAS_FOCUS
- OPuint OPRENDER_VAO
- GLFWwindow* window
- void() OP_WINDOW_DROP
Functions
----------------
- void OPrenderDragAndDropCB ( void() cb )
- OPwindow* OPrenderCreateWindow ( OPmonitor* monitor, bool fullscreen, const OPchar* title, ui32 width, ui32 height )
- OPint OPrenderInit (  )
- void OPrenderClear ( f32 r, f32 g, f32 b, f32 a )
- void OPrenderSetScreenSize ( ui32 width, ui32 height )
- void OPrenderSetViewport ( OPint x, OPint y, ui32 width, ui32 height )
- void OPrenderResetViewport (  )
- OPint OPrenderGetWidth (  )
- OPint OPrenderGetHeight (  )
- OPfloat OPrenderGetAspectRatio (  )
- OPfloat OPrenderGetWidthAspectRatio (  )
- OPfloat OPrenderGetHeightAspectRatio (  )
- void OPrenderCull ( OPint state )

.. epigraph::
	.. raw:: html

		Enables or Disables GL_CULL_FACE<br />

- void OPrenderCullMode ( OPint state )

.. epigraph::
	.. raw:: html

		Sets the direction of culling<br />

- void OPrenderSwapBuffer (  )
- void OPrenderPresent (  )
- void OPrenderUpdate (  )
- void OPrenderBlend ( OPint state )
- void OPrenderDepth ( OPint state )
- void OPrenderDepthWrite ( OPint state )
- void OPrenderShutdown (  )
- ui32 OPgetNativeScreenWidth (  )
- ui32 OPgetNativeScreenHeight (  )
- void OPrenderBlendAlpha (  )
- void OPrenderBlendAdditive (  )
- void OPrenderClear ( f32 r, f32 g, f32 b )

.. epigraph::
	.. raw:: html

		OPint OPrenderInit() {<br />return OPrenderInit(OPRENDER_WIDTH, OPRENDER_HEIGHT);<br />

- void OPrenderClear ( OPvec3 color )
- void OPrenderClear ( OPvec4 color )
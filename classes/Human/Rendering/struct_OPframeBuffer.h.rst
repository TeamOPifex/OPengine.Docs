OPframeBuffer.h
=========

OPframeBuffer
----------------
- OPtextureDescription Description
- OPtexture Texture
- ui32 Handle
- ui32 DepthBufferId
- ui32 RenderTextureId
- ui32 RenderFramebufferId
- ui32 ResolveTextureId
- ui32 ResolveFramebufferId
Globals
----------------
- OPframeBuffer* OPRENDER_CURR_FRAMEBUFFER

.. epigraph::
	.. raw:: html

		_____ _ _ _<br />/ ____| | | | | |<br />| | __| | ___ | |__ __ _| |___<br />| | |_ | |/ _ \| '_ \ / _` | / __|<br />| |__| | | (_) | |_) | (_| | \__ \<br />\_____|_|\___/|_.__/ \__,_|_|___/<br />

Functions
----------------
- OPframeBuffer OPframeBufferCreateShadow ( ui32 width, ui32 height )

.. epigraph::
	.. raw:: html

		______ _ _<br />____| | | (_)<br />|__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />__| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | |_| | | | | (__| |_| | (_) | | | \__ \<br />\__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- OPframeBuffer OPframeBufferCreateDepth ( OPtextureDescription desc )
- OPframeBuffer OPframeBufferCreate ( OPtextureDescription desc )
- OPframeBuffer OPframeBufferCreateVR ( ui32 width, ui32 height )
- void OPframeBufferDestroy ( OPframeBuffer* fb )
- void OPframeBufferAttach ( OPtexture* texture, ui16 pos )
- void OPframeBufferBind ( OPframeBuffer* fb )
- void OPframeBufferBindRead ( OPframeBuffer* fb )
- void OPframeBufferSetReadBuffer ( ui16 pos )
- void OPframeBufferSetReadBufferDepth (  )
- void OPframeBufferBindTex ( OPframeBuffer* fb )
- void OPframeBufferUnbind (  )
- void OPframeBufferAttachDepth ( OPtexture* texture )
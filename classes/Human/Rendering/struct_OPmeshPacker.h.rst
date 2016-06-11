OPmeshPacker.h
=========

OPmeshPacker
----------------
- OPrenderBuffer VertexBuffer
- OPrenderBuffer IndexBuffer
- OPuint vertexElementOffset
- OPuint vertexOffset
- OPuint indexOffset
- OPstream vertices
- OPstream indices
- OPint built

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

Globals
----------------
- OPmeshPacker* OPMESHPACKER_ACTIVE

.. epigraph::
	.. raw:: html

		_____ _ _ _<br />/ ____| | | | | |<br />| | __| | ___ | |__ __ _| |___<br />| | |_ | |/ _ \| '_ \ / _` | / __|<br />| |__| | | (_) | |_) | (_| | \__ \<br />\_____|_|\___/|_.__/ \__,_|_|___/<br />

Functions
----------------
- OPmeshPacker OPmeshPackerCreate (  )

.. epigraph::
	.. raw:: html

		______ _ _<br />____| | | (_)<br />|__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />__| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | |_| | | | | (__| |_| | (_) | | | \__ \<br />\__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- OPint OPmeshPackerDestroy ( OPmeshPacker* packer )
- OPuint OPmeshPackerAddVB ( ui32 vertexSize, void* verticesData, OPuint vertexCount )
- OPuint OPmeshPackerAddIB ( ui32 indexSize, void* indicesData, OPuint indexCount )
- void OPmeshPackerBuild (  )
- void OPmeshPackerBind ( OPmeshPacker* packer )
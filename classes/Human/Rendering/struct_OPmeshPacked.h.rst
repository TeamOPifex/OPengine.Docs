OPmeshPacked.h
=========

OPmeshPacked
----------------
- OPuint offset
- OPuint count
- OPuint elementCount

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

Globals
----------------
Functions
----------------
- OPmeshPacked OPmeshPackedCreate ( ui32 vertSize, ui32 indSize, OPuint vertCount, OPuint indCount, void* vertices, void* indices )

.. epigraph::
	.. raw:: html

		______ _ _<br />____| | | (_)<br />|__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />__| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | |_| | | | | (__| |_| | (_) | | | \__ \<br />\__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- void OPmeshPackedRender ( OPmeshPacked* mesh )
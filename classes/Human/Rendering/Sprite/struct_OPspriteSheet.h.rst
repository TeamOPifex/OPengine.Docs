OPspriteSheet.h
=========

OPspriteSheet
----------------
- OPint Width
- OPint Height
- OPint Sprites
- OPchar* Names
- OPtexture* Sheet

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />Used to maintain and clean up sprites that<br />have been stored in the manager<br />

OPspriteFrame
----------------
- OPvec2 Offset
- OPvec2 Size
- OPfloat Delay

.. epigraph::
	.. raw:: html

		Actual sprite offset data<br />

OPsprite
----------------
- OPint FrameCount
- OPspriteFrame* Frames
- OPint Frame
- OPfloat Elapsed
- OPtexture* Sheet

.. epigraph::
	.. raw:: html

		Sprite animation frames<br />

Globals
----------------
Functions
----------------
- OPint OPspriteSheetLoad ( OPstream* str, OPspriteSheet* ss )

.. epigraph::
	.. raw:: html

		______ _ _<br />| ____| | | (_)<br />| |__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />| __| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | | |_| | | | | (__| |_| | (_) | | | \__ \<br />|_| \__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- OPint OPspriteSheetUnload ( void* ss )
- OPvec2 OPspriteCurrentFrameSize ( OPsprite* sprite )
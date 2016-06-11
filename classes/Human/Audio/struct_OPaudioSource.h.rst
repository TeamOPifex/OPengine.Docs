OPaudioSource.h
=========

OPaudioDescription
----------------
- ui64 Length
- ui32 SamplesPerSecond
- ui16 BitsPerSample
- ui16 Channels
- ui16 Format
sOPaudioSource
----------------
- OPint() Read
- OPint() Seek
- OPaudioDescription Description
- void* DataSource
Globals
----------------
Functions
----------------
- OPint OPaudOpenWave ( const OPchar* filename, OPaudioSource* source )

.. epigraph::
	.. raw:: html

		____ _ ______<br />/ __ \ (_) | ____|<br />| | | |_ __ ___ _ __ _ _ __ __ _ | |__ _ _ _ __ ___ ___<br />| | | | '_ \ / _ \ '_ \| | '_ \ / _` | | __| | | | '_ \ / __/ __|<br />| |__| | |_) | __/ | | | | | | | (_| | | | | |_| | | | | (__\__ \_<br />\____/| .__/ \___|_| |_|_|_| |_|\__, | |_| \__,_|_| |_|\___|___(_)<br />| | __/ |<br />|_| |___/<br />

- OPint OPaudOpenOgg ( const OPchar* filename, OPaudioSource* source )
- OPint OPaudCloseWave ( OPaudioSource* src )

.. epigraph::
	.. raw:: html

		_____ _ _ ______<br />/ ____| | (_) | ____|<br />| | | | ___ ___ _ _ __ __ _ | |__ _ _ _ __ ___ ___<br />| | | |/ _ \/ __| | '_ \ / _` | | __| | | | '_ \ / __/ __|<br />| |____| | (_) \__ \ | | | | (_| | | | | |_| | | | | (__\__ \_<br />\_____|_|\___/|___/_|_| |_|\__, | |_| \__,_|_| |_|\___|___(_)<br />__/ |<br />|___/<br />

- OPint OPaudCloseOgg ( OPaudioSource* src )
- OPint OPaudReadWave ( OPaudioSource* src, ui64* position, ui8* dest, ui32 len )

.. epigraph::
	.. raw:: html

		_____ _ _ ______ _ _<br />| __ \ | (_) | ____| | | (_)<br />| |__) |___ __ _ __| |_ _ __ __ _ | |__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />| _ // _ \/ _` |/ _` | | '_ \ / _` | | __| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | \ \ __/ (_| | (_| | | | | | (_| | | | | |_| | | | | (__| |_| | (_) | | | \__ \<br />|_| \_\___|\__,_|\__,_|_|_| |_|\__, | |_| \__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />__/ |<br />|___/<br />

- OPint OPaudReadOgg ( OPaudioSource* src, ui64* position, ui8* dest, ui32 len )
- OPint OPaudSeekWave ( OPaudioSource* src, ui64* pos )

.. epigraph::
	.. raw:: html

		_____ _ _ ______ _ _<br />/ ____| | | (_) | ____| | | (_)<br />| (___ ___ ___| | ___ _ __ __ _ | |__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />\___ \ / _ \/ _ \ |/ / | '_ \ / _` | | __| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />____) | __/ __/ <| | | | | (_| | | | | |_| | | | | (__| |_| | (_) | | | \__ \<br />|_____/ \___|\___|_|\_\_|_| |_|\__, | |_| \__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />__/ |<br />|___/<br />

- OPint OPaudSeekOgg ( OPaudioSource* src, ui64* pos )
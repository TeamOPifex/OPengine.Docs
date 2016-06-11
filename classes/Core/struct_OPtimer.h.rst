OPtimer.h
=========

OPtimer
----------------
- ui64 TotalGametime
- ui64 Elapsed
- LARGE_INTEGER TimeLastTick
- LARGE_INTEGER Frequency

.. epigraph::
	.. raw:: html

		Struct definitions */<br />Time measurment object.<br />The OPtimer struct is responsible for keeping track of<br />time elapsed between ticks, and total time over all updates.<br />

Globals
----------------
Functions
----------------
- OPint OPtimerInit ( OPtimer* timer )

.. epigraph::
	.. raw:: html

		OPtimerInit - creates an OPtimer instance<br />Allocates space and initializes an OPtimer struct, then returns a<br />pointer to the allocated memory segment. If allocation fails, a NULL<br />pointer is returned.<br />

- void OPtimerTick ( OPtimer* timer )

.. epigraph::
	.. raw:: html

		OPtimerTick - updates a OPtimer<br />Updates an OPtimer instance with updated internal values representing<br />time at the moment of the call. This function will not check to see<br />if the OPtimer pointer is null before operating on it.<br />

- OPfloat OPtimerDelta ( OPtimer* timer )

.. epigraph::
	.. raw:: html

		OPtimerDelta - returns real time between ticks.<br />Acts as a getter for the appropriate internal values of the provided<br />OPtimer instance. The float value retuned is as a measurment in<br />milliseconds since the last call to OPtimerTick(). This function will<br />not check to see if the OPtimer pointer is null before operating on it.<br />

- ui64 OPtimerTotal ( OPtimer* timer )

.. epigraph::
	.. raw:: html

		OPtimerTotal - milliseconds since the timer's creation<br />Acts as a getter for the appropriate internal values of the provided<br />OPtimer instance. The unsigned integer value retuned is as a truncated<br />measurment of total milliseconds from the first call to OPtimerTick()<br />to the most recent call. This function will not check to see if the<br />OPtimer pointer is null before operating on it.<br />

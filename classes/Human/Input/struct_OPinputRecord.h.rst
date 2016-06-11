OPinputRecord.h
=========

OPinputRecordFrame
----------------
- ui64 timeOffset
- OPkeyboardState keyboardState
OPinputRecordMemoryBase
----------------
- void* Memory
- OPint MemorySize
Globals
----------------
Functions
----------------
- void OPinputRecordBegin ( OPtimer* start, OPinputRecordMemoryBase* memoryMaps, ui16 memoryMapCount )
- OPint OPinputRecordIsRunning (  )
- OPint OPinputRecordIsRecording (  )
- OPint OPinputRecordIsPlayingBack (  )
- void OPinputRecordUpdate ( OPtimer* timer )
- void OPinputRecordPlayback (  )
- void OPinputRecordEnd (  )
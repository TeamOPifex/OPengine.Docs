OPsharedLibrary.h
=========

OPsharedLibrarySymbol
----------------
- void* Symbol
- const OPchar* _symbolName

----------------
- HMODULE _library
- const OPchar* _libraryPath
- OPuint _lastModifiedTime
- OPlist* _symbols
OPdll
----------------
- HMODULE library
- const OPchar* path
Globals
----------------
Functions
----------------
- OPsharedLibrary* OPsharedLibraryLoad ( const OPchar* path )
- OPint OPsharedLibraryDestroy ( OPsharedLibrary* sharedLibrary )
- OPint OPsharedLibraryReload ( OPsharedLibrary* sharedLibrary )
- OPsharedLibrarySymbol* OPsharedLibraryLoadSymbol ( OPsharedLibrary* sharedLibrary, const OPchar* symbolName )
- OPint OPsharedLibraryClose ( OPsharedLibrary* sharedLibrary )
- OPdll OPdllOpen ( const OPchar* path )
- OPint OPdllUpdate ( OPdll* dll )
- void* OPdllSymbol ( OPdll* dll, const OPchar* symbol )
- void OPdllClose ( OPdll* dll )
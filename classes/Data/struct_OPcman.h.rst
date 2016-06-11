OPcman.h
=========

OPresourceFile
----------------
- OPfile resourceFile
- ui16 headerSize
- ui16 resourceCount
- OPchar* resourceNames
- ui32* resourceOffset
- ui32* resourceSize
OPassetLoader
----------------
-  Extension
- const OPchar* AssetTypePath
- OPint AssetSize
- OPint() Load
- OPint() Unload
- OPint() Reload
OPasset
----------------
- void* Asset
- OPint() Unload
- OPint Dirty
Globals
----------------
- OPhashMap OP_CMAN_HASHMAP
- OPassetLoader* OP_CMAN_ASSETLOADERS
- OPint OP_CMAN_ASSET_LOADER_COUNT
- OPlinkedList* OP_CMAN_PURGE
-  OP_CMAN_RESOURCE_FILES
Functions
----------------
- void OPcmanUpdate ( OPtimer* timer )

.. epigraph::
	.. raw:: html

		*Debug Only*<br />Watches the files of loaded resources for changes<br />Looks at Last Write Time for each file once every second<br />When a change happens the Reload method is called<br />

- void OPcmanAddLoader ( OPassetLoader* loader )

.. epigraph::
	.. raw:: html

		Adds a loader to be used when OPcmanInit is called<br />

- OPint OPcmanInit ( const OPchar* dir )

.. epigraph::
	.. raw:: html

		Initializes the Content Manager with an array of Asset Loaders<br />A custom directoy can be provided otherwise it defaults to assets/<br />

- OPint OPcmanPurge (  )

.. epigraph::
	.. raw:: html

		Unloads all assets that are no longer needed (marked deleted)<br />Assets that are no longer needed have been deleted with OPcmanDelete<br />

- OPint OPcmanIsLoaded ( const OPchar* key )

.. epigraph::
	.. raw:: html

		checks to see if an asset is loaded, triggers the load or unload.<br />

- OPint OPcmanLoad ( const OPchar* key )

.. epigraph::
	.. raw:: html

		Attempts to load an asset<br />

- OPint OPcmanUnload ( const OPchar* key )

.. epigraph::
	.. raw:: html

		Unloads a resource<br />

- void* OPcmanGet ( const OPchar* key )

.. epigraph::
	.. raw:: html

		Returns a pointer to the resource requested by file name<br />

- void* OPcmanLoadGet ( const OPchar* key )

.. epigraph::
	.. raw:: html

		Loads a resource and returns a pointer to the resource requested<br />

- OPint OPcmanDelete ( const OPchar* key )

.. epigraph::
	.. raw:: html

		Marks an asset as ready to delete<br />It will only be removed from memory when OPcmanPurge is called<br />

- void OPcmanDestroy (  )

.. epigraph::
	.. raw:: html

		Marks an asset as ready to delete<br />It will only be removed from memory when OPcmanPurge is called<br />

- OPint OPcmanSetDir ( OPchar* dir )
- void OPcmanLoadResourcePack ( const OPchar* filename )

.. epigraph::
	.. raw:: html

		Loads a Resource Pack into the OPcman<br />The header data is loaded into memory, but the individual resources will be loaded<br />at request. The FILE handle will remain open until the Resource Pack is unloaded.<br />

- OPstream* OPcmanGetResource ( const OPchar* resourceName )

.. epigraph::
	.. raw:: html

		Gets an asset OPstream out of a Resource Pack that has been loaded<br />It will look in Resource Packs in the order they were loaded. If no<br />resource could be found, it will return NULL<br />

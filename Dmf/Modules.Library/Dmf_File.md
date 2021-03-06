## DMF_File

-----------------------------------------------------------------------------------------------------------------------------------

#### Module Summary

-----------------------------------------------------------------------------------------------------------------------------------

Support for working with files in drivers.

-----------------------------------------------------------------------------------------------------------------------------------

#### Module Configuration

-----------------------------------------------------------------------------------------------------------------------------------

* None

-----------------------------------------------------------------------------------------------------------------------------------

#### Module Enumeration Types

* None

-----------------------------------------------------------------------------------------------------------------------------------

#### Module Structures

* None

-----------------------------------------------------------------------------------------------------------------------------------

#### Module Callbacks

-----------------------------------------------------------------------------------------------------------------------------------

* None

#### Module Methods

-----------------------------------------------------------------------------------------------------------------------------------

##### DMF_DMF_File_Read

````
_Must_inspect_result_
NTSTATUS
DMF_File_Read(
    _In_ DMFMODULE DmfModule,
    _In_ WDFSTRING FileName, 
    _Out_ WDFMEMORY* FileContentMemory
    );
````

Reads the contents of a file into a buffer that is allocated for the Client. Client is responsible
for freeing the allocated memory.

##### Returns

NTSTATUS

##### Parameters
Parameter | Description
----|----
DmfModule | An open DMF_File Module handle.
FileName  | Name of the file.
FileContentMemory | Buffer handle where read file contents are copied. The caller owns this memory.

##### Remarks

*

-----------------------------------------------------------------------------------------------------------------------------------

#### Module Children

* None

-----------------------------------------------------------------------------------------------------------------------------------

#### Module Implementation Details

* 

-----------------------------------------------------------------------------------------------------------------------------------

#### Examples

-----------------------------------------------------------------------------------------------------------------------------------

#### To Do

* Add support for Kernel-mode.

-----------------------------------------------------------------------------------------------------------------------------------
#### Module Category

-----------------------------------------------------------------------------------------------------------------------------------

Driver Patterns

-----------------------------------------------------------------------------------------------------------------------------------


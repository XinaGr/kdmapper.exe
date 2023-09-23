# kdmapper.exe
Creator: https://github.com/TheCruZ/kdmapper
# Features: 

```Works with /GS- compiled drivers
Hooks NtAddAtom which exists everywhere and is rarely called
Clears MmUnloadedDrivers
Clears PiDDBCacheTable
Clears g_KernelHashBucketList
Clears Wdfilter RuntimeDriverList RuntimeDriverCount and RuntimeDriverArry
Use NtLoadDriver and NtUnloadDriver for less traces
Prevent load if \Device\Nal exists (Prevents BSOD)
Header section skipped while copying driver to kernel
Added param --free to automatically unmap the allocated memory
Added param --mdl to map in mdl memory
Added param --indPages to map in allocated independent pages
Added param --PassAllocationPtr to pass allocation ptr as first param
Added the possibility to modify params before call driver entry
Now you can pass directly bytes to mapdriver function```

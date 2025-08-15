Created: Aug 15 2025
Class: [[Bootcamp]] 
- - -
# Static
A binary file for the library dependency is generated during the linker's process. The linker then bundles this in with the user's binary from the assembler. This can lead to redundant binary files being generated for libraries that will be compiled into more than one executable. Typically used for more niche and specific libraries.
# Dynamic
Incorporates any dependencies and libraries from DLLs (Dynamic Link Library).
DLLs are precompiled libraries that will get used by many different programs. Instead of generating a new binary for the library each time it is used, a DLL binary can be generated once and then used by each program's linkers. Typically used for standard libraries or system libraries.
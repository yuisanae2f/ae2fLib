# ae2fLib : C
> is the project of separating the code from [CPure](https://github.com/yuisanae2f/CPure).  
> Separated code will be updated here.

[Click here to check the available libraries.](./index.md)

# AE2F_IGNORE_MISSINGS
> Each of the headers which has any of critical dependencies would try to find it by including.  
> If you want it not, define AE2F_IGNORE_MISSINGS to halt it.

# `AE2F_CPP`
> Most of the code is written in Language of C.  
> If you are to use these in a landscape of C++, define `AE2F_CPP` to declare it.  
> Inlined class would be generated.

# Usage method
Check the critical dependency.
> You could check via each document which matches the header.  
> The top of the each pages shows the list of critical dependencies.  

Check the directory for linkers.
> You could find the library files which has an extension of lib and dll.  
> Take the file which has the name of the library you want.

Define the AE2F_PATH_C for .lib path.
> Each headers at the very first has the macros for implicit linking for .lib.  
> Once global directory for dll AE2F_PATH_C defined, rest will be done automatically.  
```c
#define AE2F_PATH_C "path/for/your/lib/"
```
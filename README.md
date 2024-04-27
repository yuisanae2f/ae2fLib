# ae2fLib : C
> is now managed as CMake.
> is the static library now.

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

# include
> On `include`, headers will be placed at `ae2fLib/libName/header.h`.

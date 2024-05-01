# ae2fLib : C
> is now managed as CMake.
> is the static library now.

> is the project of separating the code from [CPure](https://github.com/yuisanae2f/CPure).  
> Separated code will be updated here.

[Click here to check the available libraries.](./index.md)

# AE2F_IGNORE_MISSINGS
> Each of the headers which has any of critical dependencies would try to find it by including.  
> If you want it not, define `AE2F_IGNORE_MISSINGS` to halt it.

# `AE2F_CPP`
> Most of the code is written in Language of C.  
> If you are to use these in a landscape of C++, define `AE2F_CPP` to declare it.  
> Inlined class would be generated.

# Usage method
> Check the critical dependency.  
> You could check via each document which matches the header.  
> The top of the each pages shows the list of critical dependencies.  

# include
> On `include`, headers will be placed at `ae2fLib/libName/header.h`.

# Structure
> is the primitive structures applicable for a C landscape.  
> has a prefix of `ptr` as the pointer of this.

> Would be declared similiar to this.

Code
```c
typedef struct ae2f_Whatever {
    int member;
}* ptr_ae2f_Whatever;
```

# Functions
> Primitive functions are declared in global scope.  

> receives the pointer for an [`Structure`](#structure) as a receiver.  

# def
> An automatic type definer.  

> could access the type of its original and pointer easily.

Code
```cpp
namespace ae2f {
	template<typename t>
	class def {
	public:
		typedef t orig;
		typedef t* ptr;
	};
}
```

## t
> the type to introduce.

## orig
> its original type.

Code
```cpp
typedef t orig;
```

## ptr
> type of pointer of [`original type`](#orig).

Code
```cpp
typedef t* ptr;
```

# Abstractor
> contains only a pointer of the [`primitive types`](#structure).  
> has the inline function which calls the original functions.

> has the inheritance of [`def`](#def) for its [primitive type](#structure).

## raw
> Each abstractor has the function of `raw`.  
> This function would return the current pointer which this class contains.

# Classes
> contains the full instance of the [`Structure`](#structure).  
> expands certain [`Abstractor`](#abstractor) in order to use functions related to it.

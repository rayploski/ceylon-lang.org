---
layout: reference
title: Compilation Units
tab: documentation
unique_id: docspage
author: Tom Bentley
milestone: Milestone 1
---

# #{page.title}

A *compilation unit* is a text file with the filename extension 
`.ceylon`, containing one or more toplevel [declarations](#declarations).

## Usage 

Here's an example compilation unit in the package `com.example.foo` 
containing three toplevel declarations:

<!-- check:none -->
    import com.example.baz { Baz }

    shared interface Foo {
        // ...
    }

    shared class DefaultFoo() satisfies Foo {
        // ...
    }
    
    shared Baz? doFoo(Foo foo) {
        return null;
    }


## Description

Compilation units are a compile-time concept and have no representation or 
role at runtime.

### Declarations

A compilation unit must contain one or more declarations:

* [type declarations](../type) ([class](../class), 
  [interface](../interface) or [`object`](../object)), 
* [function declarations](../method), and/or
* [value declarations](../attribute).

Ceylon does not have Java's restriction on `public` (`shared`) classes having 
to be declared in a source file named after the class name.

### Source Location

A compilation unit belongs a [package](../package), determined 
by the location of the compilation unit in the source directory. 
For example, the compilation unit `<source-dir>/foo/bar/unit.ceylon` 
belongs to the package `foo.bar` if `<source-dir>` is the source 
directory.

All compilation units in a certain directory belong to the same
package.

## See also

* Compilation units belong to [packages](../package).

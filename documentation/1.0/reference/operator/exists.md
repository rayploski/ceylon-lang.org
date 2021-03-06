---
layout: reference
title: '`exists` operator'
tab: documentation
unique_id: docspage
author: Tom Bentley
milestone: Milestone 1
doc_root: ../../..
---

# #{page.title}

The non-associating, unary `exists` operator is used to test its operand for 
nullness.

## Usage 

    void m(Integer? num) {
        Boolean haveNum = num exists;
    }

## Description

### Definition

The meaning of `exists` is defined as follows:

<!-- check:none -->
    if (exists lhs) true else false

### Polymorphism

The `exists` operator is not [polymorphic](#{page.doc_root}/reference/operator/operator-polymorphism). 

### Note

Do not to confuse the `exists` *operator* described here and which 
takes form `attribute exists` with the 
[`exists` *condition*](../../statement/conditions) used in `if`, `assert` and 
`while` statements and which takes the form 
`exists attribute`.

## See also

* [`exists`](#{page.doc_root}/#{site.urls.spec_relative}#nullvalues) in the language specification.
* [operator precedence](#{page.doc_root}/#{site.urls.spec_relative}#operatorprecedence) in the 
  language specification

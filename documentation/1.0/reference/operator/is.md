---
layout: reference
title: '`is` operator'
tab: documentation
unique_id: docspage
author: Tom Bentley
milestone: Milestone 1
doc_root: ../../..
---

# #{page.title}

The non-associating, binary `is` operator is used to test the type of a 
variable.

## Usage 

    void m(Object? obj) {
        Boolean isNumber = obj is Number;
        Boolean isNull = obj is Null;
    }

## Description

### Definition

The `is` operator is primitive.

Note that because Ceylon supports reified generics you may use `is` with a
parameterized type, for example you can write

    Boolean intList = obj is List<Integer>;

### Polymorphism

The `is` operator is not [polymorphic](#{page.doc_root}/tour/language-module/#operator_polymorphism). 

### Note

Do not to confuse the `is` *operator* described here and which 
takes form `attribute is Type` with the 
[`is` *condition*](../../statement/conditions) used in `if`, `assert` and 
`while` statements and which takes the form 
`is Type attribute`.

## See also

* [`extends` operator](../extends)
* [`satisfies` operator](../satisfies)
* [operator precedence](#{page.doc_root}/#{site.urls.spec_relative}#operatorprecedence) in the 
  language specification
* [`if (is ...)` special form](../../statement/if#special_conditions)
* [`case (is ...)` special form](../../statement/switch#polymorphism)

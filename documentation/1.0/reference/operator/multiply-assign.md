---
layout: reference
title: '`*=` (multiply assign) operator'
tab: documentation
unique_id: docspage
author: Tom Bentley
milestone: Milestone 1
doc_root: ../../..
---

# #{page.title}

The right-associative, binary `*=` operator multiplies it's left-hand operand 
by the amount given by its right-hand operand and assigns the result to the 
left-hand operand.

## Usage 

<!-- cat: void m() { -->
    variable Integer num = 1;
    num *= 2; // double num 
    num *= num; // square num
<!-- cat: } -->

## Description


### Definition

The `*=` operator is defined as follows:

    lhs = lhs.times(rhs)

except that `lhs` is evaluated only once.

See the [language specification](#{page.doc_root}/#{site.urls.spec_relative}#arithmetic) for more details.

### Polymorphism

The `*=` operator is [polymorphic](#{page.doc_root}/reference/operator/operator-polymorphism).
The definition of the `*=` operator depends 
on the [`Numeric`](#{site.urls.apidoc_current}/interface_Numeric.html) interface.

## See also

* [arithmetic operators](#{page.doc_root}/#{site.urls.spec_relative}#arithmetic) in the 
  language specification
* [operator precedence](#{page.doc_root}/#{site.urls.spec_relative}#operatorprecedence) in the 
  language specification
* [Operator polymorphism](#{page.doc_root}/tour/language-module/#operator_polymorphism) 
  and 
  [Numeric operator semantics](#{page.doc_root}/tour/language-module/#numeric_operator_semantics) 
  in the Tour of Ceylon

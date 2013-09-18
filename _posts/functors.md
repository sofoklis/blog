title: Functors
date: 2013/04/07 3:45:00 -0800
tags: [{"name":"functor","id":125460785}, {"name":"map","id":125460786}, {"name":"category theory","id":125460786}]
author: Sofoklis Papasofokli
alias: /functors

A functor requires the following 2 properties:

1. A contructor or apply method which for any type A, we can construct a type
   in the new category T[A]
2. map method which given a transformed type T[A] and a function that
   transforms A=>B we can construct T[B]
   
Using these 2 properties we can tranform a type T[A] to a T[B] using the map method with the following steps:
1. use the A=>B function to transform the A type inside the T[A] into a B
2. use the contructor(1st property) to create a T[B] using the B from step 1.

The result is that we can have a transormation from T[A]=>T[B] using the above properties.


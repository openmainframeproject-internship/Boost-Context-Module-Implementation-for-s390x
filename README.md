# Implementation of Boost.Context for s390x Architecture

## Aim

The aim of the project was to implement the Context framework of the Boost C++
library on the s390x architecture. 

## Work Done

context module is now available on s390x.

There are many libraries which are directly  dependent on boot.context and are 
blocked from being available on the s390x due to the lack of `boost.context`.

The absence of this module blocks the following modules:

* boost.coroutine
* hhvm
* kicad

The implementation of this framework would now allow the blocked libraries to
run.

The link to the PR is https://github.com/boostorg/context/pull/117
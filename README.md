# Mu

The Mu language

## Overview

Mu is a new approach to language development. It builds on an emergent living breathing environment. Mu does not attempt to replicate 
the feature set of "programming" languages but instead attempts to define a more human way forward. Mu is not yet ready for real world 
consumption.

## Ideas

Mu is a new language we're hypothesising about which is built on the foundations of services 
rather than any sort of formally defined spec. It is firstly not a replacement for any 
existing programming language such as Go, java, ruby, python, etc and does not attempt to be 
comparable to current programming models.

The goal is to lay the foundation for an emergent language where the keywords are 
services and all we attempt to do is define a grammar to associate these services 
in a cohesive way that then lets us perform actions at a higher level.

## Design

The assumption is that we can steal from the likes of bash while creating something 
purely human readable or with a fixed type set for interop between services. We 
should also include the ability to save new programs as the aggregate of many 
others but in lazy loaded fashion as with haskell execution.

```
# a service call to the store
# [service] [method] [input] [value]
> store write foo bar

# retrieve the output
> store read foo

# storing the output of such a command
> save result = store read foo

# evaluating the output
> exec result

# passing the output to an input
> input result into broker publish values
```

## Potential

The longer term potential for such a language is that it becomes a higher level form of orchestration for services. 
At a given point when enough services have been written, they become motor functions capable of being combined 
to perform other forms of execution. Continuing to use existing programming languages to orchestrate these 
services becomes cumbersome and a dynamic language does not exist to perform operations on services.

By escaping the current programming boundaries we can elevate to a new intermediary representation that can 
either be leveraged by human beings more easily, spoken as commands or used for other purposes.

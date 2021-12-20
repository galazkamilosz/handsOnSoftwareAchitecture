# Chapter 2 - Packaging Code

## Contracts

A software contract is a formalized documentation of an interaction with a software component. It can be an interface, an API, a protocl. Contracts allow diverse unconnected components of a system to work together.

Key things of the atichitect is to ensure the following:
- contracts are durable and not reactive, and there is no change amplification, such that small requirement changes cause churn in the contract;
- contracts are versioned. Shoulb be backward compatible;
- contracts should include non-functional requirements, typically called service-level agreements.

## Pointer receivers
Used if either apply:
- you want to modify the receiver,
- struct is very large and deep copy is expensive,

Slices and maps act as references. Even passing them as value will allow mutation of the objects.
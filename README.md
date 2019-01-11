# Introduction

Overlays pattern is a generic concept for data composition.

The aim of this document is to explore and try to define generic set of rules
and attributes which such a pattern could provide.

# Properties

* Discoverability - Allow easy discoverability of the objects within pattern. This helps for adoption, reusability, user friendly etc.
* Identification - Allow to verify that we are talking about the same layer
* Versioning - Allow to verify the version of the layer
* Immutability - Allow to ensure that the layer won't change in the future
* Interoperability - Allow to reuse same layer independent from any concret implementation
* Decentralization - Allow to avoid vendor locking and to not relay on centralize repository

# Background

It seems that the concept of general overlays seems to be very interesting in
different spaces. The concept was born some time ago while we thought about new
modern file format which suppose to be compose out of different layers. Then the
idea was buried for some time and reborn again within Semantic WG in
Hyperledger where we started defining schema and overlays for decentralize
global storage.


# Overlays 
## Why we need it?

We don't know yet. But it is very interesting to evaluate possibility if
something like that could solve some problems.

Some potential problems which could be solved by this approach:
* Provide unify data language for decentralize economy including: data exchange, data storage, communication etc. 
* Allow to build global decentralize data storage for sociaty benefits
* Provide overall framework for dealing with data including consent, privacy, tracability etc.

We already started implementing this approach within schema and overlays concept in Semantic WG. 
The idea behind `Overlays` is to create unifiy notation for data which can be used in multiple cases:

* Data Vault - as a normalization solution, share and store data.
* Data capture - collecting data from different sources in standardize and reusable way
* File format - Multi layer file format which separate content, presentation layer and potential logic layer
* Verifiable credentials - for example as reusable schema with different encodings

We don't know yet if all those use cases are valid and/or if we should cover all of them or more. It seems that all of the have similar nature. Which could be described as follow:

* Static or dynamic base - the place where the base subject is (content of the file, schema base for data, data base model, protocol data description (schema) etc..)
* Layers - different type of layers from static through composed and ad-hoc layers. They can serve as a coloration, enriching or extending base without need to change it. 

## Example

### [Schema and Overlays](https://github.com/THCLab/schema-cake) - Data capture 
### File format

* Dynamic base - would be content which we are creating 
* Layers:
  * Subset overlay - could reduce the content within the document base on who is reading it. Show just brief description or hide technicalities. 
  * Information - annotation/comments or contextual information
  * Language - translations - same document supporting multiple language in the same time. 
  
### Verifaible credentials

* Static base - simple schema representing all attributes which are subject of VC
* Layers:
  * Information - annotation/comments or contextual information
  * Encoding - crypto material used for encoding (ZKP)
  * ...

# Why not to use?

* Why not use mixins?
* Why not use json-ld?
* Why not use xml/xlts?
* Why use it at all?

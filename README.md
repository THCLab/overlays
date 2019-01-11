# Introduction

Overlays pattern is a generic concept for data composition.

The aim of this document is to explore and try to define generic set of rules
and attributes which such a pattern could provide.

# Properties

* Discoverability
  Allow easy discoverability of the objects within pattern. This helps for adoption, reusability, user friendly etc.
* Identification

* Versioning
* Immutability
* Interoperability
* Decentralization

# Background

It seems that the concept of general overlays seems to be very interesting in
different spaces. The concept was born some time ago while we thought about new
modern file format which suppose to be compose out of different layers. Then the
idea was buried for some time and reborn again within Semantic WG in
Hyperledger where we started defining schema and overlays for decentralize
global storage.


# Why we need it?

We don't know yet. But it is very interesting to evaluate possibility if
something like that could sole some problems. We already started implementing
this approach within schema and overlays concept in Semantic WG. The idea is to
create unifiy data language which can be used in multiple cases:

* Data Vault - as a normalization solution, share and store data.
* Data capture - collecting data from different sources in standardize and reusable way
* File format - Multi layer file format which separate content, presentation layer and potential logic layer
* Verifiable credentials - for example as reusable schema with different encodings

# Why not to use?

Why not use mixins?
Why not use json-ld?
Why not use xml/xlts?
Why use it at all?

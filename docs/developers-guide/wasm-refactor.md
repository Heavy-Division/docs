# B78XH Web Assembly Refactor 

## Overview 

The Web Assembly (WASM) refactor consists of the overhaul of B78XH from a 
Javascript oriented framework to a WASM module.

## Background 
Support for [WASM Modules](https://docs.flightsimulator.com/html/Programming_Tools/WASM/WebAssembly.htm) 
is a relatively new feature for Microsoft Flight Simulator 2020. 

Moving forward, we're interested in harnessing the power of low level languages
such as C++ to improve the performance of the aircraft via finer control of program memory.

Prior to the refactor, the B78XH ran on a Javascript framework, which made 
development relatively easy with automatic [garbage collection](https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)) and
a web-ready interface.

WASM is what's known as a compilation target. That is, we don't actually write 
code in WASM, but in other languages like C++, which are then compiled to WASM, 
so that it can be run on a multitude of platforms and in a web application. 

The B78XH is split into two repositories: Our main [B78XH](https://github.com/Heavy-Division/B78XH)
aircraft where production deployments are released and users can continue to download
stable, development, and experimental versions. 

The second repository, [B78XH-wasm](https://github.com/Heavy-Division/B78XH-wasm)
is a C++ application which contains the source code for the systems, displays,
renderers, and an interface for interacting with the simulation API. 

When making changes or additions to this repository, the deployment to production
is a two-step process. First, we compile the WASM module from the WASM repository.
Second, the module is then output to the main repository under
`B78XH/SimObjects/Airplanes/Asobo_B787_10/panels`

Feel free to ask questions in our[Developer Support Channel](https://discord.com/channels/808476259016769546/984324843338104922) 
if you have any further questions or need assistance with a programming issue. 





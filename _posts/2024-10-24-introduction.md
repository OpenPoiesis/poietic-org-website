---
layout: post
title:  "Introduction"
date:   2024-10-24 12:45:00 +0200
categories: about
---


Hi there!

> "Look, it is already somewhat useable. You have been working on it for quite
some time, it would be a pity not to publish it".

– A good friend of mine pushed me recently.

I am releasing a preview of a hobby project of mine: **[Open Poiesis](https://github.com/openpoiesis/)** – building
blocks of a virtual laboratory for systems thinking.


## Overview

Intention of the Open Poiesis project is to create an open architecture for
a virtual laboratory for modelling, simulation and reasoning about systems.
Focus is on the modelling process, model reasoning, model composition and
sharing of reusable model fragments.

![Overview](/images/introduction-overview@2x.png)


This project is about _modelling the modelling_. Where the intended output is
an answer to the question:

> How a model of a modelling, simulation, reasoning and experimentation
process looks like?

The included collection of libraries and tools that are part of the project
are essential, yet they are not the primary goal. Their purpose is to reflect
and verify ideas about the architecture, structures, algorithms, interchange
formats and more. Learnings are captured as a systems architecture, which
is constantly evolving.

## Existing Sofware

As of the time of this post, the following components exist:

- [**Poietic Core**](https://github.com/OpenPoiesis/poietic-core):
  Swift package that provides basis for design,
  design objects, metamodel, changes, persistence, arithmetic
  expressions.
- [**Poietic Flows**](https://github.com/OpenPoiesis/poietic-flows):
  Swift package for [Stock and Flow](https://en.wikipedia.org/wiki/Stock_and_flow)
  modelling domain and simulator.
- [**Poietic Tool**](https://github.com/OpenPoiesis/poietic-tool):
  Command-line tool for editing and running Poietic models.
- [**Poietic Server**](https://github.com/OpenPoiesis/poietic-server):
  Makeshift localhost simulation server for running the _PoieticFlows_ models.

![Open Poiesis First Overview](/images/open_poiesis-overview@2x.png){:width="75%"}

The design is gradually being described in the 
[**Poietic Architecture**](https://github.com/OpenPoiesis/poietic-architecture)
repository.


The language of choice for the prototype implementation,
which might become referential, is [Swift](https://www.swift.org).


## Goals and Non-Goals

> Make people see and understand the systems of the nature and society and give
them the ability to collaboratively improve the seeing and the understanding.

To achieve that, this project is based on two inter-related foundations:
an _open architecture_ of a toolkit and an ecosystem of _model libraries_. To get
there, these are the goals:

1. Describe and make tools for seeing and understanding.
2. Help others to build similar tools.
3. Make sure that the tools that exist out there can exchange user created
   content.
4. Formalise model of models (metamodel) and make sure it is practical yet
   comprehensive, transparent yet easily processable.
5. Enable a way to share, compare and compose models.
6. Allow variety of opinions, scenarios and narratives to be present
   in an open ecosystem of the models.
7. Make sure that all of the above, including user's creations, is open and
   has assured continuity through formal specification.

I will write about the model library idea in more details later.

A wish: graphical interactive modelling applications (local-first).

See also: [Requirements](https://github.com/OpenPoiesis/poietic-architecture/blob/main/Drafts/Requirements.md).


### Non-Goals

1. Performance. At this stage, focusing on performance would get in
   the way of making the software understandable and it would make the
   software hard to evolve.
2. Development of modelling methodologies that are not based on graphs nor
   can be integrated in the graph structures.


## Next Steps

My personal focus, without specific time commitment is:

- Documenting what exists, describe technical debt
- Creating diagrams of data models, data flows and other relevant aspects
  of the software. (Populating the [architecture](https://github.com/OpenPoiesis/poietic-architecture) repository.)
- Bug-fixing what exists, no radical new features at the moment, except
  if needed for model examples.
- Create more models and examples. Add features, if necessary, to support
  those models. (Populating the [examples](https://github.com/OpenPoiesis/poietic-examples) repository.)
- Attempt to sketch a simple graphical modelling application (I am contemplating
  Godot).

I will be writing more about the project. Regularity is not assured. The 
upcoming posts that I have in mind:

- Current state of the software with focus on the technical debt and on
  what is wrong/not as I want it to be.
- Description of the data model, reasoning behind it and known issues.
- Detailed description of the Flows compilation process.


## Getting Involved

If you would like to to join me on the journey of _modelling the modelling_, 
_modelling the seeing_ and _modelling the understanding_, I would be more than
happy.

If you don't have an idea how, and if you are an engineer, the help I might need
right now is code review. I have been immersed in my own code for a significant
amount if time, that I am numb to many of the design decisions I made.

If you have some technical background, even playing with the toolkit and
giving me feedback about the experience will make me happy.

If you are not an engineer, giving me a model suggestion, if you have an existing
(stock and flow) model at hand, would benefit the project as well.

Or just give any constructive feedback, ask a question or propose a feature.

  
## Links and Further Reading

- Open Poiesis Umbrella: [github](https://github.com/openpoiesis/)
- Poietic Tool: [github](https://github.com/OpenPoiesis/poietic-tool)
- Poietic Flows: [github](https://github.com/OpenPoiesis/poietic-flows), [package documentation](https://openpoiesis.github.io/poietic-flows/documentation/poieticflows/)
- Poietic Core: [github](https://github.com/OpenPoiesis/poietic-core), [package documentation](https://openpoiesis.github.io/poietic-core/documentation/poieticcore/)
- Poietic Server: [github](https://github.com/OpenPoiesis/poietic-servera)
- Poietic Architecture: [github](https://github.com/OpenPoiesis/poietic-architecture)


## Closing Remarks

Why I am doing it? because I enjoy it and I feel that it might be useful.
That is it.

This project is a hobby project that I am sharing with whoever might like it.
I hope it might be at least somewhat useful for others. Even if for nothing
else, at least the software evolution story telling and the diagrams might
inspire someone.

Cheers,

Stefan

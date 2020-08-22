# Ecovillage Resource Management Spec

* [Introduction](#introduction)
* [Resources](#resources)
* [I/O](#io)
* [Goals](#goals)
* [Principles](#principles)

## Introduction
Specification of a program to manage the resources of a ecovillage in a cyclical closed-loop system.

Village resources are defined as:

|Resource|Unit|
|--------|----|
|💧 Water|Liter|
|🌱 Food|Joule|
|⚡ Energy|Joule|

Village resources are provided by **village components**, primarily:

* Houses
* Shared Infrastructure

Each individual house in the village can be thought of as a sub-component to the overall system with resources managed by [House Resource Management Module](./house-resource-management-spec.md).

Shared infrastructure components would vary from village-to-village based on unique needs, desires, and interests, but may consist of:

* Electrical vehicles and / or charging station
* A "common house", community spaces, or community center
* Centralized village power and electrical grid (may feed into wider municipal grid)
* Plumbing and waste-water treatment center (performed ecologically using centralized bio-gas digestion)

## Resources
A **resource** is defined as something humans need to live. A distinction is made between three kinds of resources: *primary*, *secondary*, and *tertiary* resources.

A **primary resource** is defined as a non-negotiable human requirement for survival, and includes (in order of importance):

1. 💧 Water
2. 🌱 Food

A **secondary resource** is defined as a non-negotiable requirement for survival because a human depends upon it for the attainment of a *primary resource*.

Examples may include:

* 🏠 Shelter, when you depend upon your shelter for collecting, storing, and purifying rain-water
* ⚡ Energy, when depend upon energy for heating a greenhouse in winter for growing food.

A **tertiary resource** is defined as a negotiable requirement for a desired standard of living. For example, a desired *modern* standard of living might require the following tertiary resources:

* 🌐 Internet
* 🚗 Transportation

Secondary and tertiary resources should be configurable to meet the needs of different villages and people.

## I/O
A village, as well as village components can be defined in terms of I/O, or **inputs** and **outputs**.

This view lends the village and individual components to modeling by [material balance equations](https://en.wikipedia.org/wiki/Mass_balance).

### Inputs
Inputs result in **resource generation**.

Some inputs are universal, such as sunlight ☀️. Although, the amount of that input will vary based on location and may be insufficient for requisite resource generation.

Other inputs are unique to a geographic location or bio-region.

For example, in the mid-west of the United States, an input to a house may be **rain-water**.

The house would have a rain-water harvesting sub-component that adapts the **input** of rain-water to the **resource** of water.

Other geographic locations may have different inputs that lead to water resource generation such as ground-water, salt-water, river-water, glacier-water, or spring-water -- and each water input would need a different sub-component to adapt it to a water resource ready for human consumption.

### Outputs
* Human waste 💩
* are there others we care to model?

## Goals
* Assist in village planning.
* Allow village simulation.
* Assist in automation of resource management to free-up human time.
* Assist in village improvements, resource attainment efficiency, policy, and decision-making.
* Applicable to existing ecovillages such as [Dancing Rabbit Ecovillage](https://www.dancingrabbit.org/).

## Principles
The following principles should be observed by the system and guide overall design and decision making.

Each principle is not mutually exclusive, and may tie into other principles.

* **Universal**
  * Applicable to any geographic location or unique bio-regions.
* **Accessible**
  * Available to any person regardless of disability: deaf, blind, vision or hearing impaired, amputee.
* **Low Cost**
  * Financial cost to individuals should be minimized.
* **Global**
  * Applicable to any person, culture, or language in the world.
* **Open Source**
  * The code should be freely available and observe the four freedoms of open-source software.

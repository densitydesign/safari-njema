---
title: Title
permalink: "/question2/"
number: 2
layout: visualization
type: visualization
department: Department of Mathematics, Department of Design
authors: Anna Calissano, Paola Riva, Elena Castelli, Andrea Benedetti (design and
  development), Tommaso Elli (development)
data: https://www.facebook.it/
data-description: Brief description of the dataset.
---

As a first experiment, a small map-athon was organized in Maputo within the research team to have a first hand experience of the mobility systems in the city. For the Mobility Week organized in September, members of the research teams explored the city with formal and para-transit transportations systems through the whole week, gathering data both from the platforms provided by the research partners, and from a simple web app developed for this purpose.

![image-title-here]({{ "/assets/images/map-athon-mockup.jpg" | relative_url }})

## Experiment methodology
1. Researchers explored the city using four different kinds of transportation methods: Machinbombo, taxi, Xopela, private car, walk and Chapas.
2. Upon starting and ending, they logged their position through a [web app](https://densitydesign.github.io/map-uto/) developed inside the research team. This allowed to have precise starting and ending point for the trip.
3. These points were then interpolated to infer the trip inside the city. They were finally categorized by transportation method and who initiated the trip[^1].

## Future steps
The aim of this experiment, besides having a trace of the first hand experience that the research team had in Maputo, was to build a first framework to be replicated by other participants on larger scale.
The usage of a web app helped to have a simple data format, but it also introduced a number of complications related to the use of web technologies that often inhibit geolocation of mobile devices for prolonged online sessions.
Avoiding the use of web technologies could improve this aspect of the data gathering, and would make it more robust.

[^1]: It's also possible to see singular complete trips from each participant in the small maps below. These trips are cumulative after one week of travel.

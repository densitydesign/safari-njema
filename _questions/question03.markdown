---
title: Request and Offer in Public Transport System
permalink: "/request/"
number: 3
layout: output
type: post
sources:
- name: Trajectories
- name: Origin Destination
---

In the mobility setting of Maputo area, measuring mobility through GPS data can have a two side effect. On one side, local transport authorities can use the analysis results to better map and optimize the offer of public transport system. On the other side, citizens can also access to more informative description of the public transport system. Builting Origin Destination Matrices is a first step towards the measurement and the understanding of the phenomenon.

## Objectives
> 1. Building Origin Destination Matrices

In the context of mobility, an accurate census data with high sample coverage  could not be enough for the analysis of a dynamic phenomenon such as urban mobility. To map citizens’ movement with GPS traces, we create a set of Origin Destination matrices describing the hourly fluxes between morphological areas within the city. Origin Destination matrices are a standard data format for the analysis of urban mobility and they are usually acquired by surveys combined with physical models. In the recent years, the usage of GPS traces to build Origin Destination matrices has become more and more common in the literature. Given a set of Origin Destination matrices, the analysis can focus on:
- Finding Attracting Areas in different time of the day
- Finding Isolated Areas in different time of the day

These two outputs can help decision making in improving consciously the offer based on the real time measured request.

## Activities
### Trajectories building
Given a set of localization in time, the first step is to identify if a point belongs to a trajectory or if it is a stationary point. To do so, the difference in time and space between observation is computed, setting a threshold to define moving and stopping points. Among the stopping points, some of them represent the end of a trajectories while others represent a waiting point (a traffic light, a bus stop). To discern between these two different stationary points, a spatio-temporal criterion has been applied. The city has been divided in different areas. In some area, the stopping point with a time difference of less than 30 minutes are considered as end of the trajectories. In other areas, the threshold is set to 60 minutes. Those areas where the tolerance is higher are the one close to Chapas stops or stration, bus terminals, informal markets etc.. Once all the points have been assigned to either a trajectory or a stopping point, the datasets results of a set of trajectories evolving over time and space.

### Origin Destination Matrices Building
Given a set of trajectories obtained by GPS traces data preprocessing, we aggregate them into hourly origin destination matrices. The Maputo Metropolitan Area has been divided into the morphological areas described in output - possiamo fare riferimento con link all’output 2?. The origin destination matrices are  a network where every node is a morphological area and every edge between two areas count the number of trajectories starting in one area and ending in the other area. The edge weight correspond to the number of trajectories leaving within a certain hour.

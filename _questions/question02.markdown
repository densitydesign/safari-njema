---
title: Accessibility, equity and social exclusion
permalink: "/accessibility/"
number: 2
layout: output
type: post
expertise:
- Data analysis
- Data retrieval
- GIS modelling
- Urban analysis
sources:
- name: Health facilities
  link: https://www.mozgis.gov.mz/portal/home/item.html?id=24b14545ee6d4e758066e509f546ab1d
  description: Data are provided by the official GIS portal of the Mozambican Ministry
    of Transport.
- name: High Resolution Settlement Layer (HRSL)
  link: https://google.com
  description: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt
- name: OSM Road Network
  link: https://www.openstreetmap.org
  description: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt
- name: Financial services (POS, ATM, Banks, Money exchange)
  link: https://www.mozgis.gov.mz/portal/home/item.html?id=93c32bb32cad4e9b84b0123695cdc376
  description: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt
- name: Education system
  link: https://www.google.com/maps/
- name: Google Earth Imagery
  link: https://www.google.it/intl/it/earth/index.html
diagram: "/assets/images/diagram-02.png"
---

## Objectives
> 1. Mapping poverty rate considering the level of accessibility
2. Methodology to calculate accessibility indicator
3. Analyse paratransit mobility and formal public transportation. Consider both during planning analysis.
4. Identify low connected areas and lack of public transport or paratransit mobility.
5. Build GPS model - data disclosure

Despite the significant growth of Mozambique since 1993, in this country more than half of the population still lives below the poverty line. The poverty reduction better performs in cities than in rural areas and in Mozambique the main urban growth happened in Greater Maputo Area. The rapid growth of the capital city involves negative externalities such as new urban poor, gentrification and underserved neighbourhoods.
The output attempt to measure the wealth and map the poverty in the Greater Maputo Area. Give a spatial dimension to this phenomenon allow to drive policies and perform services and new infrastructures.
The definition of wealth (or poverty) is generic and there are many variables that contribute to determine its value. From the literature review we identify key factors that influence wealth in Greater Maputo Area.

- access to drinking water at home
- access to information and communication technology
- access to public transport
- access to CBD (Central Business District)
- access to health facilities
- access to education system
- access to real estate market (affordable houses)
- having a permanent source of income or savings
- house construction material
- adequate sanitation at home
- source of reliable energy
- building density
- infrastructure density
- presence of formal / Informal business and jobs

Some of the items in the list concern a place-based accessibility. This is another generic term. Recent researches inspect this kind of accessibility and in many cases show a strong correlation between poverty reduction and access to basic services and urban infrastructure. In particular, the analysis of accessibility in low and middle-income countries point out the primary role of public transport in the reduction of urban inequality. Considerable number of people move and commute by public transport in Greater Maputo Area (%) and just a minority is car owner (increasing number).
“Constrained accessibility can result in higher rates of jobs informality. Reduce informality can be a target for well-designed transport policies.”
“Difficult access to formal jobs for the lower-income population.”
The relation between public transport and formal jobs emerge also comparing bus stops and financial services (POS, ATM and banks). Financial services identify presence of formal commercial and economic activities, most of them fall within 250 m from a stop.
Therefore, measure accessibility for the listed factors and considering public transport, means point out segregation areas, where there is a lack of services and a significant distance from them. These areas are unequal, people who live there have difficulties to access to job opportunities, there is a high rate of unemployment and informal employment and a lower educational level. The literature proves that all these social costs are also related to public transport equity and efficiency.
Define where these areas are located will help to define policies and focus areas for investments and public interventions. Equity, inclusion, segregation and wealth can be analysed measuring accessibility to the following factors by public transport.

- accessibility to health system
- accessibility to education system
- accessibility to CBD (Central Business District)
- accessibility to public transport
- accessibility to water sources
- presence of financial services

Until now the attempt to map the poverty in Maputo consider census data that are aggregated to the district or province level. These data are not relevant due to their poor detail, therefore the indicator have been calculated at the neighbour level.

## Activities
### Accessibility to health system
The access to healthcare facilities is crucial and has a strong impact on people and their wealth. To allow everyone equal access, it is necessary that health facilities are well distributed. The World Bank report on Maputo urban poverty and inclusive growth, estimates that “the number of poor households with no access to health facilities within 2km is three time as high as for non poor households”. The walking distance to a health facility is crucial, especially for poor people that do not own a car. The poor population reaches these facilities on foot, for this reason it is necessary to consider both the walking distance and the level of the sanitary structure that can be reached. To calculate this indicator, we considered the isochrones generated by each health facilities and their level, which is based on the available care services. The indicator is applied to morphological areas which identified a detailed and homogeneous subdivision of the metropolitan area, smaller than existing administrative areas (district or bairros).

*Activities: Isochrones, Morphological areas*

![]({{ 'assets/images/question02/1.png' | relative_url }})

### Accessibility to education system
The walking distance and the level of the school considered are factors even more relevant than for the health system. In order to support school attendance, especially primary and secondary schools, these facilities must be easily accessible on foot by students. In the poorest areas it is crucial due to the high risk of dropping out of school. World Bank reports on Maputo show the correlation between poverty and greater distance from primary and secondary schools. The same indicator was created analysing international schools and universities, in these cases walking distance is less relevant, while high accessibility by public transport is more relevant.

*Activities: Isochrones, Morphological areas*

![]({{ 'assets/images/question02/2.png' | relative_url }})

### Accessibility to public transport stops
Walking is the main travel mode in Maputo, especially poor people used to travel long distances on foot to reach their destination, they do not own a car and they save money of public transport tickets.
However certain travels are too long for walking. Public transport is essential for poor, commuting distance is often a key factor for wealth. Recent resources demonstrate correlation between mode of transport and access to formal job opportunities.
Walking and public transport movements are often integrated, most of the people used to travel long distances to reach bus stops.
This indicator analyses accessibility to public transport stops, considering their walking distance from the trip origin. The weight of public transport is relevant in Maputo, approximately 60% of all non-walking trips were made by chapas and 17% by conventional buses.

*Activities: Isochrones, Morphological areas, Mapathon, Public transport analysis*

![]({{ 'assets/images/question02/3.png' | relative_url }})

### Accessibility to CBD
In the Central Business District there is a high density of services and the main economic and commercial activities are concentrated there. Access to this place determines social inclusion, mainly because of the formal job opportunities are generated there. Several research studies have recently analysed the benefits and issues triggered by accessibility to CBD in low and middle-income countries main cities. Access to the CBD must be as fair as possible and public transport has a primary role in this sense. Public transport guarantees connection between CBD and periphery, which otherwise would be excluded from opportunities concentrated in the city center, especially by those who do not own the car. The indicator is affected both by the distance from public transport stops, and by the direction and the route of the individual lines that pass through those stops. For each area has been calculated the connection with every single public transport line (Mapathon 2019). For each public transport line has been calculated its connection with CBD. Then, travel times along the line and stop waiting times have been considered in processing the actual time taken to reach the CBD.

*Activities: Isochrones, Morphological areas, Accessibility to public transport stops, Public transport analysis, OD Matrices, OD Matrices with time, Bus stops waiting times*

![]({{ 'assets/images/question02/4.png' | relative_url }})

### Presence of financial services
Financial services such as POS, ATM and banks indicates where formal activities are concentrated. The densities of these services confirm the presence of commercial and economic formal activities, but not the informal business. The difference between formal and informal activities and jobs is crucial in Maputo and recent researches address the topic, that has also strong relation with accessibility and public transportation. The density of financial services is particularly high in the CBD and along the main road axes, also seat for public transport lines. In the Greater Maputo area, 53% of all the POS are located within 150 meters from a bus stop, 75% within 250 meters and the percentages increase considering ATM, banks or money exchanges. Financial services and formal activities are related to public transport and they are concentrated in the inner city. They are sources of formal jobs opportunities and wealth. To calculate this indicator the presence of financial services within 250m was considered.

*Activities: Morphological areas*


### Accessibility to water sources
Strong disparity between population living in CBD and the periphery regards the access to water sources. In 2013, only CBD inhabitants have water access at homes, while all the others less than 10% access to drinking water this way. “A majority of residents instead rely on water for drinking either from piped water outside housing or standpipes, private or public”. Strong disparities also regard the population that has direct access to sanitations (bathroom, biological pits and sewers) as well concentrated in the city center. Unfortunately, there are no recent attempts to map those services, which are very useful for providing an indicator of poverty. 2008 data have been used to calculate the indicator, based mainly on the presence of water pipes and boreholes.

*Activities: Morphological areas*

### Isochrone
The isochrone represents an area within which the desired destination is reachable in a certain time. Through the network analysis, the isochrones were generated for each point of interest object of the analysis. To perform this analysis has been considered walking distance and time threshold of five minutes. Over thirty minutes walking distance, to avoid any problems related to the road network, the isochrones were considered equal to a buffer of about 416 meters (five minutes walking at 5 km/h). Each point of interest is associated with 9 isochrones and the most external one represents the distance that can be covered in 45 minutes walking.
Morphological areas
The territorial units to which this indicator has been applied is represented by homogeneous morphological areas. These areas have been built for the Safari project, due to the absence of a suitable administrative level for the analysis. Other indicators are also applied to these areas; they provide basic support for various activities in order to make the results comparable.

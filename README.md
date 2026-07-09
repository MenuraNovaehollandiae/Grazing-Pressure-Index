# Living Landscape Grazing Pressure Index

This repository contains an interactive web map showing a grazing pressure index across the Living Landscape study region in the South Australian mallee.

The grazing pressure index was derived from the spatial distribution and persistence of pastoral dams detected using Sentinel-2 remote sensing. Artificial water points were treated as sources of grazing pressure, with grazing pressure assumed to decline with distance from each dam and to increase with the persistence of standing water.

Higher values indicate areas with greater inferred livestock grazing pressure associated with more persistent or nearby artificial water sources. Lower values indicate areas farther from persistent water points, or areas associated with less persistent or decommissioned dams.

## View the map

The interactive map can be viewed here:

[Living Landscape grazing pressure index map](https://menuranovaehollandiae.github.io/Grazing-Pressure-Index/)

## About the grazing pressure index

Artificial water points can concentrate livestock activity in semi-arid rangelands, creating gradients of grazing pressure that generally decline with distance from water. This map represents a continuous spatial index of inferred grazing pressure associated with pastoral dams across the Living Landscape study region.

The index was developed using:

- mapped pastoral dam locations;
- remote-sensing estimates of water persistence;
- information on dam decommissioning where available;
- a distance-decay model of grazing pressure away from water points.

For each dam, water availability was estimated as the proportion of the study period during which standing water was detected. For decommissioned dams, this value was reduced using a recovery multiplier based on the number of years since decommissioning and an assumed 30-year recovery timeframe.

Dam-specific grazing-pressure surfaces were then generated using an exponential distance-decay function, with grazing pressure highest at the dam and declining with distance. Individual dam surfaces were combined to produce a continuous landscape-scale grazing pressure index.

## Interpreting the map

The map shows relative grazing pressure, not directly observed vegetation condition.

Darker red areas indicate higher inferred grazing pressure, usually associated with more persistent or nearby artificial water points. Pale areas indicate lower inferred grazing pressure, generally farther from persistent pastoral water sources.

The map should be interpreted as a broad-scale decision-support layer and used alongside field observations, local ecological knowledge, management history, seasonal conditions and the limitations of remotely sensed water detection.

Factors not fully captured in the index may also influence vegetation condition, including:

- rainfall history;
- soil type;
- fire history;
- stocking history;
- rabbits, kangaroos and feral herbivores;
- land-use history;
- weed invasion;
- restoration or dam decommissioning activities.

## Relationship to other Living Landscape map products

The grazing pressure index was developed as an input to broader Living Landscape condition-state mapping. In related workflows, grazing pressure was used to inform interpretation of understorey condition and likely grazing-related modification.

Related map products include:

- [Living Landscape mallee vegetation-type map](https://menuranovaehollandiae.github.io/Mallee-vegetation-types/)
- [Living Landscape condition-state maps](https://menuranovaehollandiae.github.io/Living-Landscape-condition-states/)
- [Safeguarding mallee birds — habitat suitability maps](https://menuranovaehollandiae.github.io/Safeguarding-mallee-birds---habitat-suitability-maps/)

## Repository contents

This repository includes:

- `index.html` — landing page for the web map;
- `about.html` — background information and methods summary;
- `GPI/` — interactive qgis2web/Leaflet map files;
- `images/` — supporting images and logos.

## Suggested citation

Maisey, A. C. & Radford, J. Q. 2026. *Living Landscape grazing pressure index map*. Interactive web map. GitHub repository.

Update this citation with a DOI if one becomes available.

## Acknowledgement

This project was supported by funding from the Australian Government’s National Environmental Science Program through the Resilient Landscapes Hub.

We acknowledge the Traditional Owners of Country throughout Australia and their continuing connection to land, sea and community, and pay our respects to Elders past and present.

## Licence

Unless otherwise stated, written content and map outputs in this repository are provided under a Creative Commons Attribution 4.0 International licence.

Basemap imagery and third-party spatial data remain subject to their original licences and terms of use.

# Urban Accessibility Analysis — ZM Guadalajara

Pedestrian accessibility analysis to primary schools in the Guadalajara 
Metropolitan Area (Mexico), using real road network data and official 
school registry.

## What this analysis does

- Downloads the pedestrian street network of the ZM Guadalajara 
  (166,528 nodes) from OpenStreetMap via OSMnx
- Loads 1,485 primary schools from INEGI DENUE 2025
- Computes 15-minute walking coverage from every school simultaneously 
  using Multi-Source Dijkstra
- Maps which areas of the city have walkable access to a primary school 
  and which do not

## Key finding

**75.1% of the metropolitan network** is within 15 minutes walking of a 
primary school. The remaining 24.9% is concentrated in peripheral areas 
of Zapopan, Tlajomulco, and Tonalá — zones of rapid urban growth where 
residential expansion has outpaced educational infrastructure.

## Stack

- Python · OSMnx · GeoPandas · NetworkX · INEGI DENUE · OpenStreetMap

## Data sources

- Street network: OpenStreetMap via OSMnx
- Schools: INEGI DENUE 2025 (SCIAN codes 611121, 611122)

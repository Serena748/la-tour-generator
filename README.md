# LA Tour Generator (Originally: Bruin Tours) 
LA text-based tour generator that loads and indexes OSM data to build a turn-by-turn navigation system using hash tables and the A* algorithm.

Geospatial data from Open Street Maps (OSM): https://www.openstreetmap.org

Important classes:

- MyMap: implement a map-like structure using a binary search tree.
- MapLoaderImpl: load and parse OSM data into StreetSegments
= AttractionMapperImpl: input(attraction name) -> output(attraction location)
- SegmentMapperImpl: input(location:lat,long) -> output(list)
- NavImpl: input(start attraction, end attraction) -> output(list)

I used the A* search algorithm to find optimal path from start to end attraction. The Euclidean distance was used as the heuristic.


# Geometry Exercises
---

Here\'s a reminder of all the functions we have seen so far. They should
be useful for the exercises!

-   `sum(expression)`{.interpreted-text role="command"} aggregate to
    return a sum for a set of records
-   `count(expression)`{.interpreted-text role="command"} aggregate to
    return the size of a set of records
-   `ST_GeometryType(geometry)`{.interpreted-text role="command"}
    returns the type of the geometry
-   `ST_NDims(geometry)`{.interpreted-text role="command"} returns the
    number of dimensions of the geometry
-   `ST_SRID(geometry)`{.interpreted-text role="command"} returns the
    spatial reference identifier number of the geometry
-   `ST_X(point)`{.interpreted-text role="command"} returns the X
    ordinate
-   `ST_Y(point)`{.interpreted-text role="command"} returns the Y
    ordinate
-   `ST_Length(linestring)`{.interpreted-text role="command"} returns
    the length of the linestring
-   `ST_StartPoint(geometry)`{.interpreted-text role="command"} returns
    the first coordinate as a point
-   `ST_EndPoint(geometry)`{.interpreted-text role="command"} returns
    the last coordinate as a point
-   `ST_NPoints(geometry)`{.interpreted-text role="command"} returns the
    number of coordinates in the linestring
-   `ST_Area(geometry)`{.interpreted-text role="command"} returns the
    area of the polygons
-   `ST_NRings(geometry)`{.interpreted-text role="command"} returns the
    number of rings (usually 1, more if there are holes)
-   `ST_ExteriorRing(polygon)`{.interpreted-text role="command"} returns
    the outer ring as a linestring
-   `ST_InteriorRingN(polygon, integer)`{.interpreted-text
    role="command"} returns a specified interior ring as a linestring
-   `ST_Perimeter(geometry)`{.interpreted-text role="command"} returns
    the length of all the rings
-   `ST_NumGeometries(multi/geomcollection)`{.interpreted-text
    role="command"} returns the number of parts in the collection
-   `ST_GeometryN(geometry, integer)`{.interpreted-text role="command"}
    returns the specified part of the collection
-   `ST_GeomFromText(text)`{.interpreted-text role="command"} returns
    `geometry`
-   `ST_AsText(geometry)`{.interpreted-text role="command"} returns WKT
    `text`
-   `ST_AsEWKT(geometry)`{.interpreted-text role="command"} returns EWKT
    `text`
-   `ST_GeomFromWKB(bytea)`{.interpreted-text role="command"} returns
    `geometry`
-   `ST_AsBinary(geometry)`{.interpreted-text role="command"} returns
    WKB `bytea`
-   `ST_AsEWKB(geometry)`{.interpreted-text role="command"} returns EWKB
    `bytea`
-   `ST_GeomFromGML(text)`{.interpreted-text role="command"} returns
    `geometry`
-   `ST_AsGML(geometry)`{.interpreted-text role="command"} returns GML
    `text`
-   `ST_GeomFromKML(text)`{.interpreted-text role="command"} returns
    `geometry`
-   `ST_AsKML(geometry)`{.interpreted-text role="command"} returns KML
    `text`
-   `ST_AsGeoJSON(geometry)`{.interpreted-text role="command"} returns
    JSON `text`
-   `ST_AsSVG(geometry)`{.interpreted-text role="command"} returns SVG
    `text`

Also remember the tables we have available:

-   `nyc_census_blocks`
    -   blkid, popn_total, boroname, geom
-   `nyc_streets`
    -   name, type, geom
-   `nyc_subway_stations`
    -   name, geom
-   `nyc_neighborhoods`
    -   name, boroname, geom

# Exercises

-   **What is the area of the \'West Village\' neighborhood?** (Hint: The area is given in square meters. To get an area in hectares, divide by 10000. To get an area in acres, divide by 4047.)
-   **What is the geometry type of 'Pelham St'? The length?**

-   **What is the GeoJSON representation of the \'Broad St\' subway
    station?**

-   **What is the total length of streets (in kilometers) in New York
    City?** (Hint: The units of measurement of the spatial data are
    meters, there are 1000 meters in a kilometer.)

-   **What is the area of Manhattan in acres?** (Hint: both
    `nyc_census_blocks` and `nyc_neighborhoods` have a `boroname` in
    them.)

-   **What is the most westerly subway station?**

-   **How long is \'Columbus Cir\' (aka Columbus Circle)?**

-   **What is the length of streets in New York City, summarized by
    type?**



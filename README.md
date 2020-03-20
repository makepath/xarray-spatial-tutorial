Xarray-Spatial Tutorial
--------------

### rough outline

1. Introduction to video playlist

# FLIP TO MAKEPATH HOMEPAGE
Hi, I'm Brendan from makepath.

At makepath, we love open source Python.

# FLIP TO GITHUB
Makepath's most recent open source project is a suite of analysis tools called Xarray-Spatial. Its built on top the scientific Python stack, and is fully open souce with an MIT license.

The following content is a look at the major features inside of Xarray-Spatial through their use in common spatial analyses.

Xarray-Spatial wouldn't be possible without a list of people too long to mention.  As an organization, Anaconda has spearheaded building high quality, open source tools for the Python community and their partnership with makepath made Xarray-Spatial possible.

Xarray-Spatial provides a set of raster analysis tools with names common to GIS professionals.

By raster analysis, I mean analysis based on regularlly gridded datasets which many times are georeferenced with a explicit x, y origin and extent in latitude and longitude (or the units of the map projection)...don't worry, we won't be going too deep into map projections.

So basically, raster is another name image, and we are talking about doing analysis on a huge numbers of pixels which are associate with real-world locations.

These images can come from satellites, planes, drones, or they can represent continuous phenoma like rainfall, elevation, or distance to the nearest Buckies gas station.

Common raster formats include JPG and PNG but we will mostly look at the GeoTIFF format for loading data and persisting our results. 

Tools available within Xarray-Spatial will be helpful for people working with Digital Elevation Models (DEM)

Some of these surface analysis tools include:
  - Slope
  - Aspect
  - Curvature
  - Hillshade
  - Bump Mapping
  - Procedural Terrain Generation
  - Focal Statistics

Xarray-Spatial also contains routines for:
- classification of vegetation with satellite imagery (NDVI)
- Xarray-Spatial has powerful zonal analysis tools. An example of this sort of analysis would be calculating rainfall for a given county or calculating average distance to public transportation based on school district.
- Xarray-spatial has support for viewshed which calculates line-of-sight for an observer. 
- Xarray-spatial can also create tilesets for diseminating data through web mapping applications.

# FLIP TO DEPENDENCY GRAPH
Xarray-Spatial exists within an ecosystem of tools and has a few dependence including Xarray, Datashader, Dask, Numba, and Pandas. We'll cover each of these libraries in in subsequent videos.

Xarray adds labeled dimensions to numpy arrays, and is the xarray.DataArray is the core data structure Xarray-Spatial is based on.

Datashader is a general purpose rasterization pipeline to efficiently and accurately turn huge datasets into beautiful images.

Dask helps Xarray-Spatial scale horizontally to many threads, cores, and clusters.

Numba helps Xarray-Spatial scale vertically by just-in-time compiling spatial algorithms for fast execution.

We will be talking more about Xarray spatial and these dependencies in the coming videos.

In the next video, we'll see how to get setup with Xarray-Spatial and a basic Jupyter notebook environment to run the user guide.

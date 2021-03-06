Making maps with ggvis with some examples showing:

-   basic map creation
-   basic maps with points/labels
-   dynamic choropleths (with various scales)
-   applying projections and custom color fills
-   apply projections and projecting coordinates for plotting

The `R` file lets you play interactively with each example. The `Rmd` file shows what the plots look like in static format. The Shiny code (`ui.R`, `server.R`) provides an interactive version in a Shiny app context.

The `Rmd` has also been published on [RPubs](http://rpubs.com/hrbrmstr/ggvis-maps) and there's a [blog post](http://rud.is/b/2014/12/29/making-static-interactive-maps-with-ggvis-using-ggvis-maps-wshiny/) with slightly more expository than the code.

One of the caveats with `ggvis` is that you need an online context for interactively (making things like interactive choropleths useless without such a context). You'd need to account for this in the `Rmd` by setting up a faux-facet series for the maps, either with a `<table>` or `<div>` grid.

=======================

-   Maine GeoJSON from `http://catalog.opendata.city/hu/dataset/maine-counties-polygon/resource/ee88d12c-a832-4e4f-a93c-dfd693694688`
-   Maine crime data from `http://muskie.usm.maine.edu/justiceresearch/datacenter.html`
-   Maine population data from `http://www.maine.gov/economist/census/`
-   US GeoJSON from `http://eric.clst.org/Stuff/USGeoJSON`
-   Drought data from `http://droughtmonitor.unl.edu/MapsAndData/GISData.aspx`
-   World GeoJSON from `http://www.naturalearthdata.com/downloads/`
-   Launch sites `kml` from `http://en.wikipedia.org/wiki/List_of_rocket_launch_sites`

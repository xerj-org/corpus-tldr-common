# gdal_contour

> Create contour lines and polygons from a digital elevation model.
> More information: <https://gdal.org/en/stable/programs/gdal_contour.html>.

- Create a vector dataset with contour lines spread over a 100-meter interval while attributing the elevation property as "ele":

`gdal_contour -a {{ele}} -i {{100.0}} {{path/to/input.tif}} {{path/to/output.gpkg}}`

- Create a vector dataset with polygons spread over a 100-meter interval:

`gdal_contour -i {{100.0}} -p {{path/to/input.tif}} {{path/to/output.gpkg}}`

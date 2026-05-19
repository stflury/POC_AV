# TODO

In this POC, swisstopo products will be converted into GeoParquet files. These will be described in the following sections. After importing the data into GeoParquet, it will be filtered and exported via a DuckDB query. A GeoJSON file will be generated as the POC export format. 
The data model in the Parquet file should correspond to the product data model that serves as the source.
The following scripts should be created for each dataset
- Create the GeoParquet file with the schema
- Load the data from Stac to the GeoParquet
The selection area for the POC is "Glarus Süd", as defined in the official cadastral boundaries dataset.
source: https://www.geodienste.ch/downloads/interlis/av/GL/av_GL_lv95.zip (TABL Gemeindegrenze_Geometrie)
If the POC is successful, modules for Python and other development environments may follow, as well as support for additional formats such as Interlis. 
Also try using ogr2ogr to read the data from Stac in Interlis.
Also try to read the selection polygon out of the Interlisfile (TABL Gemeindegrenze_Geometrie)

## Planimetric control Points LFP1 (National Survey)
https://data.geo.admin.ch/ch.swisstopo.fixpunkte-lfp1/fixpunkte-lfp1/fixpunkte-lfp1_2056_5728.gdb.zip

## Height control points HFP1 (National Survey)
https://data.geo.admin.ch/ch.swisstopo.fixpunkte-hfp1/fixpunkte-hfp1/fixpunkte-hfp1_2056_5728.gdb.zip

## Official index of cities and towns including postal codes and perimeter
https://data.geo.admin.ch/ch.swisstopo-vd.ortschaftenverzeichnis_plz/ortschaftenverzeichnis_plz/ortschaftenverzeichnis_plz_2056.gdb.zip

## Territorial Limit NS
https://data.geo.admin.ch/ch.swisstopo.hoheitsgrenze-landesvermessung/hoheitsgrenze-landesvermessung/hoheitsgrenze-landesvermessung_2056.gdb.zip

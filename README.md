# csueb_projects, currently showing:

Project #1 for STAT 6610
  (by John King)

Data taken from the China Labor Bulletin (http://www.clb.org.hk/en/).

Map data from 

http://www.naturalearthdata.com/http//www.naturalearthdata.com/download/10m/cultural/ne_10m_admin_1_states_provinces_lakes.zip"

(I found it via https://github.com/clemsos/d3-china-map):

To change the .shp file we need a tool.  I used ogr2ogr, part of the GDAL toolkit.  See http://www.gdal.org/ogr2ogr.html and for a mac download, http://www.kyngchaos.com/software:frameworks .

Make the json file:

~/gdal/ogr2ogr.py -f GeoJSON -where "gu_A3 IN ('CHN')" zh-mainland-provinces.json ne_10m_admin_1_states_provinces_lakes.shp

The rest is in the Javascript/d3 file.

# csueb_projects

#### Q1: What is the URL of the WMS GetCapabilities request?

##### A: *http://localhost:8080/geoserver/wms?request=getCapabilities*

#### Q2: What is the URL of the WFS GetCapabilities request?

##### A: *http://localhost:8080/geoserver/wfs*

#### Q3: Submit a screenshot of your updated WFS Layer Preview

##### A: _Lab Screenshot 1.png_

#### Q4: What does drawing order refer to? Which layer goes on `top`, the first or the last layer in the list?

##### A: *The order the layers are drawn in. The last layer drawn is on top.*

#### Q5: Submit a screenshot of the Layer Preview of the Spearfish Layer Group when sf:sfdem is listed as the 3rd layer.

##### A: _Lab screenshot 2.png_

#### Q6: What is the WMS url for the single-tiled request?

##### A: *http://localhost:8080/geoserver/wms?SERVICE=WMS&VERSION=1.1.1&REQUEST=GetMap&FORMAT=image%2Fpng&TRANSPARENT=true&LAYERS=spearfish&exceptions=application%2Fvnd.ogc.se_inimage&SRS=EPSG%3A26713&STYLES=&WIDTH=768&HEIGHT=539&BBOX=591647.4706640587%2C4916070.146012163%2C606306.9511605742%2C4926358.505371045*

#### Q7: What is the WMS url for one of the tiled requests? What is the image size?

##### A: *http://localhost:8080/geoserver/wms?SERVICE=WMS&VERSION=1.1.1&REQUEST=GetMap&FORMAT=image%2Fpng&TRANSPARENT=true&tiled=true&LAYERS=spearfish&exceptions=application%2Fvnd.ogc.se_inimage&tilesOrigin=589425.9342365642%2C4913959.224611808&WIDTH=256&HEIGHT=256&SRS=EPSG%3A26713&STYLES=&BBOX=605925.1938559785%2C4925585.446829237%2C610811.687354817%2C4930471.940328076* 
      *The tile size is 256 x 256.*

#### Q8: What is the URL of your coarse resolution sample of a WMTS url? What level does this tile refer to? Notice the differences. What are some of the fields that are unique to this url?

##### A: *http://localhost:8080/geoserver/gwc/service/wmts?layer=spearfish&style=&tilematrixset=EPSG%3A4326&Service=WMTS&Request=GetTile&Version=1.0.0&Format=image%2Fpng&TileMatrix=EPSG%3A4326%3A12&TileCol=1734&TileRow=1037. Level 12. There is a tilerow and tile column rather than an image size.

#### Q9: In the zoomed-out URL, what are the TileCol and TileRow?

##### A: *TileCol: 1734 and TileRow: 1037*

#### Q10: In the zoomed-in URL, what are the TileCol and TileRow?

##### A: *TileCol: 111016 and TileRow: 66382*

#### Q11: Why are they so different for the same location in the map?

##### A: *Since we are zoomed in, the original image is divided into many smaller tiles.*

#### Q12: Is there a difference in the TileMatrix? %3A is an HTML encoding for a colon, `:`.What does the number after EPSG:4326 mean?

#### A: *There is a difference. The number after the colon is the level. In the coarse it was 12; here it is 18.*

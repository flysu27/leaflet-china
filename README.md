其余操作和leaflet一样（已包含proj4.js）

√ 修改默认底图+投影为 中国腾讯地图

```
<!DOCTYPE html>
<html>

<head>
    <title></title>
    <meta charset="utf-8">
    <style type="text/css">
        body {
            padding: 0;
            margin: 0;
        }

        html,
        body,
        #map {
            height: 100%;
        }
    </style>
    <link rel="stylesheet" href="./leaflet.css" />

</head>

<body>
    <div id='map'></div>
</body>
<script type="text/javascript" src='./leaflet-china.js'></script>
<script type="text/javascript">

    var map = L.map("map", {
        center: [31.59, 120.29],
        zoom: 12,
        layers: [image],
        zoomControl: false
    });
</script>

</html>
```

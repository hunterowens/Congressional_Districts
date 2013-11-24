Congressional_Districts
=======================

A geojson representation of the 113th Congress. 

Converision was done from the [2013 Tiger Line Shapefiles](http://www.census.gov/cgi-bin/geo/shapefiles2013/layers.cgi) using the [GDAL](http://www.gdal.org/) library. 

The file `districts.json` is too large to have stored in github (100.4 MB), so it is pushed gziped to github. 

To get the file on your computer -
```
$ git clone http://github.com/hunterowens/Congressional_Districts.git
$ cd Congressional_Districts
$ gunzip districts.json
```
And you can then accesss the file. To avoid adding the full file to git when running commands such as `git add .`, `districts.json` is in the gitignore. Should you make modifications to file, run gzip `districts.json`, add the file to git and then push it to origin. Pull Requests Welcome. 

One way to the load the geojson onto a map is to use [Tilemill](https://www.mapbox.com/tilemill/) and add the file `districts.json` as a layer.

![Example Map](https://raw.github.com/hunterowens/Congressional_Districts/master/CongressionalDistricts.png)

==============================================

The MIT License (MIT)

Copyright (c) 2013 Hunter Owens (hunter [at] hunterowens.net)

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
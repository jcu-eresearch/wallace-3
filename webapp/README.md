climas-ng
=========

https://travis-ci.org/jcu-eresearch/climas-ng.svg?branch=master

CliMAS Next Generation

The project is built using [pyramid (python 2.7)](https://trypyramid.com/) and [coffee script](https://coffeescript.org/).

# Installing dependencies 
The project isn't (currently) compatible with the latest versions of all the dependencies. 

Python dependencies:

```
# install problematic dependencies
pip install 'pygments==1.6'
pip install MarkupSafe

# install everything else
python setup.py install
```

JS dependencies:

`npm install` will work but you will need a version of node < 11 for gulp to run.

# Running the project

To build the js: `gulp` (will watch) or `gulp build`
- will need to re-run each time CoffeeScript code is changed
- code changes will need to be committed before pushing to production

To build/install python code: `python setup.py install`
- will need to re-run each time python code is changed

To run the project `pserve [ production.ini | test.ini ]`
- will need to re-run every time the python or js code changes
- runs on localhost:6543

# About

Main frontend/map code in: `webapp/climasng/src/coffee/mapview/views/app.coffee`

Main API code in: `webapp/climasng/views/apiview.py`

Files in `webapp/climasng/static` and `webapp/climasng/src/js` are generated

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

`npm install` will work but you will need a version of Node < 11 for gulp to run.
[`nvm`](https://github.com/nvm-sh/nvm) provides an easy way of installing older versions of Node;
builds have been tested with `v8.17.0`.

# Running the project

To build the js: `npm run build` (to run a build) or `npx gulp` (will watch for changes)
- will need to be re-run each time CoffeeScript code is changed
- code changes will need to be committed before pushing to production

To build/install python code: `python setup.py install`
- will need to be re-run each time Python code is changed

To run the project `pserve [ production.ini | test.ini ]`
- will need to rbe e-run every time the Python or JS code changes
- runs on `localhost:6543`

# About

Main frontend/map code in: `webapp/climasng/src/coffee/mapview/views/app.coffee`

Main API code in: `webapp/climasng/views/apiview.py`

Files in `webapp/climasng/static` and `webapp/climasng/src/js` are generated

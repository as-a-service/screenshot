# Takes a screenshot of the given page

A simple web service that takes screenshot of the given URL.

Run with `docker run -p 8080:8080 gcr.io/as-a-service-dev/screenshot`

[![Run on Google Cloud](https://storage.googleapis.com/cloudrun/button.svg)](https://deploy.cloud.run)

## API

### URL parameters:

* `url`: The URL of the website to screenshot
* (`width`): The viewport width (in pixels), defaults to 1280
* (`height`): The viewport height (in pixels), defaults to 800

Example: `/?url=https://steren.fr`

## Running the server locally

* Build with `docker build . -t screenshot`
* Start with `docker run -p 8080:8080 screenshot`
* Open in your browser at `http://localhost:8080/?url=https://steren.fr`

![CloudBuild](https://badger-l7zawt5jsq-uw.a.run.app/build/status?project=as-a-service-dev&id=55d8abca-3a3c-428e-a608-2c4caa10df58)

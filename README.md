## The `openapi` folder

This folder contains your entrypoint `openapi.yaml`.

That file contains references to the entire Data Transfer Exchange Format definition.
 
In components, the `schemas` holds all definitions for the entities and their associations `*.yaml`.

There is no security scheme as this is a public documentation of the Data Transfer Exchange Format for DRK-UC1

# To Preview 

In the `openapi` folder run: `redocly preview-docs openapi.yaml`

# To build

In the `openapi` folder run: `redocly bundle -o dist/bundle.yaml`

# To test

In the `openapi` folder run: `redocly lint`

# To update  

* In the root folder install `npm install -g redoc-cli`  

* Build into index.html `npx @redocly/cli build-docs  openapi/openapi.yaml -o index.html`

* Check `open index.html`

Further information: https://spec.openapis.org/oas/v3.0.3.html#contact-object


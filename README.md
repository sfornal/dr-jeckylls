# Dr. Jeckyll's Beer Lab Redesign

[![Netlify Status](https://api.netlify.com/api/v1/badges/d5ef6e13-4280-401e-828b-562a9ca6735a/deploy-status)](https://app.netlify.com/sites/dr-jeckylls-beerlab/deploys)

A new website design for Dr. Jeckyll's Beer Lab in Pantego, TX. Static site, hosted on Netlify, using Netlify CMS for content management. Built on Eleventy and the EleventyOne starter kit by Phil Hawksworth.

## Prerequisites

- [Node and NPM](https://nodejs.org/)

## Running locally

```bash
# install the dependencies
npm install

# External data sources can be stashed locally
npm run seed

# It will then be available locally for building with
npm run start
```

## Add some Netlify helpers
Netlify Dev adds the ability to use Netlify redirects, proxies, and serverless functions.

```bash
# install the Netlify CLI in order to get Netlify Dev
npm install -g netlify-cli

# run a local server with some added Netlify sugar in front of Eleventy
netlify dev
```

A serverless functions pipeline is included via Netlify Dev. By running `netlify dev` you'll be able to execute any of your serverless functions directly like this:

- /.netlify/functions/hello
- /.netlify/functions/fetch-joke


### Redirects and proxies

Netlify's Redirects API can provide friendlier URLs as proxies to these URLs.

- /api/hello
- /api/fetch-joke


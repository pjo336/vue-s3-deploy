# Vue S3 Deploy

## This package provides a quick utility to upload Vue applications that are deployed as static web pages on Aws S3

### Qualifiers:
- `dist` package expected
- `dist/index.html` must exist

### Installation

`yarn add -D vue-s3-deploy`

or

`npm install --save-dev vue-s3-deploy`

### Usage
Accepts the bucket name as the sole argument. Place a deploy script in your package.json. Here is an example:

```
"scripts": {
  "deploy": "rm -rf dist && yarn build && yarn vueS3Deploy <my-bucket>",
  "start": "yarn dev",
  "build": "node build/build.js"
},
```
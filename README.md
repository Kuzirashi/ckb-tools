# CKB.tools

![GitHub package.json version](https://img.shields.io/github/package-json/v/jordanmack/ckb-tools)
![GitHub last commit](https://img.shields.io/github/last-commit/jordanmack/ckb-tools)
![Travis (.org)](https://travis-ci.com/jordanmack/ckb-tools.svg)
![Requires.io](https://img.shields.io/requires/github/jordanmack/ckb-tools)
![Uptime Robot status](https://img.shields.io/uptimerobot/status/m788404415-839b32111e1dc755c52c3e33)
![Uptime Robot ratio (30 days)](https://img.shields.io/uptimerobot/ratio/m788404415-839b32111e1dc755c52c3e33)
![GitHub Repo stars](https://img.shields.io/github/stars/jordanmack/ckb-tools?style=social)

[CKB.tools](https://ckb.tools/) is a online collection of free development tools created for use on Nervos Network.

## Developing

These instructions describe how to launch, run, and develop using the CKB.tools code base.

If you don't need to develop and just want to use the tools, visit the [CKB.tools](https://ckb.tools/) website.

### Prerequisites

- [Node.js 14+](https://nodejs.org/en/)

### Install Dependencies

```sh
npm i --force
```

You will also need to delete the following file due to a problem in the NPM package.

```sh
rm -f node_modules/hookrouter/dist/index.d.ts
cd node_modules/@polyjuice-provider/repo && npm i && npm run build
```

### Configure

Edit the `src/config.js` file.

### Start the Development Server

```sh
npm start
```

### Building

```sh
npm run build
```

### Deploying

Build the project, then copy the complete contents of the `build` directory to the document root of the web server.

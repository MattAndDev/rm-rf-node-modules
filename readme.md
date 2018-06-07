# rm-nm

[![circleci](https://circleci.com/gh/MattAndDev/rm-nm/tree/master.svg?style=shield&circle-token=12aedd82a9a427ca644f90be5404e1a7232da500)](https://circleci.com/gh/MattAndDev/rm-nm)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

> Remove node_modules

## why?

- Because not everyone is a bash ninja
- Because not everyone has 1TB ssd
- Because I tend to abuse `npm i`

and of course because:

![node modules are heavier then neutron stars](http://devhumor.com/content/uploads/images/August2017/node-modules.jpg)


## usage
As now:
```
node rm-node-modules /target/dir (args)
```
Will look into `/target/dir` for every first level `node_modules` folder and delete it.
So use at your own risk, this does `rm -rf` a lot of things.

Args as now:
```
-s // will only remove node modules if package.json is present
-ss // will only remove node modules if package.json && package-json.lock is present
```
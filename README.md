fis3-optimizer-css-compressor
========

[![Dependency Status](https://david-dm.org/wuhy/fis3-optimizer-css-compressor.svg)](https://david-dm.org/wuhy/fis3-optimizer-css-compressor) [![devDependency Status](https://david-dm.org/wuhy/fis3-optimizer-css-compressor/dev-status.svg)](https://david-dm.org/wuhy/fis3-optimizer-css-compressor#info=devDependencies) [![NPM Version](https://img.shields.io/npm/v/fis3-optimizer-css-compressor.svg?style=flat)](https://npmjs.org/package/fis3-optimizer-css-compressor)


> An optimizer for fis3 to compress css files by using clean-css.


## How to use
 
### Install
 
```shell
npm install fis3-optimizer-css-compressor -g
```

### Add configure to `fis-conf.js`

```javasciprt
fis.media('prod').match('*.css', {
    optimizer: 'css-compressor'
});
```

Custom compress options:

```javasciprt
fis.match('*.css', {
       optimizer: fis.plugin('css-compressor', {
            advanced: true
       })
   });
```

Available options, please refer to [clean-css](https://github.com/jakubpawlowicz/clean-css).


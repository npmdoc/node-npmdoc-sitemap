# api documentation for  [sitemap (v1.12.0)](https://github.com/ekalinin/sitemap.js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-sitemap.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-sitemap) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sitemap.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sitemap)
#### Sitemap-generating framework

[![NPM](https://nodei.co/npm/sitemap.png?downloads=true)](https://www.npmjs.com/package/sitemap)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sitemap/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-sitemap_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sitemap/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sitemap/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sitemap/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Eugene Kalinin",
        "email": "e.v.kalinin@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/ekalinin/sitemap.js/issues"
    },
    "dependencies": {
        "underscore": "^1.7.0",
        "url-join": "^1.1.0"
    },
    "description": "Sitemap-generating framework",
    "devDependencies": {
        "expresso": "^0.9.2",
        "sinon": "^1.16.1"
    },
    "directories": {},
    "dist": {
        "shasum": "40362c89e00e1f13a851bbdadfbc13cbec34c19b",
        "tarball": "https://registry.npmjs.org/sitemap/-/sitemap-1.12.0.tgz"
    },
    "gitHead": "7a1598374aea7bab831c4de570329363df79bad1",
    "homepage": "https://github.com/ekalinin/sitemap.js#readme",
    "keywords": [
        "sitemap",
        "sitemap.xml"
    ],
    "main": "index",
    "maintainers": [
        {
            "name": "ekalinin",
            "email": "e.v.kalinin@gmail.com"
        }
    ],
    "name": "sitemap",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ekalinin/sitemap.js.git"
    },
    "scripts": {
        "test": "./node_modules/expresso/bin/expresso tests/sitemap.test.js"
    },
    "version": "1.12.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module sitemap](#apidoc.module.sitemap)
1.  [function <span class="apidocSignatureSpan">sitemap.</span>Sitemap (urls, hostname, cacheTime, xslUrl, xmlNs)](#apidoc.element.sitemap.Sitemap)
1.  [function <span class="apidocSignatureSpan">sitemap.</span>SitemapItem (conf)](#apidoc.element.sitemap.SitemapItem)
1.  [function <span class="apidocSignatureSpan">sitemap.</span>buildSitemapIndex (conf)](#apidoc.element.sitemap.buildSitemapIndex)
1.  [function <span class="apidocSignatureSpan">sitemap.</span>createSitemap (conf)](#apidoc.element.sitemap.createSitemap)
1.  [function <span class="apidocSignatureSpan">sitemap.</span>createSitemapIndex (conf)](#apidoc.element.sitemap.createSitemapIndex)
1.  object <span class="apidocSignatureSpan">sitemap.</span>Sitemap.prototype
1.  object <span class="apidocSignatureSpan">sitemap.</span>SitemapItem.prototype
1.  object <span class="apidocSignatureSpan">sitemap.</span>errors
1.  object <span class="apidocSignatureSpan">sitemap.</span>utils
1.  string <span class="apidocSignatureSpan">sitemap.</span>version

#### [module sitemap.Sitemap](#apidoc.module.sitemap.Sitemap)
1.  [function <span class="apidocSignatureSpan">sitemap.</span>Sitemap (urls, hostname, cacheTime, xslUrl, xmlNs)](#apidoc.element.sitemap.Sitemap.Sitemap)

#### [module sitemap.Sitemap.prototype](#apidoc.module.sitemap.Sitemap.prototype)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>add (url)](#apidoc.element.sitemap.Sitemap.prototype.add)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>clearCache ()](#apidoc.element.sitemap.Sitemap.prototype.clearCache)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>del (url)](#apidoc.element.sitemap.Sitemap.prototype.del)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>isCacheValid ()](#apidoc.element.sitemap.Sitemap.prototype.isCacheValid)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>setCache (newCache)](#apidoc.element.sitemap.Sitemap.prototype.setCache)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>toGzip (callback)](#apidoc.element.sitemap.Sitemap.prototype.toGzip)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>toString ()](#apidoc.element.sitemap.Sitemap.prototype.toString)
1.  [function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>toXML (callback)](#apidoc.element.sitemap.Sitemap.prototype.toXML)

#### [module sitemap.SitemapItem](#apidoc.module.sitemap.SitemapItem)
1.  [function <span class="apidocSignatureSpan">sitemap.</span>SitemapItem (conf)](#apidoc.element.sitemap.SitemapItem.SitemapItem)

#### [module sitemap.SitemapItem.prototype](#apidoc.module.sitemap.SitemapItem.prototype)
1.  [function <span class="apidocSignatureSpan">sitemap.SitemapItem.prototype.</span>toString ()](#apidoc.element.sitemap.SitemapItem.prototype.toString)
1.  [function <span class="apidocSignatureSpan">sitemap.SitemapItem.prototype.</span>toXML ()](#apidoc.element.sitemap.SitemapItem.prototype.toXML)

#### [module sitemap.errors](#apidoc.module.sitemap.errors)
1.  [function <span class="apidocSignatureSpan">sitemap.errors.</span>ChangeFreqInvalidError (message)](#apidoc.element.sitemap.errors.ChangeFreqInvalidError)
1.  [function <span class="apidocSignatureSpan">sitemap.errors.</span>InvalidVideoFormat (message)](#apidoc.element.sitemap.errors.InvalidVideoFormat)
1.  [function <span class="apidocSignatureSpan">sitemap.errors.</span>NoURLError (message)](#apidoc.element.sitemap.errors.NoURLError)
1.  [function <span class="apidocSignatureSpan">sitemap.errors.</span>NoURLProtocolError (message)](#apidoc.element.sitemap.errors.NoURLProtocolError)
1.  [function <span class="apidocSignatureSpan">sitemap.errors.</span>PriorityInvalidError (message)](#apidoc.element.sitemap.errors.PriorityInvalidError)
1.  [function <span class="apidocSignatureSpan">sitemap.errors.</span>UndefinedTargetFolder (message)](#apidoc.element.sitemap.errors.UndefinedTargetFolder)

#### [module sitemap.utils](#apidoc.module.sitemap.utils)
1.  [function <span class="apidocSignatureSpan">sitemap.utils.</span>abort (str)](#apidoc.element.sitemap.utils.abort)
1.  [function <span class="apidocSignatureSpan">sitemap.utils.</span>chunkArray (arr, chunkSize)](#apidoc.element.sitemap.utils.chunkArray)
1.  [function <span class="apidocSignatureSpan">sitemap.utils.</span>distinctArray (arr)](#apidoc.element.sitemap.utils.distinctArray)
1.  [function <span class="apidocSignatureSpan">sitemap.utils.</span>getTimestamp ()](#apidoc.element.sitemap.utils.getTimestamp)
1.  [function <span class="apidocSignatureSpan">sitemap.utils.</span>getTimestampFromDate (dt, bRealtime)](#apidoc.element.sitemap.utils.getTimestampFromDate)
1.  [function <span class="apidocSignatureSpan">sitemap.utils.</span>htmlEscape (text)](#apidoc.element.sitemap.utils.htmlEscape)
1.  [function <span class="apidocSignatureSpan">sitemap.utils.</span>lpad (n, len, chr)](#apidoc.element.sitemap.utils.lpad)



# <a name="apidoc.module.sitemap"></a>[module sitemap](#apidoc.module.sitemap)

#### <a name="apidoc.element.sitemap.Sitemap"></a>[function <span class="apidocSignatureSpan">sitemap.</span>Sitemap (urls, hostname, cacheTime, xslUrl, xmlNs)](#apidoc.element.sitemap.Sitemap)
- description and source-code
```javascript
function Sitemap(urls, hostname, cacheTime, xslUrl, xmlNs) {

  // This limit is defined by Google. See:
  // http://sitemaps.org/protocol.php#index
  this.limit = 50000

  // Base domain
  this.hostname = hostname;

  // URL list for sitemap
  this.urls = [];

  // Make copy of object
  if (urls) _.extend(this.urls, (urls instanceof Array) ? urls : [urls]);

  // sitemap cache
  this.cacheResetPeriod = cacheTime || 0;
  this.cache = '';

  this.xslUrl = xslUrl;
  this.xmlNs = xmlNs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.SitemapItem"></a>[function <span class="apidocSignatureSpan">sitemap.</span>SitemapItem (conf)](#apidoc.element.sitemap.SitemapItem)
- description and source-code
```javascript
function SitemapItem(conf) {
  var conf = conf || {}
    , is_safe_url = conf['safe'];

  if (!conf['url']) {
    throw new err.NoURLError();
  }

  // URL of the page
  if(!conf.cdata) {
    this.loc = safeUrl(conf);
  } else {
    this.loc = conf.url;
  }

  // If given a file to use for last modified date
  if (conf['lastmodfile']) {
    //console.log('should read stat from file: ' + conf['lastmodfile']);
    var file = conf['lastmodfile'];

    var stat = fs.statSync(file);

    var mtime = stat.mtime;

    var dt = new Date(mtime);
    this.lastmod = ut.getTimestampFromDate(dt, conf['lastmodrealtime']);

  }
  // The date of last modification (YYYY-MM-DD)
  else if (conf['lastmod']) {
    // append the timezone offset so that dates are treated as local time.
    // Otherwise the Unit tests fail sometimes.
    var timezoneOffset = 'UTC-' + (new Date().getTimezoneOffset() / 60) + '00';
    timezoneOffset = timezoneOffset.replace('--', '-');
    var dt = new Date(conf['lastmod'] + ' ' + timezoneOffset);
    this.lastmod = ut.getTimestampFromDate(dt, conf['lastmodrealtime']);
  } else if (conf['lastmodISO']) {
    this.lastmod = conf['lastmodISO'];
  }

  // How frequently the page is likely to change
  // due to this field is optional no default value is set
  // please see: http://www.sitemaps.org/protocol.html
  this.changefreq = conf['changefreq'];
  if (!is_safe_url && this.changefreq) {
    if (['always', 'hourly', 'daily', 'weekly', 'monthly',
        'yearly', 'never'].indexOf(this.changefreq) === -1) {
      throw new err.ChangeFreqInvalidError();
    }
  }

  // The priority of this URL relative to other URLs
  // due to this field is optional no default value is set
  // please see: http://www.sitemaps.org/protocol.html
  this.priority = conf['priority'];
  if (!is_safe_url && this.priority) {
    if (!(this.priority >= 0.0 && this.priority <= 1.0) || typeof this.priority !== 'number') {
      throw new err.PriorityInvalidError();
    }
  }

  this.news = conf['news'] || null;
  this.img = conf['img'] || null;
  this.links = conf['links'] || null;
  this.expires = conf['expires'] || null;
  this.androidLink = conf['androidLink'] || null;
  this.mobile = conf['mobile'] || null;
  this.video = conf['video'] || null;
  this.ampLink = conf['ampLink'] || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.buildSitemapIndex"></a>[function <span class="apidocSignatureSpan">sitemap.</span>buildSitemapIndex (conf)](#apidoc.element.sitemap.buildSitemapIndex)
- description and source-code
```javascript
function buildSitemapIndex(conf) {
  var xml = [];

  xml.push('<?xml version="1.0" encoding="UTF-8"?>');
  if (conf.xslUrl) {
    xml.push('<?xml-stylesheet type="text/xsl" href="' + conf.xslUrl + '"?>');
  }
  if(!conf.xmlNs) {
    xml.push('<sitemapindex xmlns="http://www.sitemaps.org/schemas/sitemap/0.9" ' +
      'xmlns:mobile="http://www.google.com/schemas/sitemap-mobile/1.0" ' +
      'xmlns:image="http://www.google.com/schemas/sitemap-image/1.1" ' +
      'xmlns:video="http://www.google.com/schemas/sitemap-video/1.1">');
  } else {
    xml.push('<sitemapindex ' + conf.xmlNs + '>')
  }


  conf.urls.forEach(function (url) {
    xml.push('<sitemap>');
    xml.push('<loc>' + url + '</loc>');
    xml.push('</sitemap>');
  });

  xml.push('</sitemapindex>');

  return xml.join('\n');
}
```
- example usage
```shell
...
    });
'''

### Example of Sitemap Index as String

'''javascript
var sm = require('sitemap')
  , smi = sm.buildSitemapIndex({
      urls: ['https://example.com/sitemap1.xml', 'https://example.com/sitemap2.xml']
      xslUrl: 'https://example.com/style.xsl' // optional
    });
'''

### Example of Sitemap Index
...
```

#### <a name="apidoc.element.sitemap.createSitemap"></a>[function <span class="apidocSignatureSpan">sitemap.</span>createSitemap (conf)](#apidoc.element.sitemap.createSitemap)
- description and source-code
```javascript
function createSitemap(conf) {
  return new Sitemap(conf.urls, conf.hostname, conf.cacheTime, conf.xslUrl, conf.xmlNs);
}
```
- example usage
```shell
...
Usage
-----
The main functions you want to use in the sitemap module are

'''javascript
var sm = require('sitemap')
// Creates a sitemap object given the input configuration with URLs
var sitemap = sm.createSitemap({ options });
// Generates XML with a callback function
sitemap.toXML( function(err, xml){ if (!err){ console.log(xml) } });
// Gives you a string containing the XML data
var xml = sitemap.toString();
'''

### Example of using sitemap.js with [express](https://github.com/visionmedia/express):
...
```

#### <a name="apidoc.element.sitemap.createSitemapIndex"></a>[function <span class="apidocSignatureSpan">sitemap.</span>createSitemapIndex (conf)](#apidoc.element.sitemap.createSitemapIndex)
- description and source-code
```javascript
function createSitemapIndex(conf) {
  return new SitemapIndex(conf.urls,
    conf.targetFolder,
    conf.hostname,
    conf.cacheTime,
    conf.sitemapName,
    conf.sitemapSize,
    conf.xslUrl,
    conf.gzip,
    conf.callback);
}
```
- example usage
```shell
...
  });
'''

### Example of Sitemap Index

'''javascript
var sm = require('sitemap')
, smi = sm.createSitemapIndex({
    cacheTime: 600000,
    hostname: 'http://www.sitemap.org',
    sitemapName: 'sm-test',
    sitemapSize: 1,
    targetFolder: require('os').tmpdir(),
    urls: ['http://ya.ru', 'http://ya2.ru']
    // optional:
...
```



# <a name="apidoc.module.sitemap.Sitemap"></a>[module sitemap.Sitemap](#apidoc.module.sitemap.Sitemap)

#### <a name="apidoc.element.sitemap.Sitemap.Sitemap"></a>[function <span class="apidocSignatureSpan">sitemap.</span>Sitemap (urls, hostname, cacheTime, xslUrl, xmlNs)](#apidoc.element.sitemap.Sitemap.Sitemap)
- description and source-code
```javascript
function Sitemap(urls, hostname, cacheTime, xslUrl, xmlNs) {

  // This limit is defined by Google. See:
  // http://sitemaps.org/protocol.php#index
  this.limit = 50000

  // Base domain
  this.hostname = hostname;

  // URL list for sitemap
  this.urls = [];

  // Make copy of object
  if (urls) _.extend(this.urls, (urls instanceof Array) ? urls : [urls]);

  // sitemap cache
  this.cacheResetPeriod = cacheTime || 0;
  this.cache = '';

  this.xslUrl = xslUrl;
  this.xmlNs = xmlNs;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sitemap.Sitemap.prototype"></a>[module sitemap.Sitemap.prototype](#apidoc.module.sitemap.Sitemap.prototype)

#### <a name="apidoc.element.sitemap.Sitemap.prototype.add"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>add (url)](#apidoc.element.sitemap.Sitemap.prototype.add)
- description and source-code
```javascript
add = function (url) {
  return this.urls.push(url);
}
```
- example usage
```shell
...
### Example of dynamic page manipulations into sitemap:

'''javascript
var sitemap = sm.createSitemap ({
      hostname: 'http://example.com',
      cacheTime: 600000
    });
sitemap.add({url: '/page-1/'});
sitemap.add({url: '/page-2/', changefreq: 'monthly', priority: 0.7});
sitemap.del({url: '/page-2/'});
sitemap.del('/page-1/');
'''
...
```

#### <a name="apidoc.element.sitemap.Sitemap.prototype.clearCache"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>clearCache ()](#apidoc.element.sitemap.Sitemap.prototype.clearCache)
- description and source-code
```javascript
clearCache = function () {
  this.cache = '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.Sitemap.prototype.del"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>del (url)](#apidoc.element.sitemap.Sitemap.prototype.del)
- description and source-code
```javascript
del = function (url) {
  var index_to_remove = [],
    key = '',
    self = this;

  if (typeof url == 'string') {
    key = url;
  } else {
    key = url['url'];
  }

  // find
  this.urls.forEach(function (elem, index) {
    if (typeof elem == 'string') {
      if (elem == key) {
        index_to_remove.push(index);
      }
    } else {
      if (elem['url'] == key) {
        index_to_remove.push(index);
      }
    }
  });

  // delete
  index_to_remove.forEach(function (elem) {
    self.urls.splice(elem, 1);
  });

  return index_to_remove.length;
}
```
- example usage
```shell
...
'''javascript
var sitemap = sm.createSitemap ({
      hostname: 'http://example.com',
      cacheTime: 600000
    });
sitemap.add({url: '/page-1/'});
sitemap.add({url: '/page-2/', changefreq: 'monthly', priority: 0.7});
sitemap.del({url: '/page-2/'});
sitemap.del('/page-1/');
'''



### Example of pre-generating sitemap based on existing static files:
...
```

#### <a name="apidoc.element.sitemap.Sitemap.prototype.isCacheValid"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>isCacheValid ()](#apidoc.element.sitemap.Sitemap.prototype.isCacheValid)
- description and source-code
```javascript
isCacheValid = function () {
  var currTimestamp = ut.getTimestamp();
  return this.cacheResetPeriod && this.cache &&
    (this.cacheSetTimestamp + this.cacheResetPeriod) >= currTimestamp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.Sitemap.prototype.setCache"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>setCache (newCache)](#apidoc.element.sitemap.Sitemap.prototype.setCache)
- description and source-code
```javascript
setCache = function (newCache) {
  this.cache = newCache;
  this.cacheSetTimestamp = ut.getTimestamp();
  return this.cache;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.Sitemap.prototype.toGzip"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>toGzip (callback)](#apidoc.element.sitemap.Sitemap.prototype.toGzip)
- description and source-code
```javascript
toGzip = function (callback) {
  var zlib = require('zlib');

  if (typeof callback === 'function') {
    zlib.gzip(this.toString(), callback);
  } else {
    return zlib.gzipSync(this.toString());
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.Sitemap.prototype.toString"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>toString ()](#apidoc.element.sitemap.Sitemap.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var self = this, xml;
  if(!self.xmlNs) {
      xml = ['<?xml version="1.0" encoding="UTF-8"?>',
      '<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9" ' +
      'xmlns:news="http://www.google.com/schemas/sitemap-news/0.9" ' +
      'xmlns:xhtml="http://www.w3.org/1999/xhtml" ' +
      'xmlns:mobile="http://www.google.com/schemas/sitemap-mobile/1.0" ' +
      'xmlns:image="http://www.google.com/schemas/sitemap-image/1.1" ' +
      'xmlns:video="http://www.google.com/schemas/sitemap-video/1.1">'
    ];
  } else {
    xml = ['<?xml version="1.0" encoding="UTF-8"?>', '<urlset '+ this.xmlNs + '>']
  }

  if (self.xslUrl) {
    xml.splice(1, 0,
      '<?xml-stylesheet type="text/xsl" href="' + self.xslUrl + '"?>');
  }

  if (self.isCacheValid()) {
    return self.cache;
  }

  // TODO: if size > limit: create sitemapindex

  self.urls.forEach(function (elem, index) {
    // SitemapItem
    var smi = elem;

    // create object with url property
    if (typeof elem == 'string') {
      smi = {'url': elem};
    }
    // insert domain name
    if (self.hostname) {
      if (!reProto.test(smi.url)) {
        smi.url = urljoin(self.hostname, smi.url);
      }
      if (smi.img) {
        if (typeof smi.img == 'string') {
          // string -> array of objects
          smi.img = [{url: smi.img}];
        }
        if (typeof smi.img == 'object' && smi.img.length == undefined) {
          // object -> array of objects
          smi.img = [smi.img];
        }
        // prepend hostname to all image urls
        smi.img.forEach(function (img) {
          if (!reProto.test(img.url)) {
            img.url = urljoin(self.hostname, img.url);
          }
        });
      }
      if (smi.links) {
        smi.links.forEach(function (link) {
          if (!reProto.test(link.url)) {
            link.url = urljoin(self.hostname, link.url);
          }
        });
      }
    }
    xml.push(new SitemapItem(smi));
  });
  // close xml
  xml.push('</urlset>');

  return self.setCache(xml.join('\n'));
}
```
- example usage
```shell
...
'''javascript
var sm = require('sitemap')
// Creates a sitemap object given the input configuration with URLs
var sitemap = sm.createSitemap({ options });
// Generates XML with a callback function
sitemap.toXML( function(err, xml){ if (!err){ console.log(xml) } });
// Gives you a string containing the XML data
var xml = sitemap.toString();
'''

### Example of using sitemap.js with [express](https://github.com/visionmedia/express):

'''javascript
var express = require('express')
, sm = require('sitemap');
...
```

#### <a name="apidoc.element.sitemap.Sitemap.prototype.toXML"></a>[function <span class="apidocSignatureSpan">sitemap.Sitemap.prototype.</span>toXML (callback)](#apidoc.element.sitemap.Sitemap.prototype.toXML)
- description and source-code
```javascript
toXML = function (callback) {
  if (typeof callback === 'undefined') {
    return this.toString();
  }
  var self = this;
  process.nextTick(function () {
    try {
      return callback(null, self.toString());
    } catch (err) {
      return callback(err);
    }
  });
}
```
- example usage
```shell
...
The main functions you want to use in the sitemap module are

'''javascript
var sm = require('sitemap')
// Creates a sitemap object given the input configuration with URLs
var sitemap = sm.createSitemap({ options });
// Generates XML with a callback function
sitemap.toXML( function(err, xml){ if (!err){ console.log(xml) } });
// Gives you a string containing the XML data
var xml = sitemap.toString();
'''

### Example of using sitemap.js with [express](https://github.com/visionmedia/express):

'''javascript
...
```



# <a name="apidoc.module.sitemap.SitemapItem"></a>[module sitemap.SitemapItem](#apidoc.module.sitemap.SitemapItem)

#### <a name="apidoc.element.sitemap.SitemapItem.SitemapItem"></a>[function <span class="apidocSignatureSpan">sitemap.</span>SitemapItem (conf)](#apidoc.element.sitemap.SitemapItem.SitemapItem)
- description and source-code
```javascript
function SitemapItem(conf) {
  var conf = conf || {}
    , is_safe_url = conf['safe'];

  if (!conf['url']) {
    throw new err.NoURLError();
  }

  // URL of the page
  if(!conf.cdata) {
    this.loc = safeUrl(conf);
  } else {
    this.loc = conf.url;
  }

  // If given a file to use for last modified date
  if (conf['lastmodfile']) {
    //console.log('should read stat from file: ' + conf['lastmodfile']);
    var file = conf['lastmodfile'];

    var stat = fs.statSync(file);

    var mtime = stat.mtime;

    var dt = new Date(mtime);
    this.lastmod = ut.getTimestampFromDate(dt, conf['lastmodrealtime']);

  }
  // The date of last modification (YYYY-MM-DD)
  else if (conf['lastmod']) {
    // append the timezone offset so that dates are treated as local time.
    // Otherwise the Unit tests fail sometimes.
    var timezoneOffset = 'UTC-' + (new Date().getTimezoneOffset() / 60) + '00';
    timezoneOffset = timezoneOffset.replace('--', '-');
    var dt = new Date(conf['lastmod'] + ' ' + timezoneOffset);
    this.lastmod = ut.getTimestampFromDate(dt, conf['lastmodrealtime']);
  } else if (conf['lastmodISO']) {
    this.lastmod = conf['lastmodISO'];
  }

  // How frequently the page is likely to change
  // due to this field is optional no default value is set
  // please see: http://www.sitemaps.org/protocol.html
  this.changefreq = conf['changefreq'];
  if (!is_safe_url && this.changefreq) {
    if (['always', 'hourly', 'daily', 'weekly', 'monthly',
        'yearly', 'never'].indexOf(this.changefreq) === -1) {
      throw new err.ChangeFreqInvalidError();
    }
  }

  // The priority of this URL relative to other URLs
  // due to this field is optional no default value is set
  // please see: http://www.sitemaps.org/protocol.html
  this.priority = conf['priority'];
  if (!is_safe_url && this.priority) {
    if (!(this.priority >= 0.0 && this.priority <= 1.0) || typeof this.priority !== 'number') {
      throw new err.PriorityInvalidError();
    }
  }

  this.news = conf['news'] || null;
  this.img = conf['img'] || null;
  this.links = conf['links'] || null;
  this.expires = conf['expires'] || null;
  this.androidLink = conf['androidLink'] || null;
  this.mobile = conf['mobile'] || null;
  this.video = conf['video'] || null;
  this.ampLink = conf['ampLink'] || null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sitemap.SitemapItem.prototype"></a>[module sitemap.SitemapItem.prototype](#apidoc.module.sitemap.SitemapItem.prototype)

#### <a name="apidoc.element.sitemap.SitemapItem.prototype.toString"></a>[function <span class="apidocSignatureSpan">sitemap.SitemapItem.prototype.</span>toString ()](#apidoc.element.sitemap.SitemapItem.prototype.toString)
- description and source-code
```javascript
toString = function () {
  // result xml
  var xml = '<url> {loc} {img} {video} {lastmod} {changefreq} {priority} {links} {expires} {androidLink} {mobile} {news} {ampLink
}</url>'
  // xml property
    , props = ['loc', 'img', 'video', 'lastmod', 'changefreq', 'priority', 'links', 'expires', 'androidLink', 'mobile', 'news', '
ampLink']
  // property array size (for loop)
    , ps = props.length
  // current property name (for loop)
    , p;

  while (ps--) {
    p = props[ps];

    if (this[p] && p == 'img') {
      var imagexml = '';
      // Image handling
      if (typeof(this[p]) != 'object' || this[p].length == undefined) {
        // make it an array
        this[p] = [this[p]];
      }
      this[p].forEach(function (image) {
        if(typeof(image) != 'object') {
          // it’s a string
          // make it an object
          image = {url: image};
        }
        var caption = image.caption ? '<image:caption><![CDATA['+image.caption+']]></image:caption>' : '';
        var geoLocation = image.geoLocation ? '<image:geo_location>'+image.geoLocation+'</image:geo_location>' : '';
        var title = image.title ? '<image:title><![CDATA['+image.title+']]></image:title>' : '';
        var license = image.license ? '<image:license>'+image.license+'</image:license>' : '';

        imagexml += '<image:image><image:loc>' + image.url + '</image:loc>' + caption + geoLocation + title + license + '</image
:image> ';
      });

      xml = xml.replace('{' + p + '}', imagexml);

    } else if (this[p] && p == 'video') {
      var videoxml = '';
      // Image handling
      if (typeof(this[p]) != 'object' || this[p].length == undefined) {
        // make it an array
        this[p] = [this[p]];
      }
      this[p].forEach(function (video) {
        if(typeof(video) != 'object' || !video.thumbnail_loc || !video.title || !video.description) {
          // has to be an object and include required categories https://developers.google.com/webmasters/videosearch/sitemaps
          throw new err.InvalidVideoFormat();
        }
        videoxml += '<video:video>' +
          '<video:thumbnail_loc>' + video.thumbnail_loc + '</video:thumbnail_loc>' +
          '<video:title><![CDATA[' + video.title + ']]></video:title>' +
          '<video:description><![CDATA[' + video.description + ']]></video:description>';
        if (video.content_loc)
          videoxml += '<video:content_loc>' + video.content_loc + '</video:content_loc>';
        if (video.player_loc)
          videoxml += '<video:player_loc>' + video.player_loc + '</video:player_loc>';
        if (video.duration)
          videoxml += '<video:duration>' + video.duration + '</video:duration>';
        if (video.expiration_date)
          videoxml += '<video:expiration_date>' + video.expiration_date + '</video:expiration_date>';
        if (video.rating)
          videoxml += '<video:rating>' + video.rating + '</video:rating>';
        if (video.view_count)
          videoxml += '<video:view_count>' + video.view_count + '</video:view_count>';
        if (video.publication_date)
          videoxml += '<video:publication_date>' + video.publication_date + '</video:publication_date>';
        if (video.family_friendly)
          videoxml += '<video:family_friendly>' + video.family_friendly + '</video:family_friendly>';
        if (video.tag)
          videoxml += '<video:tag>' + video.tag + '</video:tag>';
        if (video.category)
          videoxml += '<video:category>' + video.category + '</video:category>';
        if (video.restriction)
          videoxml += '<video:restriction>' + video.restriction + '</video:restriction>';
        if (video.gallery_loc)
          videoxml += '<video:gallery_loc>' + video.gallery_loc + '</video:gallery_loc>';
        if (video.price)
          videoxml += '<video:price>' + video.price + '</video:price>';
        if (video.requires_subscription)
          videoxml += '<video:requires_subscription>' + video.requires_subscription + '</video:requires_subscription>';
        if (video.uploader)
          videoxml += '<video:uploader>' + video.uploader + ...
```
- example usage
```shell
...
'''javascript
var sm = require('sitemap')
// Creates a sitemap object given the input configuration with URLs
var sitemap = sm.createSitemap({ options });
// Generates XML with a callback function
sitemap.toXML( function(err, xml){ if (!err){ console.log(xml) } });
// Gives you a string containing the XML data
var xml = sitemap.toString();
'''

### Example of using sitemap.js with [express](https://github.com/visionmedia/express):

'''javascript
var express = require('express')
, sm = require('sitemap');
...
```

#### <a name="apidoc.element.sitemap.SitemapItem.prototype.toXML"></a>[function <span class="apidocSignatureSpan">sitemap.SitemapItem.prototype.</span>toXML ()](#apidoc.element.sitemap.SitemapItem.prototype.toXML)
- description and source-code
```javascript
toXML = function () {
  return this.toString();
}
```
- example usage
```shell
...
The main functions you want to use in the sitemap module are

'''javascript
var sm = require('sitemap')
// Creates a sitemap object given the input configuration with URLs
var sitemap = sm.createSitemap({ options });
// Generates XML with a callback function
sitemap.toXML( function(err, xml){ if (!err){ console.log(xml) } });
// Gives you a string containing the XML data
var xml = sitemap.toString();
'''

### Example of using sitemap.js with [express](https://github.com/visionmedia/express):

'''javascript
...
```



# <a name="apidoc.module.sitemap.errors"></a>[module sitemap.errors](#apidoc.module.sitemap.errors)

#### <a name="apidoc.element.sitemap.errors.ChangeFreqInvalidError"></a>[function <span class="apidocSignatureSpan">sitemap.errors.</span>ChangeFreqInvalidError (message)](#apidoc.element.sitemap.errors.ChangeFreqInvalidError)
- description and source-code
```javascript
ChangeFreqInvalidError = function (message) {
  this.name = 'ChangeFreqInvalidError';
  this.message = message || 'changefreq is invalid';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.errors.InvalidVideoFormat"></a>[function <span class="apidocSignatureSpan">sitemap.errors.</span>InvalidVideoFormat (message)](#apidoc.element.sitemap.errors.InvalidVideoFormat)
- description and source-code
```javascript
InvalidVideoFormat = function (message) {
  this.name = 'InvalidVideoFormat';
  this.message = message || 'must include thumbnail_loc, title and description fields for videos ';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.errors.NoURLError"></a>[function <span class="apidocSignatureSpan">sitemap.errors.</span>NoURLError (message)](#apidoc.element.sitemap.errors.NoURLError)
- description and source-code
```javascript
NoURLError = function (message) {
  this.name = 'NoURLError';
  this.message = message || 'URL is required';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.errors.NoURLProtocolError"></a>[function <span class="apidocSignatureSpan">sitemap.errors.</span>NoURLProtocolError (message)](#apidoc.element.sitemap.errors.NoURLProtocolError)
- description and source-code
```javascript
NoURLProtocolError = function (message) {
  this.name = 'NoURLProtocolError';
  this.message = message || 'Protocol is required';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.errors.PriorityInvalidError"></a>[function <span class="apidocSignatureSpan">sitemap.errors.</span>PriorityInvalidError (message)](#apidoc.element.sitemap.errors.PriorityInvalidError)
- description and source-code
```javascript
PriorityInvalidError = function (message) {
  this.name = 'PriorityInvalidError';
  this.message = message || 'priority is invalid';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.errors.UndefinedTargetFolder"></a>[function <span class="apidocSignatureSpan">sitemap.errors.</span>UndefinedTargetFolder (message)](#apidoc.element.sitemap.errors.UndefinedTargetFolder)
- description and source-code
```javascript
UndefinedTargetFolder = function (message) {
  this.name = 'UndefinedTargetFolder';
  this.message = message || 'Target folder must exist';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sitemap.utils"></a>[module sitemap.utils](#apidoc.module.sitemap.utils)

#### <a name="apidoc.element.sitemap.utils.abort"></a>[function <span class="apidocSignatureSpan">sitemap.utils.</span>abort (str)](#apidoc.element.sitemap.utils.abort)
- description and source-code
```javascript
abort = function (str) {
  console.error(str);
  process.exit(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.utils.chunkArray"></a>[function <span class="apidocSignatureSpan">sitemap.utils.</span>chunkArray (arr, chunkSize)](#apidoc.element.sitemap.utils.chunkArray)
- description and source-code
```javascript
chunkArray = function (arr, chunkSize) {
  var lists = _.groupBy(arr, function (element, index) {
    return Math.floor(index / chunkSize);
  });
  lists = _.toArray(lists);
  return lists;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.utils.distinctArray"></a>[function <span class="apidocSignatureSpan">sitemap.utils.</span>distinctArray (arr)](#apidoc.element.sitemap.utils.distinctArray)
- description and source-code
```javascript
distinctArray = function (arr) {
  var hash = {}
    , res = []
    , arr_length = arr.length;
  while (arr_length--) {
    hash[arr[arr_length]] = true;
  }
  for (key in hash) {
    res.push(key);
  }
  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.utils.getTimestamp"></a>[function <span class="apidocSignatureSpan">sitemap.utils.</span>getTimestamp ()](#apidoc.element.sitemap.utils.getTimestamp)
- description and source-code
```javascript
getTimestamp = function () {
  return (new Date()).getTime();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.utils.getTimestampFromDate"></a>[function <span class="apidocSignatureSpan">sitemap.utils.</span>getTimestampFromDate (dt, bRealtime)](#apidoc.element.sitemap.utils.getTimestampFromDate)
- description and source-code
```javascript
getTimestampFromDate = function (dt, bRealtime) {
  var timestamp = [dt.getUTCFullYear(), exports.lpad(dt.getUTCMonth() + 1, 2),
    exports.lpad(dt.getUTCDate(), 2)].join('-');

  // Indicate that lastmod should include minutes and seconds (and timezone)
  if (bRealtime && bRealtime === true) {
    timestamp += 'T';
    timestamp += [exports.lpad(dt.getUTCHours(), 2),
      exports.lpad(dt.getUTCMinutes(), 2),
      exports.lpad(dt.getUTCSeconds(), 2)
    ].join(':');
    timestamp += 'Z';
  }

  return timestamp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.utils.htmlEscape"></a>[function <span class="apidocSignatureSpan">sitemap.utils.</span>htmlEscape (text)](#apidoc.element.sitemap.utils.htmlEscape)
- description and source-code
```javascript
htmlEscape = function (text) {
  return text.replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;').replace(/"/g, '&quot;').replace(/'/g, '&#039;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sitemap.utils.lpad"></a>[function <span class="apidocSignatureSpan">sitemap.utils.</span>lpad (n, len, chr)](#apidoc.element.sitemap.utils.lpad)
- description and source-code
```javascript
lpad = function (n, len, chr) {
  var res = n.toString()
    , chr = chr || '0'
    , leading = (res.substr(0, 1) === '-');

  //If left side of string is a minus sign (negative number), we want to ignore that in the padding process
  if (leading) {
    res = res.substr(1); //cut-off the leading '-'
  }

  while (res.length < len) {
    res = chr + res;
  }

  if (leading) { //If we initially cutoff the leading '-', we add it again here
    res = '-' + res;
  }

  return res;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)

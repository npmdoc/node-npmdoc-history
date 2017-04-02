# api documentation for  [history (v4.6.1)](https://github.com/reacttraining/history#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-history.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-history) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-history.svg)](https://travis-ci.org/npmdoc/node-npmdoc-history)
#### Manage session history with JavaScript

[![NPM](https://nodei.co/npm/history.png?downloads=true)](https://www.npmjs.com/package/history)

[![apidoc](https://npmdoc.github.io/node-npmdoc-history/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-history_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-history/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-history/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Michael Jackson"
    },
    "browserify": {
        "transform": [
            "loose-envify"
        ]
    },
    "bugs": {
        "url": "https://github.com/reacttraining/history/issues"
    },
    "dependencies": {
        "invariant": "^2.2.1",
        "loose-envify": "^1.2.0",
        "resolve-pathname": "^2.0.0",
        "value-equal": "^0.2.0",
        "warning": "^3.0.0"
    },
    "description": "Manage session history with JavaScript",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-core": "^6.23.1",
        "babel-eslint": "^7.0.0",
        "babel-loader": "^6.2.10",
        "babel-plugin-dev-expression": "^0.2.1",
        "babel-plugin-transform-object-assign": "^6.8.0",
        "babel-preset-es2015": "^6.9.0",
        "babel-preset-stage-1": "^6.5.0",
        "eslint": "^3.3.0",
        "eslint-plugin-import": "^2.0.0",
        "expect": "^1.20.1",
        "gzip-size": "^3.0.0",
        "in-publish": "^2.0.0",
        "karma": "^1.2.0",
        "karma-browserstack-launcher": "^1.0.1",
        "karma-chrome-launcher": "^2.0.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.0.1",
        "karma-mocha-reporter": "^2.0.4",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-webpack": "^2.0.1",
        "mocha": "^3.0.2",
        "pretty-bytes": "^4.0.2",
        "readline-sync": "^1.4.4",
        "webpack": "^1.13.1",
        "webpack-dev-server": "^1.14.1"
    },
    "directories": {},
    "dist": {
        "shasum": "911cf8eb65728555a94f2b12780a0c531a14d2fd",
        "tarball": "https://registry.npmjs.org/history/-/history-4.6.1.tgz"
    },
    "files": [
        "DOMUtils.js",
        "ExecutionEnvironment.js",
        "LocationUtils.js",
        "PathUtils.js",
        "createBrowserHistory.js",
        "createHashHistory.js",
        "createMemoryHistory.js",
        "createTransitionManager.js",
        "es",
        "index.js",
        "umd"
    ],
    "gitHead": "a647c5d1e5442998855700195b80a8a60b7f7656",
    "homepage": "https://github.com/reacttraining/history#readme",
    "keywords": [
        "history",
        "location"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "mjackson",
            "email": "mjijackson@gmail.com"
        }
    ],
    "name": "history",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/reacttraining/history.git"
    },
    "scripts": {
        "build": "node ./tools/build.js",
        "clean": "git clean -e '!node_modules' -fdX .",
        "lint": "eslint modules",
        "prepublish": "node ./tools/build.js",
        "release": "node ./tools/release.js",
        "start": "webpack-dev-server -d --content-base ./ --history-api-fallback --inline modules/index.js",
        "test": "karma start --single-run"
    },
    "version": "4.6.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module history](#apidoc.module.history)
1.  boolean <span class="apidocSignatureSpan">history.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.</span>createBrowserHistory ()](#apidoc.element.history.createBrowserHistory)
1.  [function <span class="apidocSignatureSpan">history.</span>createHashHistory ()](#apidoc.element.history.createHashHistory)
1.  [function <span class="apidocSignatureSpan">history.</span>createLocation (path, state, key, currentLocation)](#apidoc.element.history.createLocation)
1.  [function <span class="apidocSignatureSpan">history.</span>createMemoryHistory ()](#apidoc.element.history.createMemoryHistory)
1.  [function <span class="apidocSignatureSpan">history.</span>createPath (location)](#apidoc.element.history.createPath)
1.  [function <span class="apidocSignatureSpan">history.</span>locationsAreEqual (a, b)](#apidoc.element.history.locationsAreEqual)
1.  [function <span class="apidocSignatureSpan">history.</span>parsePath (path)](#apidoc.element.history.parsePath)
1.  object <span class="apidocSignatureSpan"></span>history
1.  object <span class="apidocSignatureSpan">history.</span>DOMUtils
1.  object <span class="apidocSignatureSpan">history.</span>LocationUtils
1.  object <span class="apidocSignatureSpan">history.</span>PathUtils
1.  object <span class="apidocSignatureSpan">history.</span>createTransitionManager

#### [module history.DOMUtils](#apidoc.module.history.DOMUtils)
1.  boolean <span class="apidocSignatureSpan">history.DOMUtils.</span>__esModule
1.  boolean <span class="apidocSignatureSpan">history.DOMUtils.</span>canUseDOM
1.  [function <span class="apidocSignatureSpan">history.DOMUtils.</span>addEventListener (node, event, listener)](#apidoc.element.history.DOMUtils.addEventListener)
1.  [function <span class="apidocSignatureSpan">history.DOMUtils.</span>getConfirmation (message, callback)](#apidoc.element.history.DOMUtils.getConfirmation)
1.  [function <span class="apidocSignatureSpan">history.DOMUtils.</span>isExtraneousPopstateEvent (event)](#apidoc.element.history.DOMUtils.isExtraneousPopstateEvent)
1.  [function <span class="apidocSignatureSpan">history.DOMUtils.</span>removeEventListener (node, event, listener)](#apidoc.element.history.DOMUtils.removeEventListener)
1.  [function <span class="apidocSignatureSpan">history.DOMUtils.</span>supportsGoWithoutReloadUsingHash ()](#apidoc.element.history.DOMUtils.supportsGoWithoutReloadUsingHash)
1.  [function <span class="apidocSignatureSpan">history.DOMUtils.</span>supportsHistory ()](#apidoc.element.history.DOMUtils.supportsHistory)
1.  [function <span class="apidocSignatureSpan">history.DOMUtils.</span>supportsPopStateOnHashChange ()](#apidoc.element.history.DOMUtils.supportsPopStateOnHashChange)

#### [module history.LocationUtils](#apidoc.module.history.LocationUtils)
1.  boolean <span class="apidocSignatureSpan">history.LocationUtils.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.LocationUtils.</span>createLocation (path, state, key, currentLocation)](#apidoc.element.history.LocationUtils.createLocation)
1.  [function <span class="apidocSignatureSpan">history.LocationUtils.</span>locationsAreEqual (a, b)](#apidoc.element.history.LocationUtils.locationsAreEqual)

#### [module history.PathUtils](#apidoc.module.history.PathUtils)
1.  boolean <span class="apidocSignatureSpan">history.PathUtils.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.PathUtils.</span>addLeadingSlash (path)](#apidoc.element.history.PathUtils.addLeadingSlash)
1.  [function <span class="apidocSignatureSpan">history.PathUtils.</span>createPath (location)](#apidoc.element.history.PathUtils.createPath)
1.  [function <span class="apidocSignatureSpan">history.PathUtils.</span>parsePath (path)](#apidoc.element.history.PathUtils.parsePath)
1.  [function <span class="apidocSignatureSpan">history.PathUtils.</span>stripLeadingSlash (path)](#apidoc.element.history.PathUtils.stripLeadingSlash)
1.  [function <span class="apidocSignatureSpan">history.PathUtils.</span>stripPrefix (path, prefix)](#apidoc.element.history.PathUtils.stripPrefix)
1.  [function <span class="apidocSignatureSpan">history.PathUtils.</span>stripTrailingSlash (path)](#apidoc.element.history.PathUtils.stripTrailingSlash)

#### [module history.createBrowserHistory](#apidoc.module.history.createBrowserHistory)
1.  boolean <span class="apidocSignatureSpan">history.createBrowserHistory.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.createBrowserHistory.</span>default ()](#apidoc.element.history.createBrowserHistory.default)

#### [module history.createHashHistory](#apidoc.module.history.createHashHistory)
1.  boolean <span class="apidocSignatureSpan">history.createHashHistory.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.createHashHistory.</span>default ()](#apidoc.element.history.createHashHistory.default)

#### [module history.createMemoryHistory](#apidoc.module.history.createMemoryHistory)
1.  boolean <span class="apidocSignatureSpan">history.createMemoryHistory.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.createMemoryHistory.</span>default ()](#apidoc.element.history.createMemoryHistory.default)

#### [module history.createTransitionManager](#apidoc.module.history.createTransitionManager)
1.  boolean <span class="apidocSignatureSpan">history.createTransitionManager.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.createTransitionManager.</span>default ()](#apidoc.element.history.createTransitionManager.default)

#### [module history.history](#apidoc.module.history.history)
1.  boolean <span class="apidocSignatureSpan">history.history.</span>__esModule
1.  [function <span class="apidocSignatureSpan">history.history.</span>createBrowserHistory ()](#apidoc.element.history.history.createBrowserHistory)
1.  [function <span class="apidocSignatureSpan">history.history.</span>createHashHistory ()](#apidoc.element.history.history.createHashHistory)
1.  [function <span class="apidocSignatureSpan">history.history.</span>createLocation (path, state, key, currentLocation)](#apidoc.element.history.history.createLocation)
1.  [function <span class="apidocSignatureSpan">history.history.</span>createMemoryHistory ()](#apidoc.element.history.history.createMemoryHistory)
1.  [function <span class="apidocSignatureSpan">history.history.</span>createPath (location)](#apidoc.element.history.history.createPath)
1.  [function <span class="apidocSignatureSpan">history.history.</span>locationsAreEqual (a, b)](#apidoc.element.history.history.locationsAreEqual)
1.  [function <span class="apidocSignatureSpan">history.history.</span>parsePath (path)](#apidoc.element.history.history.parsePath)



# <a name="apidoc.module.history"></a>[module history](#apidoc.module.history)

#### <a name="apidoc.element.history.createBrowserHistory"></a>[function <span class="apidocSignatureSpan">history.</span>createBrowserHistory ()](#apidoc.element.history.createBrowserHistory)
- description and source-code
```javascript
function createBrowserHistory() {
  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

  (0, _invariant2.default)(_DOMUtils.canUseDOM, 'Browser history needs a DOM');

  var globalHistory = window.history;
  var canUseHistory = (0, _DOMUtils.supportsHistory)();
  var needsHashChangeListener = !(0, _DOMUtils.supportsPopStateOnHashChange)();

  var _props$forceRefresh = props.forceRefresh,
      forceRefresh = _props$forceRefresh === undefined ? false : _props$forceRefresh,
      _props$getUserConfirm = props.getUserConfirmation,
      getUserConfirmation = _props$getUserConfirm === undefined ? _DOMUtils.getConfirmation : _props$getUserConfirm,
      _props$keyLength = props.keyLength,
      keyLength = _props$keyLength === undefined ? 6 : _props$keyLength;

  var basename = props.basename ? (0, _PathUtils.stripTrailingSlash)((0, _PathUtils.addLeadingSlash)(props.basename)) : '';

  var getDOMLocation = function getDOMLocation(historyState) {
    var _ref = historyState || {},
        key = _ref.key,
        state = _ref.state;

    var _window$location = window.location,
        pathname = _window$location.pathname,
        search = _window$location.search,
        hash = _window$location.hash;


    var path = pathname + search + hash;

    if (basename) path = (0, _PathUtils.stripPrefix)(path, basename);

    return _extends({}, (0, _PathUtils.parsePath)(path), {
      state: state,
      key: key
    });
  };

  var createKey = function createKey() {
    return Math.random().toString(36).substr(2, keyLength);
  };

  var transitionManager = (0, _createTransitionManager2.default)();

  var setState = function setState(nextState) {
    _extends(history, nextState);

    history.length = globalHistory.length;

    transitionManager.notifyListeners(history.location, history.action);
  };

  var handlePopState = function handlePopState(event) {
    // Ignore extraneous popstate events in WebKit.
    if ((0, _DOMUtils.isExtraneousPopstateEvent)(event)) return;

    handlePop(getDOMLocation(event.state));
  };

  var handleHashChange = function handleHashChange() {
    handlePop(getDOMLocation(getHistoryState()));
  };

  var forceNextPop = false;

  var handlePop = function handlePop(location) {
    if (forceNextPop) {
      forceNextPop = false;
      setState();
    } else {
      var action = 'POP';

      transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
        if (ok) {
          setState({ action: action, location: location });
        } else {
          revertPop(location);
        }
      });
    }
  };

  var revertPop = function revertPop(fromLocation) {
    var toLocation = history.location;

    // TODO: We could probably make this more reliable by
    // keeping a list of keys we've seen in sessionStorage.
    // Instead, we just default to 0 for keys we don't know.

    var toIndex = allKeys.indexOf(toLocation.key);

    if (toIndex === -1) toIndex = 0;

    var fromIndex = allKeys.indexOf(fromLocation.key);

    if (fromIndex === -1) fromIndex = 0;

    var delta = toIndex - fromIndex;

    if (delta) {
      forceNextPop = true;
      go(delta);
    }
  };

  var initialLocation = getDOMLocation(getHistoryState());
  var allKeys = [initialLocation.key];

  // Public interface

  var createHref = function createHref(location) {
    return basename + (0, _PathUtils.createPath)(location);
  };

  var push = function push(path, state) {
    (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !== undefined
 && state !== undefined), 'You should avoid providing a 2nd state argument to push when the 1st ' + 'argument is a location-like
 object that already has state; it is ignored');

    var action = 'PUSH';
    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      var href = createHref(location);
      var key = l ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.createHashHistory"></a>[function <span class="apidocSignatureSpan">history.</span>createHashHistory ()](#apidoc.element.history.createHashHistory)
- description and source-code
```javascript
function createHashHistory() {
  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

  (0, _invariant2.default)(_DOMUtils.canUseDOM, 'Hash history needs a DOM');

  var globalHistory = window.history;
  var canGoWithoutReload = (0, _DOMUtils.supportsGoWithoutReloadUsingHash)();

  var _props$getUserConfirm = props.getUserConfirmation,
      getUserConfirmation = _props$getUserConfirm === undefined ? _DOMUtils.getConfirmation : _props$getUserConfirm,
      _props$hashType = props.hashType,
      hashType = _props$hashType === undefined ? 'slash' : _props$hashType;

  var basename = props.basename ? (0, _PathUtils.stripTrailingSlash)((0, _PathUtils.addLeadingSlash)(props.basename)) : '';

  var _HashPathCoders$hashT = HashPathCoders[hashType],
      encodePath = _HashPathCoders$hashT.encodePath,
      decodePath = _HashPathCoders$hashT.decodePath;


  var getDOMLocation = function getDOMLocation() {
    var path = decodePath(getHashPath());

    if (basename) path = (0, _PathUtils.stripPrefix)(path, basename);

    return (0, _PathUtils.parsePath)(path);
  };

  var transitionManager = (0, _createTransitionManager2.default)();

  var setState = function setState(nextState) {
    _extends(history, nextState);

    history.length = globalHistory.length;

    transitionManager.notifyListeners(history.location, history.action);
  };

  var forceNextPop = false;
  var ignorePath = null;

  var handleHashChange = function handleHashChange() {
    var path = getHashPath();
    var encodedPath = encodePath(path);

    if (path !== encodedPath) {
      // Ensure we always have a properly-encoded hash.
      replaceHashPath(encodedPath);
    } else {
      var location = getDOMLocation();
      var prevLocation = history.location;

      if (!forceNextPop && (0, _LocationUtils.locationsAreEqual)(prevLocation, location)) return; // A hashchange doesn't always
 == location change.

      if (ignorePath === (0, _PathUtils.createPath)(location)) return; // Ignore this change; we already setState in push/replace
.

      ignorePath = null;

      handlePop(location);
    }
  };

  var handlePop = function handlePop(location) {
    if (forceNextPop) {
      forceNextPop = false;
      setState();
    } else {
      var action = 'POP';

      transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
        if (ok) {
          setState({ action: action, location: location });
        } else {
          revertPop(location);
        }
      });
    }
  };

  var revertPop = function revertPop(fromLocation) {
    var toLocation = history.location;

    // TODO: We could probably make this more reliable by
    // keeping a list of paths we've seen in sessionStorage.
    // Instead, we just default to 0 for paths we don't know.

    var toIndex = allPaths.lastIndexOf((0, _PathUtils.createPath)(toLocation));

    if (toIndex === -1) toIndex = 0;

    var fromIndex = allPaths.lastIndexOf((0, _PathUtils.createPath)(fromLocation));

    if (fromIndex === -1) fromIndex = 0;

    var delta = toIndex - fromIndex;

    if (delta) {
      forceNextPop = true;
      go(delta);
    }
  };

  // Ensure the hash is encoded properly before doing anything else.
  var path = getHashPath();
  var encodedPath = encodePath(path);

  if (path !== encodedPath) replaceHashPath(encodedPath);

  var initialLocation = getDOMLocation();
  var allPaths = [(0, _PathUtils.createPath)(initialLocation)];

  // Public interface

  var createHref = function createHref(location) {
    return '#' + encodePath(basename + (0, _PathUtils.createPath)(location));
  };

  var push = function push(path, state) {
    (0, _warning2.default)(state === undefined, 'Hash history cannot push state; it is ignored');

    var action = 'PUSH';
    var location = (0, _LocationUtils.createLocation)(path, undefined, undefined, history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      var path = (0, _PathUtils.createPath)(location);
      var en ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.createLocation"></a>[function <span class="apidocSignatureSpan">history.</span>createLocation (path, state, key, currentLocation)](#apidoc.element.history.createLocation)
- description and source-code
```javascript
function createLocation(path, state, key, currentLocation) {
  var location = void 0;
  if (typeof path === 'string') {
    // Two-arg form: push(path, state)
    location = (0, _PathUtils.parsePath)(path);
    location.state = state;
  } else {
    // One-arg form: push(location)
    location = _extends({}, path);

    if (location.pathname === undefined) location.pathname = '';

    if (location.search) {
      if (location.search.charAt(0) !== '?') location.search = '?' + location.search;
    } else {
      location.search = '';
    }

    if (location.hash) {
      if (location.hash.charAt(0) !== '#') location.hash = '#' + location.hash;
    } else {
      location.hash = '';
    }

    if (state !== undefined && location.state === undefined) location.state = state;
  }

  location.key = key;

  if (currentLocation) {
    // Resolve incomplete/relative pathname relative to current location.
    if (!location.pathname) {
      location.pathname = currentLocation.pathname;
    } else if (location.pathname.charAt(0) !== '/') {
      location.pathname = (0, _resolvePathname2.default)(location.pathname, currentLocation.pathname);
    }
  }

  return location;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.createMemoryHistory"></a>[function <span class="apidocSignatureSpan">history.</span>createMemoryHistory ()](#apidoc.element.history.createMemoryHistory)
- description and source-code
```javascript
function createMemoryHistory() {
  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};
  var getUserConfirmation = props.getUserConfirmation,
      _props$initialEntries = props.initialEntries,
      initialEntries = _props$initialEntries === undefined ? ['/'] : _props$initialEntries,
      _props$initialIndex = props.initialIndex,
      initialIndex = _props$initialIndex === undefined ? 0 : _props$initialIndex,
      _props$keyLength = props.keyLength,
      keyLength = _props$keyLength === undefined ? 6 : _props$keyLength;


  var transitionManager = (0, _createTransitionManager2.default)();

  var setState = function setState(nextState) {
    _extends(history, nextState);

    history.length = history.entries.length;

    transitionManager.notifyListeners(history.location, history.action);
  };

  var createKey = function createKey() {
    return Math.random().toString(36).substr(2, keyLength);
  };

  var index = clamp(initialIndex, 0, initialEntries.length - 1);
  var entries = initialEntries.map(function (entry) {
    return typeof entry === 'string' ? (0, _LocationUtils.createLocation)(entry, undefined, createKey()) : (0, _LocationUtils.createLocation
)(entry, undefined, entry.key || createKey());
  });

  // Public interface

  var createHref = _PathUtils.createPath;

  var push = function push(path, state) {
    (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !== undefined
 && state !== undefined), 'You should avoid providing a 2nd state argument to push when the 1st ' + 'argument is a location-like
 object that already has state; it is ignored');

    var action = 'PUSH';
    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      var prevIndex = history.index;
      var nextIndex = prevIndex + 1;

      var nextEntries = history.entries.slice(0);
      if (nextEntries.length > nextIndex) {
        nextEntries.splice(nextIndex, nextEntries.length - nextIndex, location);
      } else {
        nextEntries.push(location);
      }

      setState({
        action: action,
        location: location,
        index: nextIndex,
        entries: nextEntries
      });
    });
  };

  var replace = function replace(path, state) {
    (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !== undefined
 && state !== undefined), 'You should avoid providing a 2nd state argument to replace when the 1st ' + 'argument is a location-like
 object that already has state; it is ignored');

    var action = 'REPLACE';
    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      history.entries[history.index] = location;

      setState({ action: action, location: location });
    });
  };

  var go = function go(n) {
    var nextIndex = clamp(history.index + n, 0, history.entries.length - 1);

    var action = 'POP';
    var location = history.entries[nextIndex];

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (ok) {
        setState({
          action: action,
          location: location,
          index: nextIndex
        });
      } else {
        // Mimic the behavior of DOM histories by
        // causing a render after a cancelled POP.
        setState();
      }
    });
  };

  var goBack = function goBack() {
    return go(-1);
  };

  var goForward = function goForward() {
    return go(1);
  };

  var canGo = function canGo(n) {
    var nextIndex = history.index + n;
    return nextIndex >= 0 && nextIndex < history.entries.length;
  };

  var block = function block() {
    var prompt = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : false;
    return transitionManag ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.createPath"></a>[function <span class="apidocSignatureSpan">history.</span>createPath (location)](#apidoc.element.history.createPath)
- description and source-code
```javascript
function createPath(location) {
  var pathname = location.pathname,
      search = location.search,
      hash = location.hash;


  var path = encodeURI(pathname || '/');

  if (search && search !== '?') path += search.charAt(0) === '?' ? search : '?' + search;

  if (hash && hash !== '#') path += hash.charAt(0) === '#' ? hash : '#' + hash;

  return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.locationsAreEqual"></a>[function <span class="apidocSignatureSpan">history.</span>locationsAreEqual (a, b)](#apidoc.element.history.locationsAreEqual)
- description and source-code
```javascript
function locationsAreEqual(a, b) {
  return a.pathname === b.pathname && a.search === b.search && a.hash === b.hash && a.key === b.key && (0, _valueEqual2.default)(
a.state, b.state);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.parsePath"></a>[function <span class="apidocSignatureSpan">history.</span>parsePath (path)](#apidoc.element.history.parsePath)
- description and source-code
```javascript
function parsePath(path) {
  var pathname = path || '/';
  var search = '';
  var hash = '';

  var hashIndex = pathname.indexOf('#');
  if (hashIndex !== -1) {
    hash = pathname.substr(hashIndex);
    pathname = pathname.substr(0, hashIndex);
  }

  var searchIndex = pathname.indexOf('?');
  if (searchIndex !== -1) {
    search = pathname.substr(searchIndex);
    pathname = pathname.substr(0, searchIndex);
  }

  pathname = decodeURI(pathname);

  return {
    pathname: pathname,
    search: search === '?' ? '' : search,
    hash: hash === '#' ? '' : hash
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.DOMUtils"></a>[module history.DOMUtils](#apidoc.module.history.DOMUtils)

#### <a name="apidoc.element.history.DOMUtils.addEventListener"></a>[function <span class="apidocSignatureSpan">history.DOMUtils.</span>addEventListener (node, event, listener)](#apidoc.element.history.DOMUtils.addEventListener)
- description and source-code
```javascript
function addEventListener(node, event, listener) {
  return node.addEventListener ? node.addEventListener(event, listener, false) : node.attachEvent('on' + event, listener);
}
```
- example usage
```shell
...

'use strict';

exports.__esModule = true;
var canUseDOM = exports.canUseDOM = !!(typeof window !== 'undefined' && window.document && window.document.createElement);

var addEventListener = exports.addEventListener = function addEventListener(node, event, listener) {
  return node.addEventListener ? node.addEventListener(event, listener, false) : node.attachEvent('on' + event, listener);
};

var removeEventListener = exports.removeEventListener = function removeEventListener(node, event, listener) {
  return node.removeEventListener ? node.removeEventListener(event, listener, false) : node.detachEvent('on' + event, listener);
};

var getConfirmation = exports.getConfirmation = function getConfirmation(message, callback) {
...
```

#### <a name="apidoc.element.history.DOMUtils.getConfirmation"></a>[function <span class="apidocSignatureSpan">history.DOMUtils.</span>getConfirmation (message, callback)](#apidoc.element.history.DOMUtils.getConfirmation)
- description and source-code
```javascript
function getConfirmation(message, callback) {
  return callback(window.confirm(message));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.DOMUtils.isExtraneousPopstateEvent"></a>[function <span class="apidocSignatureSpan">history.DOMUtils.</span>isExtraneousPopstateEvent (event)](#apidoc.element.history.DOMUtils.isExtraneousPopstateEvent)
- description and source-code
```javascript
function isExtraneousPopstateEvent(event) {
  return event.state === undefined && navigator.userAgent.indexOf('CriOS') === -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.DOMUtils.removeEventListener"></a>[function <span class="apidocSignatureSpan">history.DOMUtils.</span>removeEventListener (node, event, listener)](#apidoc.element.history.DOMUtils.removeEventListener)
- description and source-code
```javascript
function removeEventListener(node, event, listener) {
  return node.removeEventListener ? node.removeEventListener(event, listener, false) : node.detachEvent('on' + event, listener);
}
```
- example usage
```shell
...
var canUseDOM = exports.canUseDOM = !!(typeof window !== 'undefined' && window.document && window.document.createElement);

var addEventListener = exports.addEventListener = function addEventListener(node, event, listener) {
  return node.addEventListener ? node.addEventListener(event, listener, false) : node.attachEvent('on' + event, listener);
};

var removeEventListener = exports.removeEventListener = function removeEventListener(node, event, listener) {
  return node.removeEventListener ? node.removeEventListener(event, listener, false) : node.detachEvent('on' + event, listener);
};

var getConfirmation = exports.getConfirmation = function getConfirmation(message, callback) {
  return callback(window.confirm(message));
}; // eslint-disable-line no-alert

/**
...
```

#### <a name="apidoc.element.history.DOMUtils.supportsGoWithoutReloadUsingHash"></a>[function <span class="apidocSignatureSpan">history.DOMUtils.</span>supportsGoWithoutReloadUsingHash ()](#apidoc.element.history.DOMUtils.supportsGoWithoutReloadUsingHash)
- description and source-code
```javascript
function supportsGoWithoutReloadUsingHash() {
  return window.navigator.userAgent.indexOf('Firefox') === -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.DOMUtils.supportsHistory"></a>[function <span class="apidocSignatureSpan">history.DOMUtils.</span>supportsHistory ()](#apidoc.element.history.DOMUtils.supportsHistory)
- description and source-code
```javascript
function supportsHistory() {
  var ua = window.navigator.userAgent;

  if ((ua.indexOf('Android 2.') !== -1 || ua.indexOf('Android 4.0') !== -1) && ua.indexOf('Mobile Safari') !== -1 && ua.indexOf('
Chrome') === -1 && ua.indexOf('Windows Phone') === -1) return false;

  return window.history && 'pushState' in window.history;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.DOMUtils.supportsPopStateOnHashChange"></a>[function <span class="apidocSignatureSpan">history.DOMUtils.</span>supportsPopStateOnHashChange ()](#apidoc.element.history.DOMUtils.supportsPopStateOnHashChange)
- description and source-code
```javascript
function supportsPopStateOnHashChange() {
  return window.navigator.userAgent.indexOf('Trident') === -1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.LocationUtils"></a>[module history.LocationUtils](#apidoc.module.history.LocationUtils)

#### <a name="apidoc.element.history.LocationUtils.createLocation"></a>[function <span class="apidocSignatureSpan">history.LocationUtils.</span>createLocation (path, state, key, currentLocation)](#apidoc.element.history.LocationUtils.createLocation)
- description and source-code
```javascript
function createLocation(path, state, key, currentLocation) {
  var location = void 0;
  if (typeof path === 'string') {
    // Two-arg form: push(path, state)
    location = (0, _PathUtils.parsePath)(path);
    location.state = state;
  } else {
    // One-arg form: push(location)
    location = _extends({}, path);

    if (location.pathname === undefined) location.pathname = '';

    if (location.search) {
      if (location.search.charAt(0) !== '?') location.search = '?' + location.search;
    } else {
      location.search = '';
    }

    if (location.hash) {
      if (location.hash.charAt(0) !== '#') location.hash = '#' + location.hash;
    } else {
      location.hash = '';
    }

    if (state !== undefined && location.state === undefined) location.state = state;
  }

  location.key = key;

  if (currentLocation) {
    // Resolve incomplete/relative pathname relative to current location.
    if (!location.pathname) {
      location.pathname = currentLocation.pathname;
    } else if (location.pathname.charAt(0) !== '/') {
      location.pathname = (0, _resolvePathname2.default)(location.pathname, currentLocation.pathname);
    }
  }

  return location;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.LocationUtils.locationsAreEqual"></a>[function <span class="apidocSignatureSpan">history.LocationUtils.</span>locationsAreEqual (a, b)](#apidoc.element.history.LocationUtils.locationsAreEqual)
- description and source-code
```javascript
function locationsAreEqual(a, b) {
  return a.pathname === b.pathname && a.search === b.search && a.hash === b.hash && a.key === b.key && (0, _valueEqual2.default)(
a.state, b.state);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.PathUtils"></a>[module history.PathUtils](#apidoc.module.history.PathUtils)

#### <a name="apidoc.element.history.PathUtils.addLeadingSlash"></a>[function <span class="apidocSignatureSpan">history.PathUtils.</span>addLeadingSlash (path)](#apidoc.element.history.PathUtils.addLeadingSlash)
- description and source-code
```javascript
function addLeadingSlash(path) {
  return path.charAt(0) === '/' ? path : '/' + path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.PathUtils.createPath"></a>[function <span class="apidocSignatureSpan">history.PathUtils.</span>createPath (location)](#apidoc.element.history.PathUtils.createPath)
- description and source-code
```javascript
function createPath(location) {
  var pathname = location.pathname,
      search = location.search,
      hash = location.hash;


  var path = encodeURI(pathname || '/');

  if (search && search !== '?') path += search.charAt(0) === '?' ? search : '?' + search;

  if (hash && hash !== '#') path += hash.charAt(0) === '#' ? hash : '#' + hash;

  return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.PathUtils.parsePath"></a>[function <span class="apidocSignatureSpan">history.PathUtils.</span>parsePath (path)](#apidoc.element.history.PathUtils.parsePath)
- description and source-code
```javascript
function parsePath(path) {
  var pathname = path || '/';
  var search = '';
  var hash = '';

  var hashIndex = pathname.indexOf('#');
  if (hashIndex !== -1) {
    hash = pathname.substr(hashIndex);
    pathname = pathname.substr(0, hashIndex);
  }

  var searchIndex = pathname.indexOf('?');
  if (searchIndex !== -1) {
    search = pathname.substr(searchIndex);
    pathname = pathname.substr(0, searchIndex);
  }

  pathname = decodeURI(pathname);

  return {
    pathname: pathname,
    search: search === '?' ? '' : search,
    hash: hash === '#' ? '' : hash
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.PathUtils.stripLeadingSlash"></a>[function <span class="apidocSignatureSpan">history.PathUtils.</span>stripLeadingSlash (path)](#apidoc.element.history.PathUtils.stripLeadingSlash)
- description and source-code
```javascript
function stripLeadingSlash(path) {
  return path.charAt(0) === '/' ? path.substr(1) : path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.PathUtils.stripPrefix"></a>[function <span class="apidocSignatureSpan">history.PathUtils.</span>stripPrefix (path, prefix)](#apidoc.element.history.PathUtils.stripPrefix)
- description and source-code
```javascript
function stripPrefix(path, prefix) {
  return path.indexOf(prefix) === 0 ? path.substr(prefix.length) : path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.PathUtils.stripTrailingSlash"></a>[function <span class="apidocSignatureSpan">history.PathUtils.</span>stripTrailingSlash (path)](#apidoc.element.history.PathUtils.stripTrailingSlash)
- description and source-code
```javascript
function stripTrailingSlash(path) {
  return path.charAt(path.length - 1) === '/' ? path.slice(0, -1) : path;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.createBrowserHistory"></a>[module history.createBrowserHistory](#apidoc.module.history.createBrowserHistory)

#### <a name="apidoc.element.history.createBrowserHistory.default"></a>[function <span class="apidocSignatureSpan">history.createBrowserHistory.</span>default ()](#apidoc.element.history.createBrowserHistory.default)
- description and source-code
```javascript
function createBrowserHistory() {
  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

  (0, _invariant2.default)(_DOMUtils.canUseDOM, 'Browser history needs a DOM');

  var globalHistory = window.history;
  var canUseHistory = (0, _DOMUtils.supportsHistory)();
  var needsHashChangeListener = !(0, _DOMUtils.supportsPopStateOnHashChange)();

  var _props$forceRefresh = props.forceRefresh,
      forceRefresh = _props$forceRefresh === undefined ? false : _props$forceRefresh,
      _props$getUserConfirm = props.getUserConfirmation,
      getUserConfirmation = _props$getUserConfirm === undefined ? _DOMUtils.getConfirmation : _props$getUserConfirm,
      _props$keyLength = props.keyLength,
      keyLength = _props$keyLength === undefined ? 6 : _props$keyLength;

  var basename = props.basename ? (0, _PathUtils.stripTrailingSlash)((0, _PathUtils.addLeadingSlash)(props.basename)) : '';

  var getDOMLocation = function getDOMLocation(historyState) {
    var _ref = historyState || {},
        key = _ref.key,
        state = _ref.state;

    var _window$location = window.location,
        pathname = _window$location.pathname,
        search = _window$location.search,
        hash = _window$location.hash;


    var path = pathname + search + hash;

    if (basename) path = (0, _PathUtils.stripPrefix)(path, basename);

    return _extends({}, (0, _PathUtils.parsePath)(path), {
      state: state,
      key: key
    });
  };

  var createKey = function createKey() {
    return Math.random().toString(36).substr(2, keyLength);
  };

  var transitionManager = (0, _createTransitionManager2.default)();

  var setState = function setState(nextState) {
    _extends(history, nextState);

    history.length = globalHistory.length;

    transitionManager.notifyListeners(history.location, history.action);
  };

  var handlePopState = function handlePopState(event) {
    // Ignore extraneous popstate events in WebKit.
    if ((0, _DOMUtils.isExtraneousPopstateEvent)(event)) return;

    handlePop(getDOMLocation(event.state));
  };

  var handleHashChange = function handleHashChange() {
    handlePop(getDOMLocation(getHistoryState()));
  };

  var forceNextPop = false;

  var handlePop = function handlePop(location) {
    if (forceNextPop) {
      forceNextPop = false;
      setState();
    } else {
      var action = 'POP';

      transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
        if (ok) {
          setState({ action: action, location: location });
        } else {
          revertPop(location);
        }
      });
    }
  };

  var revertPop = function revertPop(fromLocation) {
    var toLocation = history.location;

    // TODO: We could probably make this more reliable by
    // keeping a list of keys we've seen in sessionStorage.
    // Instead, we just default to 0 for keys we don't know.

    var toIndex = allKeys.indexOf(toLocation.key);

    if (toIndex === -1) toIndex = 0;

    var fromIndex = allKeys.indexOf(fromLocation.key);

    if (fromIndex === -1) fromIndex = 0;

    var delta = toIndex - fromIndex;

    if (delta) {
      forceNextPop = true;
      go(delta);
    }
  };

  var initialLocation = getDOMLocation(getHistoryState());
  var allKeys = [initialLocation.key];

  // Public interface

  var createHref = function createHref(location) {
    return basename + (0, _PathUtils.createPath)(location);
  };

  var push = function push(path, state) {
    (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !== undefined
 && state !== undefined), 'You should avoid providing a 2nd state argument to push when the 1st ' + 'argument is a location-like
 object that already has state; it is ignored');

    var action = 'PUSH';
    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      var href = createHref(location);
      var key = l ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.createHashHistory"></a>[module history.createHashHistory](#apidoc.module.history.createHashHistory)

#### <a name="apidoc.element.history.createHashHistory.default"></a>[function <span class="apidocSignatureSpan">history.createHashHistory.</span>default ()](#apidoc.element.history.createHashHistory.default)
- description and source-code
```javascript
function createHashHistory() {
  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

  (0, _invariant2.default)(_DOMUtils.canUseDOM, 'Hash history needs a DOM');

  var globalHistory = window.history;
  var canGoWithoutReload = (0, _DOMUtils.supportsGoWithoutReloadUsingHash)();

  var _props$getUserConfirm = props.getUserConfirmation,
      getUserConfirmation = _props$getUserConfirm === undefined ? _DOMUtils.getConfirmation : _props$getUserConfirm,
      _props$hashType = props.hashType,
      hashType = _props$hashType === undefined ? 'slash' : _props$hashType;

  var basename = props.basename ? (0, _PathUtils.stripTrailingSlash)((0, _PathUtils.addLeadingSlash)(props.basename)) : '';

  var _HashPathCoders$hashT = HashPathCoders[hashType],
      encodePath = _HashPathCoders$hashT.encodePath,
      decodePath = _HashPathCoders$hashT.decodePath;


  var getDOMLocation = function getDOMLocation() {
    var path = decodePath(getHashPath());

    if (basename) path = (0, _PathUtils.stripPrefix)(path, basename);

    return (0, _PathUtils.parsePath)(path);
  };

  var transitionManager = (0, _createTransitionManager2.default)();

  var setState = function setState(nextState) {
    _extends(history, nextState);

    history.length = globalHistory.length;

    transitionManager.notifyListeners(history.location, history.action);
  };

  var forceNextPop = false;
  var ignorePath = null;

  var handleHashChange = function handleHashChange() {
    var path = getHashPath();
    var encodedPath = encodePath(path);

    if (path !== encodedPath) {
      // Ensure we always have a properly-encoded hash.
      replaceHashPath(encodedPath);
    } else {
      var location = getDOMLocation();
      var prevLocation = history.location;

      if (!forceNextPop && (0, _LocationUtils.locationsAreEqual)(prevLocation, location)) return; // A hashchange doesn't always
 == location change.

      if (ignorePath === (0, _PathUtils.createPath)(location)) return; // Ignore this change; we already setState in push/replace
.

      ignorePath = null;

      handlePop(location);
    }
  };

  var handlePop = function handlePop(location) {
    if (forceNextPop) {
      forceNextPop = false;
      setState();
    } else {
      var action = 'POP';

      transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
        if (ok) {
          setState({ action: action, location: location });
        } else {
          revertPop(location);
        }
      });
    }
  };

  var revertPop = function revertPop(fromLocation) {
    var toLocation = history.location;

    // TODO: We could probably make this more reliable by
    // keeping a list of paths we've seen in sessionStorage.
    // Instead, we just default to 0 for paths we don't know.

    var toIndex = allPaths.lastIndexOf((0, _PathUtils.createPath)(toLocation));

    if (toIndex === -1) toIndex = 0;

    var fromIndex = allPaths.lastIndexOf((0, _PathUtils.createPath)(fromLocation));

    if (fromIndex === -1) fromIndex = 0;

    var delta = toIndex - fromIndex;

    if (delta) {
      forceNextPop = true;
      go(delta);
    }
  };

  // Ensure the hash is encoded properly before doing anything else.
  var path = getHashPath();
  var encodedPath = encodePath(path);

  if (path !== encodedPath) replaceHashPath(encodedPath);

  var initialLocation = getDOMLocation();
  var allPaths = [(0, _PathUtils.createPath)(initialLocation)];

  // Public interface

  var createHref = function createHref(location) {
    return '#' + encodePath(basename + (0, _PathUtils.createPath)(location));
  };

  var push = function push(path, state) {
    (0, _warning2.default)(state === undefined, 'Hash history cannot push state; it is ignored');

    var action = 'PUSH';
    var location = (0, _LocationUtils.createLocation)(path, undefined, undefined, history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      var path = (0, _PathUtils.createPath)(location);
      var en ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.createMemoryHistory"></a>[module history.createMemoryHistory](#apidoc.module.history.createMemoryHistory)

#### <a name="apidoc.element.history.createMemoryHistory.default"></a>[function <span class="apidocSignatureSpan">history.createMemoryHistory.</span>default ()](#apidoc.element.history.createMemoryHistory.default)
- description and source-code
```javascript
function createMemoryHistory() {
  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};
  var getUserConfirmation = props.getUserConfirmation,
      _props$initialEntries = props.initialEntries,
      initialEntries = _props$initialEntries === undefined ? ['/'] : _props$initialEntries,
      _props$initialIndex = props.initialIndex,
      initialIndex = _props$initialIndex === undefined ? 0 : _props$initialIndex,
      _props$keyLength = props.keyLength,
      keyLength = _props$keyLength === undefined ? 6 : _props$keyLength;


  var transitionManager = (0, _createTransitionManager2.default)();

  var setState = function setState(nextState) {
    _extends(history, nextState);

    history.length = history.entries.length;

    transitionManager.notifyListeners(history.location, history.action);
  };

  var createKey = function createKey() {
    return Math.random().toString(36).substr(2, keyLength);
  };

  var index = clamp(initialIndex, 0, initialEntries.length - 1);
  var entries = initialEntries.map(function (entry) {
    return typeof entry === 'string' ? (0, _LocationUtils.createLocation)(entry, undefined, createKey()) : (0, _LocationUtils.createLocation
)(entry, undefined, entry.key || createKey());
  });

  // Public interface

  var createHref = _PathUtils.createPath;

  var push = function push(path, state) {
    (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !== undefined
 && state !== undefined), 'You should avoid providing a 2nd state argument to push when the 1st ' + 'argument is a location-like
 object that already has state; it is ignored');

    var action = 'PUSH';
    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      var prevIndex = history.index;
      var nextIndex = prevIndex + 1;

      var nextEntries = history.entries.slice(0);
      if (nextEntries.length > nextIndex) {
        nextEntries.splice(nextIndex, nextEntries.length - nextIndex, location);
      } else {
        nextEntries.push(location);
      }

      setState({
        action: action,
        location: location,
        index: nextIndex,
        entries: nextEntries
      });
    });
  };

  var replace = function replace(path, state) {
    (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !== undefined
 && state !== undefined), 'You should avoid providing a 2nd state argument to replace when the 1st ' + 'argument is a location-like
 object that already has state; it is ignored');

    var action = 'REPLACE';
    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (!ok) return;

      history.entries[history.index] = location;

      setState({ action: action, location: location });
    });
  };

  var go = function go(n) {
    var nextIndex = clamp(history.index + n, 0, history.entries.length - 1);

    var action = 'POP';
    var location = history.entries[nextIndex];

    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
      if (ok) {
        setState({
          action: action,
          location: location,
          index: nextIndex
        });
      } else {
        // Mimic the behavior of DOM histories by
        // causing a render after a cancelled POP.
        setState();
      }
    });
  };

  var goBack = function goBack() {
    return go(-1);
  };

  var goForward = function goForward() {
    return go(1);
  };

  var canGo = function canGo(n) {
    var nextIndex = history.index + n;
    return nextIndex >= 0 && nextIndex < history.entries.length;
  };

  var block = function block() {
    var prompt = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : false;
    return transitionManag ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.createTransitionManager"></a>[module history.createTransitionManager](#apidoc.module.history.createTransitionManager)

#### <a name="apidoc.element.history.createTransitionManager.default"></a>[function <span class="apidocSignatureSpan">history.createTransitionManager.</span>default ()](#apidoc.element.history.createTransitionManager.default)
- description and source-code
```javascript
function createTransitionManager() {
  var prompt = null;

  var setPrompt = function setPrompt(nextPrompt) {
    (0, _warning2.default)(prompt == null, 'A history supports only one prompt at a time');

    prompt = nextPrompt;

    return function () {
      if (prompt === nextPrompt) prompt = null;
    };
  };

  var confirmTransitionTo = function confirmTransitionTo(location, action, getUserConfirmation, callback) {
    // TODO: If another transition starts while we're still confirming
    // the previous one, we may end up in a weird state. Figure out the
    // best way to handle this.
    if (prompt != null) {
      var result = typeof prompt === 'function' ? prompt(location, action) : prompt;

      if (typeof result === 'string') {
        if (typeof getUserConfirmation === 'function') {
          getUserConfirmation(result, callback);
        } else {
          (0, _warning2.default)(false, 'A history needs a getUserConfirmation function in order to use a prompt message');

          callback(true);
        }
      } else {
        // Return false from a transition hook to cancel the transition.
        callback(result !== false);
      }
    } else {
      callback(true);
    }
  };

  var listeners = [];

  var appendListener = function appendListener(fn) {
    var isActive = true;

    var listener = function listener() {
      if (isActive) fn.apply(undefined, arguments);
    };

    listeners.push(listener);

    return function () {
      isActive = false;
      listeners = listeners.filter(function (item) {
        return item !== listener;
      });
    };
  };

  var notifyListeners = function notifyListeners() {
    for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
      args[_key] = arguments[_key];
    }

    listeners.forEach(function (listener) {
      return listener.apply(undefined, args);
    });
  };

  return {
    setPrompt: setPrompt,
    confirmTransitionTo: confirmTransitionTo,
    appendListener: appendListener,
    notifyListeners: notifyListeners
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.history.history"></a>[module history.history](#apidoc.module.history.history)

#### <a name="apidoc.element.history.history.createBrowserHistory"></a>[function <span class="apidocSignatureSpan">history.history.</span>createBrowserHistory ()](#apidoc.element.history.history.createBrowserHistory)
- description and source-code
```javascript
function createBrowserHistory() {
	  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

	  !_DOMUtils.canUseDOM ?  false ? (0, _invariant2.default)(false, 'Browser history needs a DOM') : (0, _invariant2.default)(false
) : void 0;

	  var globalHistory = window.history;
	  var canUseHistory = (0, _DOMUtils.supportsHistory)();
	  var needsHashChangeListener = !(0, _DOMUtils.supportsPopStateOnHashChange)();

	  var _props$forceRefresh = props.forceRefresh,
	      forceRefresh = _props$forceRefresh === undefined ? false : _props$forceRefresh,
	      _props$getUserConfirm = props.getUserConfirmation,
	      getUserConfirmation = _props$getUserConfirm === undefined ? _DOMUtils.getConfirmation : _props$getUserConfirm,
	      _props$keyLength = props.keyLength,
	      keyLength = _props$keyLength === undefined ? 6 : _props$keyLength;

	  var basename = props.basename ? (0, _PathUtils.stripTrailingSlash)((0, _PathUtils.addLeadingSlash)(props.basename)) : '';

	  var getDOMLocation = function getDOMLocation(historyState) {
	    var _ref = historyState || {},
	        key = _ref.key,
	        state = _ref.state;

	    var _window$location = window.location,
	        pathname = _window$location.pathname,
	        search = _window$location.search,
	        hash = _window$location.hash;


	    var path = pathname + search + hash;

	    if (basename) path = (0, _PathUtils.stripPrefix)(path, basename);

	    return _extends({}, (0, _PathUtils.parsePath)(path), {
	      state: state,
	      key: key
	    });
	  };

	  var createKey = function createKey() {
	    return Math.random().toString(36).substr(2, keyLength);
	  };

	  var transitionManager = (0, _createTransitionManager2.default)();

	  var setState = function setState(nextState) {
	    _extends(history, nextState);

	    history.length = globalHistory.length;

	    transitionManager.notifyListeners(history.location, history.action);
	  };

	  var handlePopState = function handlePopState(event) {
	    // Ignore extraneous popstate events in WebKit.
	    if ((0, _DOMUtils.isExtraneousPopstateEvent)(event)) return;

	    handlePop(getDOMLocation(event.state));
	  };

	  var handleHashChange = function handleHashChange() {
	    handlePop(getDOMLocation(getHistoryState()));
	  };

	  var forceNextPop = false;

	  var handlePop = function handlePop(location) {
	    if (forceNextPop) {
	      forceNextPop = false;
	      setState();
	    } else {
	      var action = 'POP';

	      transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
	        if (ok) {
	          setState({ action: action, location: location });
	        } else {
	          revertPop(location);
	        }
	      });
	    }
	  };

	  var revertPop = function revertPop(fromLocation) {
	    var toLocation = history.location;

	    // TODO: We could probably make this more reliable by
	    // keeping a list of keys we've seen in sessionStorage.
	    // Instead, we just default to 0 for keys we don't know.

	    var toIndex = allKeys.indexOf(toLocation.key);

	    if (toIndex === -1) toIndex = 0;

	    var fromIndex = allKeys.indexOf(fromLocation.key);

	    if (fromIndex === -1) fromIndex = 0;

	    var delta = toIndex - fromIndex;

	    if (delta) {
	      forceNextPop = true;
	      go(delta);
	    }
	  };

	  var initialLocation = getDOMLocation(getHistoryState());
	  var allKeys = [initialLocation.key];

	  // Public interface

	  var createHref = function createHref(location) {
	    return basename + (0, _PathUtils.createPath)(location);
	  };

	  var push = function push(path, state) {
	     false ? (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !==
undefined && state !== undefined), 'You should avoid providing a 2nd state argument to push when the 1st ' + 'argument is a location
-like object that already has state; it is ignored') : void 0;

	    var action = 'PUSH';
	    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

	    transit ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.history.createHashHistory"></a>[function <span class="apidocSignatureSpan">history.history.</span>createHashHistory ()](#apidoc.element.history.history.createHashHistory)
- description and source-code
```javascript
function createHashHistory() {
	  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};

	  !_DOMUtils.canUseDOM ?  false ? (0, _invariant2.default)(false, 'Hash history needs a DOM') : (0, _invariant2.default)(false) :
void 0;

	  var globalHistory = window.history;
	  var canGoWithoutReload = (0, _DOMUtils.supportsGoWithoutReloadUsingHash)();

	  var _props$getUserConfirm = props.getUserConfirmation,
	      getUserConfirmation = _props$getUserConfirm === undefined ? _DOMUtils.getConfirmation : _props$getUserConfirm,
	      _props$hashType = props.hashType,
	      hashType = _props$hashType === undefined ? 'slash' : _props$hashType;

	  var basename = props.basename ? (0, _PathUtils.stripTrailingSlash)((0, _PathUtils.addLeadingSlash)(props.basename)) : '';

	  var _HashPathCoders$hashT = HashPathCoders[hashType],
	      encodePath = _HashPathCoders$hashT.encodePath,
	      decodePath = _HashPathCoders$hashT.decodePath;


	  var getDOMLocation = function getDOMLocation() {
	    var path = decodePath(getHashPath());

	    if (basename) path = (0, _PathUtils.stripPrefix)(path, basename);

	    return (0, _PathUtils.parsePath)(path);
	  };

	  var transitionManager = (0, _createTransitionManager2.default)();

	  var setState = function setState(nextState) {
	    _extends(history, nextState);

	    history.length = globalHistory.length;

	    transitionManager.notifyListeners(history.location, history.action);
	  };

	  var forceNextPop = false;
	  var ignorePath = null;

	  var handleHashChange = function handleHashChange() {
	    var path = getHashPath();
	    var encodedPath = encodePath(path);

	    if (path !== encodedPath) {
	      // Ensure we always have a properly-encoded hash.
	      replaceHashPath(encodedPath);
	    } else {
	      var location = getDOMLocation();
	      var prevLocation = history.location;

	      if (!forceNextPop && (0, _LocationUtils.locationsAreEqual)(prevLocation, location)) return; // A hashchange doesn't always
 == location change.

	      if (ignorePath === (0, _PathUtils.createPath)(location)) return; // Ignore this change; we already setState in push/replace
.

	      ignorePath = null;

	      handlePop(location);
	    }
	  };

	  var handlePop = function handlePop(location) {
	    if (forceNextPop) {
	      forceNextPop = false;
	      setState();
	    } else {
	      var action = 'POP';

	      transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
	        if (ok) {
	          setState({ action: action, location: location });
	        } else {
	          revertPop(location);
	        }
	      });
	    }
	  };

	  var revertPop = function revertPop(fromLocation) {
	    var toLocation = history.location;

	    // TODO: We could probably make this more reliable by
	    // keeping a list of paths we've seen in sessionStorage.
	    // Instead, we just default to 0 for paths we don't know.

	    var toIndex = allPaths.lastIndexOf((0, _PathUtils.createPath)(toLocation));

	    if (toIndex === -1) toIndex = 0;

	    var fromIndex = allPaths.lastIndexOf((0, _PathUtils.createPath)(fromLocation));

	    if (fromIndex === -1) fromIndex = 0;

	    var delta = toIndex - fromIndex;

	    if (delta) {
	      forceNextPop = true;
	      go(delta);
	    }
	  };

	  // Ensure the hash is encoded properly before doing anything else.
	  var path = getHashPath();
	  var encodedPath = encodePath(path);

	  if (path !== encodedPath) replaceHashPath(encodedPath);

	  var initialLocation = getDOMLocation();
	  var allPaths = [(0, _PathUtils.createPath)(initialLocation)];

	  // Public interface

	  var createHref = function createHref(location) {
	    return '#' + encodePath(basename + (0, _PathUtils.createPath)(location));
	  };

	  var push = function push(path, state) {
	     false ? (0, _warning2.default)(state === undefined, 'Hash history cannot push state; it is ignored') : void 0;

	    var action = 'PUSH';
	    var location = (0, _LocationUtils.createLocation)(path, undefined, undefined, history.location);

	    transitionManager.c ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.history.createLocation"></a>[function <span class="apidocSignatureSpan">history.history.</span>createLocation (path, state, key, currentLocation)](#apidoc.element.history.history.createLocation)
- description and source-code
```javascript
function createLocation(path, state, key, currentLocation) {
	  var location = void 0;
	  if (typeof path === 'string') {
	    // Two-arg form: push(path, state)
	    location = (0, _PathUtils.parsePath)(path);
	    location.state = state;
	  } else {
	    // One-arg form: push(location)
	    location = _extends({}, path);

	    if (location.pathname === undefined) location.pathname = '';

	    if (location.search) {
	      if (location.search.charAt(0) !== '?') location.search = '?' + location.search;
	    } else {
	      location.search = '';
	    }

	    if (location.hash) {
	      if (location.hash.charAt(0) !== '#') location.hash = '#' + location.hash;
	    } else {
	      location.hash = '';
	    }

	    if (state !== undefined && location.state === undefined) location.state = state;
	  }

	  location.key = key;

	  if (currentLocation) {
	    // Resolve incomplete/relative pathname relative to current location.
	    if (!location.pathname) {
	      location.pathname = currentLocation.pathname;
	    } else if (location.pathname.charAt(0) !== '/') {
	      location.pathname = (0, _resolvePathname2.default)(location.pathname, currentLocation.pathname);
	    }
	  }

	  return location;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.history.createMemoryHistory"></a>[function <span class="apidocSignatureSpan">history.history.</span>createMemoryHistory ()](#apidoc.element.history.history.createMemoryHistory)
- description and source-code
```javascript
function createMemoryHistory() {
	  var props = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};
	  var getUserConfirmation = props.getUserConfirmation,
	      _props$initialEntries = props.initialEntries,
	      initialEntries = _props$initialEntries === undefined ? ['/'] : _props$initialEntries,
	      _props$initialIndex = props.initialIndex,
	      initialIndex = _props$initialIndex === undefined ? 0 : _props$initialIndex,
	      _props$keyLength = props.keyLength,
	      keyLength = _props$keyLength === undefined ? 6 : _props$keyLength;


	  var transitionManager = (0, _createTransitionManager2.default)();

	  var setState = function setState(nextState) {
	    _extends(history, nextState);

	    history.length = history.entries.length;

	    transitionManager.notifyListeners(history.location, history.action);
	  };

	  var createKey = function createKey() {
	    return Math.random().toString(36).substr(2, keyLength);
	  };

	  var index = clamp(initialIndex, 0, initialEntries.length - 1);
	  var entries = initialEntries.map(function (entry) {
	    return typeof entry === 'string' ? (0, _LocationUtils.createLocation)(entry, undefined, createKey()) : (0, _LocationUtils.createLocation
)(entry, undefined, entry.key || createKey());
	  });

	  // Public interface

	  var createHref = _PathUtils.createPath;

	  var push = function push(path, state) {
	     false ? (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !==
undefined && state !== undefined), 'You should avoid providing a 2nd state argument to push when the 1st ' + 'argument is a location
-like object that already has state; it is ignored') : void 0;

	    var action = 'PUSH';
	    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

	    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
	      if (!ok) return;

	      var prevIndex = history.index;
	      var nextIndex = prevIndex + 1;

	      var nextEntries = history.entries.slice(0);
	      if (nextEntries.length > nextIndex) {
	        nextEntries.splice(nextIndex, nextEntries.length - nextIndex, location);
	      } else {
	        nextEntries.push(location);
	      }

	      setState({
	        action: action,
	        location: location,
	        index: nextIndex,
	        entries: nextEntries
	      });
	    });
	  };

	  var replace = function replace(path, state) {
	     false ? (0, _warning2.default)(!((typeof path === 'undefined' ? 'undefined' : _typeof(path)) === 'object' && path.state !==
undefined && state !== undefined), 'You should avoid providing a 2nd state argument to replace when the 1st ' + 'argument is a location
-like object that already has state; it is ignored') : void 0;

	    var action = 'REPLACE';
	    var location = (0, _LocationUtils.createLocation)(path, state, createKey(), history.location);

	    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
	      if (!ok) return;

	      history.entries[history.index] = location;

	      setState({ action: action, location: location });
	    });
	  };

	  var go = function go(n) {
	    var nextIndex = clamp(history.index + n, 0, history.entries.length - 1);

	    var action = 'POP';
	    var location = history.entries[nextIndex];

	    transitionManager.confirmTransitionTo(location, action, getUserConfirmation, function (ok) {
	      if (ok) {
	        setState({
	          action: action,
	          location: location,
	          index: nextIndex
	        });
	      } else {
	        // Mimic the behavior of DOM histories by
	        // causing a render after a cancelled POP.
	        setState();
	      }
	    });
	  };

	  var goBack = function goBack() {
	    return go(-1);
	  };

	  var goForward = function goForward() {
	    return go(1);
	  };

	  var canGo = function canGo(n) {
	    var nextIndex = history.index + n;
	    return nextIndex >= 0 && nextIndex < history.entries.length;
	  };

	  var block = function block() ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.history.createPath"></a>[function <span class="apidocSignatureSpan">history.history.</span>createPath (location)](#apidoc.element.history.history.createPath)
- description and source-code
```javascript
function createPath(location) {
	  var pathname = location.pathname,
	      search = location.search,
	      hash = location.hash;


	  var path = encodeURI(pathname || '/');

	  if (search && search !== '?') path += search.charAt(0) === '?' ? search : '?' + search;

	  if (hash && hash !== '#') path += hash.charAt(0) === '#' ? hash : '#' + hash;

	  return path;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.history.locationsAreEqual"></a>[function <span class="apidocSignatureSpan">history.history.</span>locationsAreEqual (a, b)](#apidoc.element.history.history.locationsAreEqual)
- description and source-code
```javascript
function locationsAreEqual(a, b) {
	  return a.pathname === b.pathname && a.search === b.search && a.hash === b.hash && a.key === b.key && (0, _valueEqual2.default
)(a.state, b.state);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.history.history.parsePath"></a>[function <span class="apidocSignatureSpan">history.history.</span>parsePath (path)](#apidoc.element.history.history.parsePath)
- description and source-code
```javascript
function parsePath(path) {
	  var pathname = path || '/';
	  var search = '';
	  var hash = '';

	  var hashIndex = pathname.indexOf('#');
	  if (hashIndex !== -1) {
	    hash = pathname.substr(hashIndex);
	    pathname = pathname.substr(0, hashIndex);
	  }

	  var searchIndex = pathname.indexOf('?');
	  if (searchIndex !== -1) {
	    search = pathname.substr(searchIndex);
	    pathname = pathname.substr(0, searchIndex);
	  }

	  pathname = decodeURI(pathname);

	  return {
	    pathname: pathname,
	    search: search === '?' ? '' : search,
	    hash: hash === '#' ? '' : hash
	  };
	}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)

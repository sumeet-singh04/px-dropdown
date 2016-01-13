# Px-dropdown

Px-dropdown is a select component.

## Overview

px-dropdown is an element which can be placed in any elements, and opens a customizable dropdown list.

## Usage

### Prerequisites
1. node.js
2. npm
3. bower
4. [webcomponents-lite.js polyfill](https://github.com/webcomponents/webcomponentsjs)

Node, npm and bower are necessary to install the component and dependencies. webcomponents.js adds support for web components and custom elements to your application.

### Getting Started

First, install the component via bower on the command line.

```
bower install https://github.com/PredixDev/px-dropdown.git --save
```

Second, import the component to your application with the following tag in your head.

```
<link rel="import" href="/bower_components/px-dropdown/px-dropdown.html"/>
```

Finally, use the component in your application:

```
<px-dropdown>
  <px-dropdown-content class="px-dropdown-content" max-cont-character-width="10" width="100" items='[{"key":"one", "val": "One"}, {"key":"two", "val": "Two"}, {"key":"three", "val": "Three"}, {"key":"four", "val": "How now brown cow"}]'>
  </px-dropdown-content>
  <px-dropdown-chevron class="px-dropdown-trigger"></px-dropdown-chevron>
</px-dropdown>
```

<br />
<hr />

## Attributes

#### max-cont-character-width

*Type:* **Number** - (*Optional*) - *Default:* "0"

a number which represents the longest string allowed in the dropdown before the string is clipped, and has an ellipsis added to the end of it. Clipping a string means a px-tooltip component appear on hover with the full - unclipped - string in it.


```
<px-dropdown-content  
  max-cont-character-width="10"
  .... >
....
</px-dropdown-content>

```
#### width

*Type:* **Number** - (*Required*) - *Default:* ""

An attribute which determines the size of the container px-dropdown sits in. This item is a number only, (no 'px'), and represents pixels.

```
<px-dropdown-content  
  width="100"
  .... >
....
</px-dropdown-content>
```

#### items

*Type:* **Object** - (*required*) - *Default:* ""

an object Literal which holds the list of items that should appear in the dropdown.

```
<px-dropdown-content
...
 items='[{"key":"one", "val": "One"}, {"key":"two", "val": "Two"}, {"key":"three", "val": "Three"}, {"key":"four", "val": "How now brown cow"}]'>
</px-dropdown-content>
```

<br />
<hr />


## Local Development

From the component's directory...

```
$ npm install
$ bower install
$ grunt sass
```

From the component's directory, to start a local server run:

```
$ grunt depserve
```

Navigate to the root of that server (e.g. http://localhost:8080/) in a browser to open the API documentation page, with link to the "Demo" / working examples.

### LiveReload

By default grunt watch is configured to enable LiveReload and will be watching for modifications in your root directory as well as `/css`.

Your browser will also need to have the LiveReload extension installed and enabled. For instructions on how to do this please refer to: [livereload.com/extensions/](http://livereload.com/extensions/).

Disable LiveReload by removing the `livereload` key from the configuration object or explicitly setting it to false.


### DevMode
Devmode runs `grunt depserve` and `grunt watch` concurrently so that when you make a change to your source files and save them, your preview will be updated in any browsers you have opened and turned on LiveReload.
From the component's directory run:

```
$ grunt devmode
```

### GE Coding Style Guide
[GE JS Developer's Guide](https://github.com/GeneralElectric/javascript)

<br />
<hr />

## Known Issues

Please use [Github Issues](https://github.com/PredixDev/px-dropdown/issues) to submit any bugs you might find.

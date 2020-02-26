# mark.js

mark.js is a JavaScript library to save and restore document position.

## Installation

Add [`mark.js`](scripts/mark.js) to your project.

## Methods

See the [source](scripts/mark.js) for a complete reference.

###### `constructor()`

Initialize object.

###### `push()`

Push mark.

###### `pop()`

Pop mark.

###### `jump()`

Jump to mark.

###### `clear()`

Clear all marks.

## Events

###### `push(x, y, index)`

A mark has been saved.

###### `pop(x, y, index)`

A mark has been removed.

###### `jump(x, y, index)`

A mark has been restored.

###### `clear()`

All marks have been removed.

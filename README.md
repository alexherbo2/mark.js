# Mark

> Save and restore document position.

## Usage

``` javascript
const mark = new Mark
mark.on('push', (x, y, index) => console.log('Push', x, y, index))
mark.on('pop', (x, y, index) => console.log('Pop', x, y, index))
mark.on('jump', (x, y, index) => console.log('Jump', x, y, index))
mark.on('clear', () => console.log('Clear'))

mark.push()
document.scrollingElement.scrollBy({ top: 70 })
mark.jump()
mark.pop()
mark.clear()
```

More examples at [Krabby].

## Methods

- `push()`: Push mark.
- `pop()`: Pop mark.
- `jump()`: Jump to mark.
- `clear()`: Clear marks.

## Events

- `push(x, y, index)`: A mark has been saved.
- `pop(x, y, index)`: A mark has been removed.
- `jump(x, y, index)`: A mark has been restored.
- `clear()`: All marks have been removed.

## References

- [Create a keyboard interface to the web]

[Krabby]: https://krabby.netlify.com
[Create a keyboard interface to the web]: https://alexherbo2.github.io/blog/chrome/create-a-keyboard-interface-to-the-web/

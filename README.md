# Mark

> Save and restore document position.

## Usage

``` javascript
const mark = new Mark
mark.on('push', (x, y, index) => console.log('Push', x, y, index))
mark.on('jump', (x, y, index) => console.log('Jump', x, y, index))

mark.push()
document.scrollingElement.scrollBy({ top: 70 })
mark.jump()
```

More examples at [Krabby].

## Methods

- `push()`: Push mark.
- `jump()`: Jump to mark.

## Events

- `push(x, y, index)`: A mark has been saved.
- `jump(x, y, index)`: A mark has been restored.

## References

- [Create a keyboard interface to the web]

[Krabby]: https://krabby.netlify.com
[Create a keyboard interface to the web]: https://alexherbo2.github.io/blog/chrome/create-a-keyboard-interface-to-the-web/

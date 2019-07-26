# html-runner

This does one thing and one thing only. It converts the following HTML to JavaScript and executes it.

```html
<ul id="foo">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>

<output for="foo" name="bar">${bar}</output>
```

becomes

```javascript
const foo = ['Item 1', 'Item 2', 'Item 3'];
foo.forEach(bar => console.log(`${bar}`));
```

and is then executed.


Sorry, not sorry.

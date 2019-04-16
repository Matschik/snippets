# JavaScript

## `<button>` child events
- `<button>` child elements events are totally ignored: it only triggers `<button>` event.
- Triggering child event will not trigger parent `<button>` event.

Example:
```html
<button>Ouvrir mes notifications <div class="badge">4</div></button>
```

```css
button {
  position: relative;
}
.badge {
  position: absolute;
  top: -9px;
  left: 152px;
  background: red;
  color: white;
  padding: 2px;
}
```

```js
document.querySelector("button").onclick = () => {
  alert("Button clicked");
};

document.querySelector(".badge").onclick = function(event) {
  alert('Badge cliked');
};
```

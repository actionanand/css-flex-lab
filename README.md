# CSS - flex lab

Dev server: Point your browser at the below address!

```
http://127.0.0.1:5173/
```

## Flex Container default values

```css
  .flex-container {
    background: white;
    padding: 10px;
    border: 5px solid black;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    align-items: stretch;
    justify-content: flex-start;
    /* align-content: space-around; */
    align-content: normal;
    height: 900px;
    /* short-hand for flex */
    flex-flow: row nowrap;
  }
```

## Flex Items default values

```css
  .item-6 {
    background: #d3c0b1;
    color: white;
    padding: 10px;
    border: 5px solid black;
    margin: 10px;
    width: 210px;
    order: 0;
    /* 'order below 0' will be placed at the beging & `order above 1` will be placed at the end */
    flex-grow: 0;
    flex-shrink: 1;
    /* If `flex-shrink: 1;` item won't shrink */
    /* flex-basis: auto | content | <width> | <height>; */
    flex-basis: auto;
    /* flex: flex-grow flex-shrink flex-basis; */
    flex: 0 1 auto;
  }
```

* `flex-basis` is based on the **main axis**. If `flex-direction: row;`, `flex-basis` will be replaced the **width** of the element (X - axis). If `flex-direction: column;`, `flex-basis` will be replace the **height** of the element (Y - axis).

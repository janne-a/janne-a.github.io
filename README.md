# Coding examples


## CSS - GRID

### CSS - Grid - Auto-fit: Dynamically place items to columns, based on screen size
Item takes min. 100px and max 1fr.

**Narrow viewport**: Puts items on another row(s)

**Wide viewport**: If fit on one row, they expand as much as they can


```css
grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
```
Narrow viewport:

<img src="images/css-grid-autofit-2.png" width="30%">

Wide viewport:

<img src="images/css-grid-autofit-1.png" width="100%">

### CSS - Grid - Auto-fill: Dynamically place items and blank items to columns, based on screen size.
Item takes min. 100px and max 1fr (max. size is not achieved).
When screen size grows, space is reserved for blank 100px items. 

```css
grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
```

![Image of css-grid-autofill](images/css-grid-autofill-2.png)

| Left | Center | Right |
| :--- | :----: | ----: |
| 1    |   2    |     3 |
| 30   |   40   |    50 |
 

# Coding examples


## CSS - GRID

### CSS - Grid - Auto-fit: Dynamically place items to columns, based on screen size
Item takes min. 100px and max 1fr.

**Narrow screen**: Puts items on another row(s)

**Wide screen**: If fit on one row, they expand as much as they can


```css
grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
```
Narrow screen:

<img src="images/css-grid-autofit-2.png" width="30%">

Wide screen:

<img src="images/css-grid-autofit-1.png" width="100%">

### CSS - Grid - Auto-fill: Dynamically place items and blank items to columns, based on screen size.
Item takes min. 100px and max 1fr (max. size is not achieved).

**Narrow screen**: Puts items on another row(s)

**Wide screen**: If items fit on one row, they expand only to 100px. New empty 100px items are added to the end.

 

```css
grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
```
Narrow viewport:

<img src="images/css-grid-autofit-2.png" width="30%">

Wide viewport (DevTools only shows lines of empty items, normal mode they are not visible): 

![Image of css-grid-autofill](images/css-grid-autofill-2.png)

| Left | Center | Right |
| :--- | :----: | ----: |
| 1    |   2    |     3 |
| 30   |   40   |    50 |
 

# Notes on Positioning

## CSS POSITION

  1. use the position property
  2. choose between static, relative, absoluter, fixed or sticky
  3. choose the x, y value positioned from the top left corner (positive values are right and down)
  4. chose z-index

    - __static__	Default value. Elements render in order, as they appear in the document flow	Play it »
    - __absolute__	The element is positioned relative to its first positioned (not static) ancestor element	Play it »
    - __fixed__	The element is positioned relative to the browser window	Play it »
    - __relative__	The element is positioned relative to its normal position, so "left:20px" adds 20 pixels to the element's LEFT position

    ```
    h2.pos_left {
        position: relative;
        left: -20px;
    }
    ```
    
    - __sticky__	The element is positioned based on the user's scroll position.  A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed). Note: Not supported in IE/Edge 15 or earlier. Supported in Safari from version 6.1 with a -webkit- prefix.

   
   ```
    div.sticky {
      position: -webkit-sticky;
      position: sticky;
      top: 0;
      padding: 5px;
      background-color: #cae8ca;
      border: 2px solid #4CAF50;
    }
    ```

## CSS TRANSFORM
The translate() CSS function repositions an element in the horizontal and/or vertical directions. Its result is a <transform-function> data type.
  1. choose transform
  2. choose 

```
div {
    -ms-transform: translate(50px, 100px); /* IE 9 */
    -webkit-transform: translate(50px, 100px); /* Safari */
    transform: translate(50px, 100px);
}
```

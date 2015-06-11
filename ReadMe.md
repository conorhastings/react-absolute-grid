React Absolute Grid
===================
An absolute layout grid with animations, filtering, and drag and drop support. Use your own component as the grid item.

Usage:
===

    import React from 'react';
    import AbsoluteGrid from './lib/AbsoluteGrid.jsx';
    
    /*
       The data structure is pretty strict, we require a unique identifier (in this case key) and a sort
    */
    var sampleItems = [
      {key: 1, name: 'Test', sort: 0, filtered: 0},
      {key: 2, name: 'Test 1', sort: 1, filtered: 0},
    ];
     
    React.render(<AbsoluteGrid items={sampleItems} />, document.getElementById('Container'));
    

Options (Properties)
=====

  * items, default: [] | The array of items in the grid
  * displayObject, default: <GridItem/> | The React compnent used to display items
  * keyProp, default: 'key' | The property to be used as a key 
  * filterProp, default: 'filtered' | The property to be used for filtering, true means it's filtered
  * sortProp, default: 'sort' | The property to sort on
  * itemWidth, default: 128 | The width of an item
  * itemHeight, default: 128 | The height of an item
  * verticalMargin, default: -1 | How much space between rows, -1 means the same as coumns spacing which is dynamically calculated
  * responsive, default: false,
  * zoom, default: 1

ToDo:
===

 * Drag and Drop
 * Selection
 * Filter Demo
 * Docs
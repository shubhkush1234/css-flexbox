Flexbox - Udemy course - Codevolution 

// https://github.com/gopinav/Flexbox-Tutorial 


What is flexbox?

CSS Flexible Box Module --> One- dimesional layout model 
Features:
1. Flexible and efficient layouts
2. Distribute space among items
3. Control their alignment in a given container.

Before Flexbox, there were 4 layout modes:

1. Block - For section in a webpage
2. Inline - For texts
3. Table - For 2 dimesional table data
4. Positioned - For explicit position of an element

Why Flexbox?
1. A lot of flexibility.
2. Arrange items
3. Spacing
4. alignment
5. Order of items
6. Bootstrap 4 is built on top of Flex layout


Terminology: 
Mainly 2 entities in a Flexbox
1. Flex container
2. Flex items
<div class="container">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>

1. Flexbox Axes:
    1. Main Axis
    2. Cross Axis

Main Axis runs left to righ
    -   The starting point of the Main axis ==> Main start
    -   The end point of the Main axis ==> Main end
    -   The length from Main start to Main end ==> Main size
    -   The flex items flows from Main start till Main end and take up main size as length.

Cross Axis runs perpendicular to the main axis and runs top to bottom.
    -   Similarly for the Cross Axis, we start from ==> Cross start
    -   End point ==> Cross end, takes the Cross size 

Flex COntainer Properties
    1. display
    2. flex-direction
    3. flex-wrap
    4. fLex-flow (flex direction , flex wrap)
    5. Justify-content
    6. align-items
    7. align-content

1. Display property
```javaScript
<body>
      <div class='container'>
        <div class="flex-item item-1">Item 1 </div>
        <div class="flex-item item-2">Item 2 </div>
        <div class="flex-item item-3">Item 3 </div>
        <div class="flex-item item-4">Item 4 </div>
        <div class="flex-item item-5">Item 5 </div>
        <div class="flex-item item-6">Item 6 </div>
        <div class="flex-item item-7">Item 7 </div>
        <div class="flex-item item-8">Item 8 </div>
        <div class="flex-item item-9">Item 9 </div>
      </div>
    <style>
      body {
      margin: 0;
      }
      .container {
      border: 6px solid black;
      display: inline-flex;
      flex-wrap: wrap;
      }
      .flex-item {
      color: white;
      font-size: 1.5rem;
      padding: 1 rem;
      text-align: center;
      }
      .item-1 {
      background-color: yellowgreen;
      }
      .item-2 {
      background-color: red;
      }
      .item-3 {
      background-color: green;
      }
      .item-4 {
      background-color: pink;
      }
      .item-5 {
      background-color: orange;
      }
      .item-6 {
      background-color: peachpuff;
      }
      .item-7 {
      background-color: black;
      }
      .item-8 {
      background-color: brown;
      }
      .item-9 {
      background-color: magenta;
      }
    </style>
    <script src="app.js"></script>
</body>



```

NOTE: Make sure that the display property is set (to flex or inline-flex), otherwise none of the flex properties will work. 

1. Display Property:
It create either a block level or inline level flex container.
Possible options are: 
    1. flex
    2. inline-flex
2. Flex Direction
flex-direction sets the direction of the main axis thereby controlling how the items are placed in a container.

By default, it is set from left to right.
Possible options are: 
    1. row
    2. row-reverse
    3. column
    4. column-reverse
row: sets the main axis to left to right 

3. flex-wrap

"Controls the wrapping of flex items within the container."

Possible values are: 
    1. nowrap
    2. wrap
    3. wrap-reverse
By default, all the flex items in a container will try to fit into a single line. If there is not enough space, the items will overflow. 

If we reduce the browser width, the items begin to shrink and then if reduced further, they are no longer in view.

We can change this behaviour using the flex-wrap property.

Default value of flex-wrap is nowrap.


```javaScript
.container{
    border: 6px solid black;
    display: flex;
    flex-wrap: wrap;
}
```

 

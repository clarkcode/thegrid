# TheGrid #

TheGrid is a lightweight barebones 12-column responsive grid. I required a grid without the overhead of a complete CSS framework. I have added a few additional components but they all focus on layout..

## Usage ##
### Layout ###
Container or Container-Full >> Row >> Columns

### 1. Create Container ###
`.container`
Container is centered has a max width of 80% of the screen on large displays and 95% for tablet displays. This is set to 100% for mobile displays.
`<div class="container"></div>`

`.container-full`  
container-full is 100% full width across all devices.
`<div class="container-full"></div>`

### 2. Create Row within a Container or Container-Full ###
`.row`
Containers are split into mulitple horizontal rows.

```
<div class="container">
    <div class="row">
    </div>
</div>
```

or depending on your design:

```
<div class="container-full">
    <div class="row">
    </div>
</div>
```

### 3. Create Columns within the Rows ###
`.col`
A column can be given size attributes for each type of display.
The following example will strech 12 columns wide on all small(s), medium(m) and large(l) displays. The grid is 12 columns wide.

```
<div class="container">
    <div class="row">
        <div class="col s12 m12 l12"></div>
    </div>
</div>
```

`.s(1 to 12)`
S (Small) followed by any number from 1 through 12, 12 being the max, specifies how wide the column should be on mobile displays.

`.m(1 to 12)`
M (Medium) followed by any number from 1 through 12, 12 being the max, specifies how wide the column should be on tablet displays.

`.l(1 to 12)`
L (Large) followed by any number from 1 through 12, 12 being the max, specifies how wide the column should be on desktop displays.


`.s(1 to 12)-offset`
S (Small) followed by any number from 1 through 12, 12 being the max, and offset specifies how wide the column should be offset on mobile displays.

`.m(1 to 12)-offset`
M (Medium) followed by any number from 1 through 12, 12 being the max, and offset specifies how wide the column should be offset on tablet displays.

`.l(1 to 12)-offset`
L (Large) followed by any number from 1 through 12, 12 being the max, and offset specifies how wide the column should be offset on desktop displays.


### Components ###

`.responsive-img`
Makes images responsive to their parent div.

`.mobile-hidden`
Hides element on mobile devices.

`.mobile-show`
Shows element on mobile devices.

`.tablet-hidden`
Hides element on tablet devices.

`.tablet-show`
Shows element on tablet devices.

`.desktop-hidden`
Hides element on desktop devices.

`.desktop-show`
Shows element on desktop devices.

`.center`
Centers content.

`.s-center // .m-center // .l-center`
Center content only on .s (small) // .m (medium) // .l (large) displays

`.left`
Left align content.

`.s-left // .m-left // .l-left`
Left align only on .s (small) // .m (medium) // .l (large) displays

`.right`
Right align content.

`.s-right // .m-right // .l-right`
Right align only on .s (small) // .m (medium) // .l (large) displays

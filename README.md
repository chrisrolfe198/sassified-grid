#sassified-grid
 
A grid designed to be used as a Sass module or as a standalone component 

##Installation
###CSS
If you are just after the css you can view it [here](https://raw2.github.com/christopherrolfe198/sassified-grid/master/stylesheets/grid.css).

If you copy and paste that into a css file locally you can then reference it in your html and start using the grid.

###Scss
If you want to use this in your scss you need to download the repository and move this into the appropriate location.

Once that's done you can reference it by just importing the grid file like so:

```
@import "sassified-grid/sass/grid";
```

##How to

This grid has been written with mobile first in mind, so ideally you would set the mobile grid position and then simply iterate upon it going up through the breakpoints. E.G.

```
<div class="col-m-12 col-t-4">
  On Desktop and large desktops the width will still be 4 columns so I don't need to add the additional classes
</div>
```

The 4 types of classes are: 

* `col-m-*`
* `col-t-*`
* `col-d-*`
* `col-ld-*`

By default sassified grid comes with 12 columns and you can use them like so:

```
<div class="row">
  <div class="col-m-12">
    <p>I am a block that fills 12 columns</p>
    <div class="row">
      <div class="col-m-6">
        <p>I am a nested block</p>
      </div>
    </div>
  </div>
</div>
```

For a clear example you can clone the repository and look at example.html in your browser

### Offsets
This grid now includes offsets.

You can apply them like the following:

```
<div class="row">
  <div class="col-m-3">
    <p>I am a block that fills 3 columns</p>
  </div>
  <div class="col-m-offset-3 col-m-6">
  	I am a block with a 3 columns gap to the block to the left
  </div>
</div>
```

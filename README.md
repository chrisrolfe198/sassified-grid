#sassified-grid

A grid designed to be used as a Sass module or as a standalone component 

##Installation
###CSS
If you are just after the css you can view it [here](https://raw2.github.com/christopherrolfe198/sassified-grid/master/stylesheets/grid.css).

If you copy and paste that into a css file locally you can then reference it in your html and start using the grid.

###Scss
If you want to use this in your scss you need to download the sass directory and move this into the appropriate location.

Once that's done you can reference it by just importing the grid file.

E.G. if I had the sass folder inside a sassified-grid folder I would reference it like this:

```
@import "sassified-grid/grid";
```

##How to
By default sassified grid comes with 12 columns and you can use them like so:

```
<div class="row">
  <div class="col-12">
    <p>I am a block that fills 12 columns</p>
    <div class="row">
      <div class="col-6">
        <p>I am a nested block</p>
      </div>
    </div>
  </div>
</div>
```

### Offsets
This grid now includes offsets.

You can apply them like the following:

```
<div class="row">
  <div class="col-3">
    <p>I am a block that fills 3 columns</p>
  </div>
  <div class="col-offset-3 col-6">
  	I am a block with a 3 columns gap to the block to the left
  </div>
</div>
```
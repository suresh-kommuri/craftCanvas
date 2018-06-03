> "A Library For Canvas"

## Installation

```sh
$ npm install --save craftcanvas
```

## Usage

Just Include your canvas tag in your html page by adding id to it.

```html
<canvas id="canvas1" width="600" height="300"></canvas>
```

And include minified `craftCanvas.min.js` Javascript file

```html
<script type="text/javascript" src="craftCanvas.min.js"></script>
```

<h2>CraftCanvas</h2>

> No script to Draw just pass keys and Draw canvas as you like

Pass your own key values in an object by calling function to draw canvas in your hmtl

<h2>Hints</h2>

* You have to call a function by passing your key values with an object.
* `multiple` key will give you to draw multiple shapes for parent shape.
* You can pass only single image.

> Circle, Square and Line only available features are in progress.

```Javascript
callCanvas("#canvas1").create({
  width: '100%',
  height: 500,
  circle: {
    radius: 70,
    context: "2d",
    moon: "full",
    stroke: 1,
    left: 150,
    top: 120,
    lineColor: "red",
    image: '/images/img.png',
    multiple: {
      two: {
        radius: 70,
        lineColor: "yellow",
        top: 100,
        stroke: 5,
        left: 100,
      }
    }
  },
  square: {
    height: 100,
    context: '2d',
    width: 180,
    left: 50,
    top: 1,
    stroke: 1,
    lineColor: 'orange',
    multiple: {
      two: {
        lineColor: 'blue',
        width: 50,
        height: 50,
        left: 200,
        stroke: 10,
        top: 10
      },
      three: {
        lineColor: 'green',
        context: '2d',
        left: 100,
        width: 100,
        height: 40,
        top: 20,
        stroke: 1
      }
    }
  },
  line: {
    moveToX: 10,
    context: '2d',
    moveToY: 20,
    lineToX: 200,
    lineToY: 100,
    stroke: 5,
    lineColor: 'red',
    lineCap: 'butt'
  }
});
```

## github

[https://github.com/suresh-kommuri/craftCanvas.git](https://github.com/suresh-kommuri/craftCanvas.git)

## License

MIT © [Suresh Kommuri](https://github.com/suresh-kommuri)

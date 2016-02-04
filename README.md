# Bootstrap Scavenger Hunt

In this scavenger hunt you'll create a webpage that uses many of the cool features
of Bootstrap. For each feature, you'll get a description and a picture of what it's
supposed to look like. Then, you'll go to the bootstrap documentation
and learn how to code the feature. Collect all of the features and earn a prize!

## Documentation

You can find everything you need to know about Bootstrap in its online documentation,

> http://v4-alpha.getbootstrap.com/

- There's a **search bar on the right side** that you can use to find what you need.
- Whenever you're stumped about something, **go to the documentation**
- If the documentation doesn't make sense, **ask questions!**

## Check your work

You can see a finished version of the Bootstrap Scavenger Hunt at

> https://bootstrap-scavenger-hunt-bbarg.c9users.io/first-bootstrap-page.html

## Getting started

You start out with a basic page outline, in the file `scavenger-hunt.html`.

```html
<head>
    <link rel="stylesheet" href="bootstrap cdn url goes here!">
    <style>
        /* Any extra CSS goes here! */    
    </style>
</head>
<body>
    <!-- Content goes here! -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.2/js/bootstrap.min.js"></script>
</body>
```

The `<link>` tag is for including the Boostrap css library. The two `<script>` tags are for
the Bootstrap javascript library (which is needed for some animations) and jQuery
(another library that the Bootstrap javascript library uses).

### Do now

- Go to the `View` menu in Cloud9 and select `Wrap Lines`. This makes it so long
  lines of code "wrap" around to the next line (so you can still read them).
- Go to `first_bootstrap_page.html` and select all of the code in the file. Then,
  go to the `Edit` menu in Cloud9 and select `Code Formatting->HTML`. This will
  format your HTML nicely so it's easier to read.

## Features

### The grid

One of bootstrap's best features is that it lets us position things a lot more
easily on the page. Bootstrap breaks up the page into a grid of 12 columns. You
as the programmer make rows, and for each row you make columns. The width of all the columns
adds up to 12.

#### Your job

- Use the grid system to create three adjacent columns.
- Each column should contain an `<h1>`, an `<img>`, and a `<p>` tag.

### Jumbotron

You'll want your site to have a big header area so people know what it is about. 
Bootstrap gives us a class called `jumbotron` that helps with this.

#### Your job

- Create a `jumbotron` header
- In the header, put an `<h1>` tag with a title, and `<p>` tag with a subtitle.
- **Challenge**: You can put a background image in your `jumbotron`. Use the css
  properties `background-image` and `background-size` to add an image and make
  it size up correctly.
    - *Hint*: You might need to change the color of the text in your `jumbotron`
      so you can read it on top of the image.

### Image styling

If you haven't already done so, pick out some images. Your images are probably
too big for each column and they're messing out your column layout. You can
use Bootstrap's `.img-responsive` class to make the image resize to fit the space
it's in.

#### Your job
- Use Bootstrap's `.img-responsive` class to make your images fit into their columns.
- Look at the bootstrap documentation to see how you can change the shape of your
  image (then make all of your `<img>` tags have the same shape).

### Buttons

You want to reward your viewer for reading all of the content on your site. When
your viewer finished reading a column, they can click a button to see a reward
message. First you'll add the button.

#### Your job

- Add a button in each of your columns below the `<p>` tag.
- Make the button say something like "Complete this column!"
- Choose a style for each button

### Collapsable elements

Now you can add some content below each button that will be "toggled" (turned off and on)
by clicking the button. Then, you'll use the Bootstrap `.collapse` class to
make the toggling happen.

Check out http://v4-alpha.getbootstrap.com/components/collapse/#example for an example
of what it means to "toggle" some content.

#### Your job

- Add a reward message inside a `<p>` tag underneath each button.
- Put that `<p>` tag *inside* a `<div>` tag (you'll need this so the button
  can reference the `<div>`
- Use the documentation to figure out how to get the button to reference the
  reward message

### Navigation bar

You have a lot of information to share on your website, and one page isn't enough.
You want to make it easy for people to find your other pages, so you create a
**navigation bar** (or "nav bar", for short).a

The Bootstrap documentation has some good examples for navigation bars, so you
should take what you see in the "getting started" example and modify it to fit
your webpage.

#### Your job

- create a navbar with a `navbar-brand` element containing the name of your site
- add a list of at least 4 sections to your nav bar

##### Challenges
  + Give your navbar a different color scheme using only Bootstrap classes
  + Make your navbar always stay in view, even when you scroll down
  + Add a search box on the right side of your nav bar

*All of the challenges can be completed by looking at the Bootstrap documentation*.

## Next steps

If you've completed the Scavenger Hunt and done all of the challenges, congratulations!

- Save your work
- Find a new cool feature in the bootstrap documentation
- Add it to your page
- In `Instructions.md`, write down a list of instructions that your friend can use
  to add the same feature to their page
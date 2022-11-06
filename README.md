# CSS_2 Visual Rules


The purpose of CSS is to add style to web page, and each element on the page can have many style properties. 

Some of the basic properties relate to the size, style, and color of the element. In this lesson, you’ll learn some fundamental CSS visual rules that you can use to start styling web page elements!


# Font Family

If you’ve ever used word processing software, like Microsoft Word or Google Docs, chances are that you probably also used a feature that allowed you to change the font you were typing in. 

Font refers to the technical term typeface, or font family.

To change the typeface of text on your web page, you can use the font-family property.

```
h1 {
  font-family: Garamond;
}
```


When the name of a typeface consists of more than one word, it’s a best practice to enclose the typeface’s name in quotes, like so:

```
h1 {
  font-family: 'Courier New';
}
```

# Class work


Here's the index.html and style.css file for this class.

Index.html/index.txt:

```
<!DOCTYPE html>
<html>

<head>
  <title>The Rise of Soccer in The US</title>
  <link href='style.css' rel='stylesheet'>
</head>

<body>
  <div class='content'>
    <img src='https://content.codecademy.com/courses/web-101/unit-4/htmlcss1-img_writer-avatar.jpg' class='writer-img'>
    <h3 class='byline'>Article By: Jane Dover</h3>
    <h1>How the Rise of Soccer in the US Is Changing the Face of Youth Sports</h1>
    <h2>The focus on soccer in youth sports programs is exploding nation-wide</h2>
    <p>When the first World Cup arrived in the US in the 90's everyone officially declared that soccer was it. Well it's taken it's time but we can definitely see the influence of soccer, especially women's soccer, across the US. This year, 3 million kids
      played in youth soccer leagues with 2/3 of those leagues for girls. In fact, in the 12-17 age range the MLS has surpassed the MLB and NFL in popularity.</p>
    <p>Part of this meteoric rise can be attributed to the impressively soaring ad dollars being pumped into the Women's World Cup games in 2014. The women's games generated $40 million for Fox, that's definitely not chump change. And those advertisers,
      like ATT, Coca Cola, Verizon, Nike, Visa, and other heavy hitters, are working to make sure they see those numbers grow year after year by investing in youth soccer facilities and promoting programs across the country. </p>
    <p>Now that big business is involved you can be assured you'll see a continued rise in popularity in soccer across the country for years to come. </p>
  </div>

  <div class='image'>
    <p class='caption'>The local semi- pro soccer team in Seattle, WA plays an international friendly</p>
  </div>
</body>

</html>
```


styles.css:

```
body {
    /* Old browsers */
    background: #141E30;
    /* Chrome 10-25, Safari 5.1-6 */
    background: -webkit-linear-gradient(-45deg, #35577D, #141E30);
    /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    background: linear-gradient(-45deg, #35577D, #141E30);
    margin: 0;
    padding: 0;
  }
  
  h1 {
    color: #FFF;
    font-size: 2em;
    padding-top: 100px;
    width: 100%;
    font-family: Georgia;
  }
  
  h2 {
    border-bottom: 1px solid rgba(255, 255, 255, 0.5);
    color: rgba(255, 255, 255, 0.5);
    font-weight: 100;
    font-size: 22px;
    line-height: 24px;
    padding-bottom: 30px;
    text-align: left;
    width: 70%;
    font-family: Georgia;
  }
  
  p {
    color: aliceblue;
    line-height: 1.3em;
    text-align: left;
    width: 100%;
    font-family: Helvetica;
  }
  
  .byline {
    font-family: Helvetica;
    color: rgba(255, 255, 255, 0.5);
    float: left;
    font-size: 14px;
    padding-left: 10px;
    text-transform: uppercase;
  }
  
  .caption {
    display: block;
    font-family: 'Playfair Display', serif;
    font-size: 14px;
    font-style: italic;
    line-height: 14px;
    margin-left: 20px;
    padding: 10px;
    position: relative;
    top: 80%;
    width: 60%;
  }
  
  .content {
    padding: 40px;
  }
  
  .image {
    background-image: url("https://content.codecademy.com/courses/web-101/unit-4/htmlcss1-img_soccer.jpeg");
    background-size: cover;
    background-position: center;
    height: 300px;
  }
  
  .writer-img {
    -webkit-box-shadow: 5px 0px 5px 0px rgba(0, 0, 50, 0.97);
    -moz-box-shadow: 5px 0px 5px 0px rgba(0, 0, 50, 0.97);
    box-shadow: 5px 0px 5px 0px rgba(0, 0, 50, 0.97);
    float: left;
    width: 50px;
  }
  ```
  
  
  

1 Inside style.css, set the font family of the main heading (h1) and subheading (h2) to Georgia.

2 Next, add a style rule that sets the font family of the paragraph (p) to Helvetica.




# Font Size

Changing the typeface isn’t the only way to customize the text. Oftentimes, different sections of a web page are highlighted by modifying the font size.

To change the size of text on your web page, you can use the font-size property.

```
p {
  font-size: 18px;
}
```

In the example above, the font-size of all paragraphs was set to 18px. px means pixels, which is one way to measure font size.


## Class work

In style.css, set the font-size of paragraph (p) elements to 18 pixels.



# Font Weight

In CSS, the font-weight property controls how bold or thin text appears.

```
p {
  font-weight: bold;
}
```

In the example above, all paragraphs on the web page would appear bolded.

## Class work

In the example above, all paragraphs on the web page would appear bolded.


styles.css:

```
p {
  color: aliceblue;
  line-height: 1.3em;
  text-align: left;
  width: 100%;
  font-family: Helvetica;
  font-size: 18px;
  font-weight: bold;
}
```

# Text Align

No matter how much styling is applied to text (typeface, size, weight, etc.), the text always appears on the left side of the container in which it resides.

To align text we can use the ```text-align``` property. The ```text-align``` property will align text to the element that holds it, otherwise known as its parent.


```
h1 {
  text-align: right;
}
```

The text-align property can be set to one of the following commonly used values:

- left — aligns text to the left side of its parent element, which in this case is the browser.
- center — centers text inside of its parent element.
- right — aligns text to the right side of its parent element.
- justify— spaces out text in order to align with the right and left side of the parent element.


## Class work

In style.css, set the text-align property of the main heading ```(h1)``` so that it appears in the center.


styles.css:

```
h1 {
  color: #FFF;
  font-size: 2em;
  padding-top: 100px;
  width: 100%;
  font-family: Georgia;
  text-align: center;
}
```


# Color and Background Color

Before discussing the specifics of color, it’s important to make two distinctions about color. Color can affect the following design aspects:

- Foreground color
- Background color

Foreground color is the color that an element appears in. For example, when a heading is styled to appear green, the foreground color of the heading has been styled. Conversely, when a heading is styled so that its background appears yellow, the background color of the heading has been styled.

In CSS, these two design aspects can be styled with the following two properties:

- color: this property styles an element’s foreground color
- background-color: this property styles an element’s background color


```
h1 {
  color: red;
  background-color: blue;
}
```

In the example above, the text of the heading will appear in red, and the background of the heading will appear blue.

## Class work


1 In style.css, set the background color in the .caption selector to white.

2 Then, in the same ruleset, set the color of the text to black. That should make the text a bit easier to read!

styles.css:

```
.caption {
  display: block;
  font-family: 'Playfair Display', serif;
  font-size: 14px;
  font-style: italic;
  line-height: 14px;
  margin-left: 20px;
  padding: 10px;
  position: relative;
  top: 80%;
  width: 60%;
  background-color: white;
  color: black;
}
```


# Opacity

Opacity is the measure of how transparent an element is. 

It’s measured from 0 to 1, with 1 representing 100%, or fully visible and opaque, and 0 representing 0%, or fully invisible.

Opacity can be used to make elements fade into others for a nice overlay effect. To adjust the opacity of an element, the syntax looks like this:

```
.overlay {
  opacity: 0.5;
}
```

In the example above, the .overlay element would be 50% visible, letting whatever is positioned behind it show through.


## Class work

Let’s give the caption on the image some transparency! In style.css, set .caption to have 0.75 opacity.


style.css:

```
.caption {
  display: block;
  font-family: 'Playfair Display', serif;
  font-size: 14px;
  font-style: italic;
  line-height: 14px;
  margin-left: 20px;
  padding: 10px;
  position: relative;
  top: 80%;
  width: 60%;
  background-color: white;
  color: black;
  opacity: 0.75;
}
```



# Background Image

CSS has the ability to change the background of an element. One option is to make the background of an element an image. This is done through the CSS property background-image. Its syntax looks like this:

```
.main-banner {
  background-image: url('https://www.example.com/image.jpg');
}
```

- The background-image property will set the element’s background to display an image.
- The value provided to background-image is a url. The url should be a URL to an image.



## Class work

In style.css, change the background image of the element with the.image class. The image is stored in the following URL: https://content.codecademy.com/courses/freelance-1/unit-2/soccer.jpeg


style.css:

```
.image {
  background-image: url("https://content.codecademy.com/courses/freelance-1/unit-2/soccer.jpeg");
  background-size: cover;
  background-position: center;
  height: 300px;
}
```



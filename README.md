# Y2 2018 Summer, Day 2: CSS Labs

## Lab 1
Before we begin, make sure to fork and clone this repository as we did yesterday:

  - Click the *Fork* button at the top right of the screen to make your own copy of the repository
  - Clone it as we did before:
  ```
  cd ~/Desktop
  git clone https://github.com/meet-projects/y2s18-css.git
  cd y2s18-css
  ```
 
1. Open hello.html and create a page with a header, two paragraphs, and at least one link.

2. Open style.css and create a style file such that the background color is blue and all text is white.

3. In your HTML file, add this somewhere inside the `<head>`:

```
<link rel="stylesheet" type="text/css" href="style.css">
```

4. Use [coolors.co](https://coolors.co/) to pick a better colorscheme for this website. Change the colors based on your new scheme, but do **not** use the style attribute!


### Extra

1. Learn more about color:
Read https://www.smashingmagazine.com/2010/02/color-theory-for-designer-part-3-creating-your-own-color-palettes/

2. Pick three of your favorite apps or websites, and explain which palette style they use.

3. Make another CSS file called style_alternate.css. Try your website with another colorscheme.


## Lab 2

### To get checked off, make sure you’re using a good color scheme for all the colors!

1. Use a CSS tag selector to change the color of all links.

2. Add a list of six favorite foods to your website. Use `<p>` tags to accomplish this. 

3. Use CSS class selectors to make vegetarian foods one color and non-vegetarian foods a different color.

4. Use a CSS id selector to give one element on your page a different background color.

5. Using Google and/or w3schools, find out what the following properties do. To get checked off, show each of them off on your website and explain them to your TA.
- font-family
- font-size

### Extra

- Pick one element in your page and give it a class and an ID. Then, add three CSS rules to style that element: one with a tag selector, one with a class selector, and one with an ID selector. Which one gets used? What happens if you have only two rules?
- Find or add two `<p>` and two `<a>` elements on your webpage and give all four of them the same class “muggle”. What happens if you use the selector “p.muggle” in `style.css` instead of ".muggle"? How about “a.muggle”? Explain these selectors to your TA to get checked off.
- Add a form to your website. You should have at least three checkboxes and one radio button. Add a CSS rule that makes selected checkboxes turn the area around them blue (you may have to add an extra `<div>` around it)

## Lab 3

1. Organize your page:

- In `hello.html`, give the header a class name of "title", and put the rest of your content (paragraphs and links) in a `<div>` with a class of "content".
- Make another `<div>` between the title and content with a class of "sidebar".
- Lastly, put the "content" and "sidebar" classes in another `<div>` with a class of "container".

If you're confused, look at the lecture slide with the title "Lab 3: Hints".

2. Open `style.css`. Give the sidebar a light background color of your choosing.

3. Make the title banner have a height of 60px.

4. Give the `container` class the `position: relative` property.

5. Give the sidebar and main content classes `position: absolute;` and `top: 0px;` Have the sidebar be positioned on the left margin of the page, and the main content be positioned 200px from the left.

6. Make it so the sidebar is exactly wide enough to touch the main content.

7. Give the container a height of 100%. 
- This is because the container has only absolutely positioned \<div\>s inside it, which means it has zero size by default.

8. Now, give the sidebar a height of 100%, to have it go all the way down the page.

9. Lastly, use the inspector on your browser (right-click on the page, then click "Inspect Element") to remove the `position: relative;` property from the `container` class. Notice how the position of the sidebar and main content changes, and show this demo to the TA to get checked off.

#### Extra:
- Center the text in the title banner using the `position` and `transform: translateX()` properties
- Make the sidebar have a gradient background


## Lab 4

1. Open `hello.html` in your browser, and open the inspector.

2. Notice the gap between your sidebar and the edge of the page. Using the inspector, click the `<body>` tag and look at the margin it has by default (the gray area that says `user agent stylesheet` at its top right).

3. In `style.css`, set the margin of `body` to 0px to get rid of this.

4. Give the sidebar a border of 5 pixels all around of any color and style. Now add padding of 10 pixels all around.

5. Reload the page on your browser. See how the sidebar is now leaking into the main content! Fix this. (For a hint, go to the lecture slide for Lab 4 Hints.)

6. Give the main content a border on the left of 2 pixels (any color and style), and a margin of 5 pixels. Also, give it padding on the left of 15 pixels.

7. As before, `git add`, `commit -m`, and `push` your code, so you have it for later.

#### Extra:
- Look up the `calc()` function and how it works, and explain it to a TA.
- Get rid of the scrollbar (that is, fit the page on the screen instead of having extra room at the bottom), possibly using the `calc()` function.

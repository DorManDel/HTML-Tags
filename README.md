# Fakeflix 🎬

A small HTML assignment project styled as a funny Netflix parody called **Fakeflix**.

The project keeps the required assignment structure, but changes the look and content into a darker streaming-style joke page with reviews, links, images, and a hidden Rickroll bonus.

---

## Project Pages

### Page 1
`index.html`

Contains:
- main title
- link to page 2
- link to paragraph 10
- 10 paragraphs
- bold words at the beginning of paragraph 1
- 2 images one under the other
- hidden Rickroll bonus

### Page 2
`index1.html`

Contains:
- main title
- link back to page 1
- secondary title
- numbered list
- each list item opens in a new tab
- 2 images side by side

---

## Design Idea

Instead of building a plain basic page, the site was turned into a parody streaming service called **Fakeflix**.

***The design was inspired by Netflix***

---

## Explanation of Important HTML and Style Parts

## 1. `<!DOCTYPE html>`
Tells the browser that this is an HTML5 document.

---

## 2. `<html lang="en">`
Starts the HTML page and tells the browser the page language is English.

---

## 3. `<head>`
Contains information about the page, such as:
- title
- encoding
- viewport settings

This part is not regular visible page content.

---

## 4. `<meta charset="UTF-8">`
Allows the page to display:
- English
- Hebrew
- symbols
- special characters

correctly.

---

## 5. `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
Helps the page scale better on smaller screens and phones.

---

## 6. `<title> ... </title>`
Sets the text shown in the browser tab.

Example:

```html
<title>Fakeflix - Page 1 - Dor Mandel</title>

7. <body style="...">

The <body> contains everything visible on the page.

Example:

<body style="margin:0; font-family: Arial, Helvetica, sans-serif; background-color:#141414; color:#ffffff;">
Meaning:
margin:0; removes default browser spacing around the page
font-family: Arial, Helvetica, sans-serif; uses a clean readable font
background-color:#141414; creates a dark Netflix-like background
color:#ffffff; makes the default text white
8. Main content container

Example:

<section style="padding: 20px; max-width: 1000px; margin: auto;">
Meaning:
padding:20px; adds space inside the section
max-width:1000px; prevents the content from becoming too wide
margin:auto; centers the content block horizontally
9. Main title styling

Example:

<h1 style="text-align:center; color:#e50914; font-size:48px; margin-bottom:10px;">
Meaning:
text-align:center; centers the title
color:#e50914; makes the title red
font-size:48px; makes it large
margin-bottom:10px; adds space under it
10. Box / card styling

Example:

<section style="background-color:#1f1f1f; padding:15px; border:2px solid #e50914; border-radius:10px; text-align:center;">
Meaning:
background-color:#1f1f1f; gives the box a slightly lighter dark background
padding:15px; adds space inside the box
border:2px solid #e50914; creates a red border
border-radius:10px; makes the corners rounded
text-align:center; centers text inside the box
11. How rounded corners work

Rounded corners are created with:

border-radius:10px;
Meaning:
border-radius controls how round the corners are
10px is the amount of roundness
bigger number = more rounded
0px = square corners

Example:

<section style="background-color:#1f1f1f; padding:15px; border:2px solid #e50914; border-radius:10px;">

In that line:

background-color creates the dark box
padding creates space inside
border adds the red outline
border-radius creates the rounded corners
12. Internal page jump

Example:

<a href="#paragraph10">Jump to Review 10</a>

This creates a link to another place on the same page.

And later:

<p id="paragraph10">

This marks the target.

Meaning:
href="#paragraph10" means jump to the element with id paragraph10
id="paragraph10" defines that location
13. Bold text in the first paragraph

Example:

<strong>Welcome to Fakeflix,</strong>

The <strong> tag makes the text bold.

This was used to satisfy the assignment rule that the first words of the first paragraph should be emphasized.

14. Paragraph content area

Example:

<section style="background-color:#1f1f1f; padding:20px; border:1px solid #333333; border-radius:10px; line-height:1.7;">
Meaning:
background-color:#1f1f1f; gives the paragraph area a dark background
padding:20px; adds inner spacing
border:1px solid #333333; gives a subtle border
border-radius:10px; rounds the corners
line-height:1.7; makes paragraph lines easier to read
15. Images

Example:

<img src="images/fakeflix-poster1.jpg" alt="Fakeflix poster 1" style="width:300px; border-radius:10px; border:2px solid #e50914;">
Meaning:
src="..." tells HTML where the image file is located
alt="..." gives fallback/accessibility text
width:300px; sets the image width
border-radius:10px; rounds the image corners
border:2px solid #e50914; adds a red border
16. Why the images stack on page 1

Example:

<br><br>

This forces the next image onto a new line and adds spacing.

That is why the two images on page 1 appear one below the other.

17. Why the images are side by side on page 2

Example:

&nbsp;&nbsp;&nbsp;&nbsp;

This adds visible spacing between the two images while keeping them on the same line.

18. External links opening in a new tab

Example:

<a href="https://www.youtube.com/watch?v=WSn1vS_wgB0" target="_blank" rel="noopener noreferrer">
Meaning:
href="..." is the destination URL
target="_blank" opens the link in a new tab
rel="noopener noreferrer" is a safer way to open external links
19. Hidden Rickroll bonus

Page 1 includes a tiny invisible secret clickable area.

Example:

<a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ" target="_blank" rel="noopener noreferrer"
   onclick="document.title='u got rickrolled';"
   aria-label="secret link"
   style="position:fixed; bottom:10px; right:10px; display:block; width:14px; height:14px; opacity:0;">
</a>
Meaning:
href="..." points to the Rickroll video
target="_blank" opens it in a new tab
onclick="document.title='u got rickrolled';" changes the browser tab title after clicking
position:fixed; bottom:10px; right:10px; places the hidden hotspot in the bottom-right corner
width:14px; height:14px; makes it tiny
opacity:0; makes it invisible

This is only a funny bonus and does not replace the assignment requirements.

20. Why <section> was used

<section> was used as a clean container to organize the page into blocks such as:

title area
navigation links
paragraph area
image area

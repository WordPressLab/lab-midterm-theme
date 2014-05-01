You are responsible for making the following changes to the following things.

## Fonts and Colors
Whenever you're asked to change a color you MUST use a hex color. When you are asked to change a font, you MUST use a google font.

## No Superfluous Code
If you are using the method of copy pasting from Firebug, you may only include the CSS that you are actually changing.

## Best Practice for Doing This
Use your searching skills for this. If you come across something you don't know how to do, 
1. Consult the Midterm assignment page in the "Things to Help You Do This" section
2. Google the phrase "css [thing you want to do]" and nine times out of ten, you'll get your answer first try.

# Specific Changes

## Basic elements

### h1-h6
- Start big and then evenly decrease both the __size__ and __top/bottom margins__ of each successive heading
-- To clarify: You are giving each heading a new size and top/bottom margin
- change font and color of each

### p
- change font for all paragraphs

### Layout
- This is a freebie. Create a right-hand sidebar.
-- go to "__lab-midterm-theme/layouts__" and copy the contents of "__content-sidebar.css__" into your child theme's stylesheet.

#### Sidebar
##### Widgets

- Change the background color of .widgets
- Change the list-style of unordered lists __within the sidebar div__. 
	- This means you're changing the lists within the widget area but not anywhere else.
- Change the color of links 
- Change the color of links when you hover using the selector a:hover

## Specifics
### site-title and site-description
- Set the margins between them so that there is a total of exactly 63 pixels of space betweet them

### entry-title
- Change text-decoration or remove it
- Reduce the top and bottom margins

### cat-links and tags-links 

####(the category and tag links at the bottom of each post on the front page)

- Change the font color
- Change the background-color
- Increase the padding on all sides
- Remove the text decoration

Create a second CSS class, using a:hover, have the font color and background color switch places.

__Clarification:__ You can use the same set of rules for both cat-links and tags-links. In fact, you can include them both in the same CSS class by separating them with a comma. 

    .cat-links a, .tags-links a {
       some: code;
       some: code;
    }

### Menu
- Make the navigation menu visible through color or borders or however you feel
- Add spacing between the menu items
- Give the menu items colored backgrounds and/or borders
- Change menu item font and color


# Modifying Templates
Since we're making a child theme, you need to copy the following template files to your theme to edit them

- header.php
- index.php
- content.php
- single.php
- sidebar.php
- footer.php

This part of the test will have you go through various template files and add identifying notes to show that you are able to navigate through a theme.

## Identify Where Major Divs Start and End
Search through the required template files and find where the major page containers are created and where they end. What are the major page containers? They’re very similar to the ones that you revealed back in HW 2 with one difference. What was “content” in twentytwelve is “entry-content” in our theme. They are as follows:

- body
- page
- masthead
- site-navigation
- main
- primary
- entry-content
- post
- secondary
- colophon

## Do What With Them?
Each one of these is the id or class of a one of the major divs that make up any given page on your website. You are going to add a code note (like in HW 3) in two places:

1. Below the opening tag, put "start of [div name]
2. Below the closing tag, put "End of [div name]


## Code Note CSS Class
You will need to create a special class for your notes so that they are unobtrusive but still legible. We are benevolent teachers and will give you the class to use.

    .code-note {
      color:black;
      font-family: Monaco, monospace;
      font-size: 8px;
      margin: 0px;
    }
    
## Where To Add Code Notes
You must add an explanatory note in the code directly below where major containers (i.e. `<div>`s like "__page__".) are produced in the template files.

### Example
    <div class="page">
      <h6 class="code-note">This is the page div</h6>


# Screenshot
This is a professional theme, make it look like it. We don't want some blank rectangle showing up in the theme manager. Just take any rectangular image and title it "__screenshot.png__" and put it in your child theme folder.

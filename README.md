# marketing-refactor

# Description

This project was about refactoring an exsisting website for horiseon marketing. The code used for their website was filled with div elements and their over use of classes and duplicate CSS selectors were somewhat of a nightmare to look at. My job was to clean this up to make the website more accesible and readable for developers in the future. I was provided a list of acceptance criteria by the client and was sure to check off all those boxes so I could supply the code they were seeking. 

## Installation 

To install this repo on your local drive you would have to clone the ssh key from my repo. Head into your local drive of choice in terminal or bash and do a git clone. Once you have done a git clone you are free to start working on this project. If you want to push your changes to my repo then you would have to head into terminal/bash to a git add .   then a git commit -m explaning the changes made, and finally a git push to push the files onto the repo. 

## Changes made to index.html 

There was many steps that had to be taken to get this code to a more semantic, accesible state then the one it was in when I found it. First step was to add a concise, descriptive title, i placed this inside the head elemnt of the index.html page. Next was to address the over use of divs in the index.html element. One of the acceptance criteria from the client was to have semantic html. I replaced all the divs in the html with what would semantically fit, adding header, h1, nav, main, section, figure, and aside elements. One link in the nav bar was not linked to its correct section so i cleaned that up by adding a id to the corresponding section. Having working links that directed to the right section was also in the acceptance criteria from the client. Another criteria was to make sure all img elements contained an alt tag with content inside them. I added this element to all of the img tags as well as removing the uneeded / at the end of the img tag. To make the page more accesible for screen readers a title element was added to the figure element, which was the background image. Some headings didn't follow sequential order, there was a h2 tag in the footer that came after a h3 tag so i changed it to a h4. I shortened the class and id names to make them more concise and removed duplicate class names and changed them to all having the same class name where it was fit in the pertaining sections. The class names were treated as id's at times when they were all having the same styling, so one class was the better option.

## Changes made to style.css

The style sheet in the code I was given to refactor was filled with its overuse of class selectors and generally bogged down by having selectors filled with multiple class names doing the same thing. There was also selector that were useless such as the p element selector. It had a property of font-size that was already specified elsewhere. The real issue's came from how the index.html was laid out. As stated in the previous section classes were used as id's at times, giving each section its on class name when they were all to be styled the same way. The main element contained 3 sections that all had their own class name which wasn't needed, and the style sheet had a selector for each one of them. Once I made them all one class then I removed the 3 selectiors in the CSS and made it one selector for the entire class. I had to do the same thing with the aside element. It also contained 3 sections with 3 different classes all doing the same thing. I again made them all one class and then trimmed down the style sheet accordingly. Both the main element and the aside elemnt contained images in the child elements, these images were all styled seperately becasue before the parents had seperate class's.Yet again I was able to consolidate these down to one selector for all now that they had one class and not multiple. My final step in the style sheet was to make sure it was properly commented for ease of understanding.

## Finished project 
My page is live on github!

https://mattrward1030.github.io/marketing-refactor/

<img src="./assets/images/webpage.png" alt="screenshot of my live webpage">

## Contributing 

Pull requests are welcome and encouraged

## License 

MIT License

Copyright (c) [2021] [Matthew Ward]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

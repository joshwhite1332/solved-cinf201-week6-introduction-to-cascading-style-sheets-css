Download Link: https://assignmentchef.com/product/solved-cinf201-week6-introduction-to-cascading-style-sheets-css
<br>
<strong>What is CSS? </strong>

CSS stands for Cascading Style Sheets. Unlike HTML, which is used to represent the structure of a web page, CSS is the language for the determining the presentation of a page in terms of colors, fonts, positioning, etc. We use CSS to select specific HTML elements to give them styles.




After selecting specific elements (either directly or based on certain criteria), we can then choose whatever properties we’d like and give them different values. An example would be targeting paragraph tags and giving them a red font color. We can do that with the code below:




p {

color: red;

}




“p” is the selector (all paragraph tags), “color” is the property, and “red” is the value we are assigning to the property. The selector comes first followed by curly brackets “{}”. The curly brackets represent a block of CSS declarations. Inside of the curly brackets is where we choose our properties and values, and each set is a CSS declaration. The properties and values are always separated by a colon and the whole statement (color: red) is ended with a semicolon.




It is <strong>best practice</strong> to separate your HTML and CSS by using an <strong>externally placed style sheet</strong>. The reason for this is because it is easier to update your code if it is in a different location. If you have a consistent banner style on many pages of your website and use inline/internal styling, you would have to go into the code for each page and edit it. If you use external styling, you can edit the code in one place and the changes would persist across all pages.




Just like HTML and other languages, we can add comments to our files in addition to regular code. In CSS, commenting is simple and requires only slashes and asterisks. To add a comment, use the syntax below:




/* This is a comment */




Anything between the asterisks is the comment content and won’t affect styles being applied.

Comments are useful if you want to keep a style, but prevent it from affecting the page. They’re also helpful for general documentation purposes and I recommend using them to distinguish different sections of your page.




<strong>How can we add styles to a page? </strong>

There are three main ways for implementing CSS on a web page and each one is explained below with a link to an example. To see the code in the example, right-click the page and select “View Source” or “Inspect Element” and look around the window that appears.

<u>Inline CSS</u>

This is typed directly into the HTML tag as part of the style attribute. The line below will do the same thing as the CSS demonstrated above. However, it will only apply to the HTML tag where it resides.

&lt;p style=“color: red”&gt;This is a red paragraph.&lt;/p&gt;

<u>Internal CSS</u>

This is CSS typed between &lt;style&gt;&lt;/style&gt; tags which are located inside of the &lt;head&gt;&lt;/head&gt; tags of your HTML document. I’ve used this in some of the assignments this semester to give our tables styles.

In the CSS declaration below, I select the table, tr, th, and td tags to give them all a solid black border that is 1px in width. I then collapse the border, so it appears as one line and then add a little padding, so the text is easier to read.

&lt;style&gt;

table, tr, th, td {         border: 1px solid black;         border-collapse: collapse;         padding: 5px;

}

&lt;/style&gt;

<u>External CSS – BEST PRACTICE</u>

This is CSS placed in a separate document with a “.css” extension. It is connected to our HTML through the usage of a &lt;link&gt; tag which is placed inside of the &lt;head&gt;&lt;/head&gt; tags. The link tag uses two attributes which are rel and href.

The rel is required to explain the relationship between our resource and the HTML. Here, we are saying it’s a style sheet. The href section is where you link your CSS style sheet. Like working with local images, you need to include folder/file names accurately to link them correctly. In the example below, my CSS file is located in a css folder which I refer to before the file itself.

&lt;head&gt;

&lt;link rel=”stylesheet” href=”css/style.css”&gt;

&lt;/head&gt;

View of my folder structure (style.css is inside of the css folder):




Since I use “css/style.css” my CSS file should be inside of that folder. If I wanted to have my HTML and CSS files be in the same folder, the link tag would be changed so that the href had style.css as shown below.

&lt;link rel=”stylesheet” href=”style.css”&gt;




View of my folder structure (they’re blue because I selected both items in my folder):







A lot of students tend to put both files in the same folder. I would recommend keeping them separated like they are in the first screenshot. This will keep your files organized and is helpful for assignments/the final project. When you move your files to FileZilla, the folder organization there should be the same as it is on your local machine. <strong>If your CSS doesn’t work at all with your HTML, it’s probably because the href value is incorrect. </strong>




<h2>CSS Examples</h2>

Open a text editor and follow along as I demonstrate how we can use CSS on a page. I will go over the general syntax and show you how to apply styles and check them with web developer tools in the browser. For my demo, I will be using Brackets and Google Chrome.




<u>Online Resources (Not required reading, only meant to help you if you need it)</u>

<ul>

 <li><u>https://www.htmldog.com/guides/css/</u> – CSS Tutorials for all levels</li>

 <li><u>https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps</u> – Excellent resource with guides/tutorials for CSS</li>

 <li><u>https://www.tutorialspoint.com/css/css_syntax.htm</u> – Specific syntax examples</li>

 <li><u>https://css-tricks.com/</u> – Cool website for code snippets and articles</li>

</ul>

<h1>First CSS Exercise (CW/HW)</h1>

<strong><u>There are two parts to this assignment.</u></strong> For the first part, you will add CSS styles to a web page so that it matches a provided image as closely as possible. In part two, you will open an existing web page and inspect it. After inspecting the page, you will alter the styles on the page and take a screenshot of the changes.

Part 1

Download the “First-CSS-Exercise.zip” folder from Blackboard under today’s Lecture Notes or the Assignment folder. Extract everything from inside of this zip folder to some place where you will be able to find them easily. There will be an HTML file, a css folder with a style.css file in it, and an image with an example of a finished assignment.




Based on the instructions below, add CSS to the style.css file to alter the way the page looks. The image I’ve provided is an example of how the assignment should look after you are done with it. Your page should look exactly like mine if you follow my instructions listed below.




To get started, extract all the files from the Zip folder on Blackboard or get them from the link mentioned above. Open the HTML/CSS files inside of a text editor and add code as necessary. All CSS should go inside of the style.css file. You don’t need to include any tags, only CSS should be inside of that document.




For all assignments/project work in this course, your CSS must be <strong>externally placed.</strong> This is because it will be easier to manipulate styles on your page if the styles are separated. I would recommend leaving the “.css” file inside of the folder provided. Otherwise, you will have to change the href value in your link tag. The instructions for the styles I’d like to see are listed below.




<u>Instructions for Adding CSS</u>

<ul>

 <li>Give the body a font-family of verdana, a font size of 16px, and a background of black</li>

 <li>Give the h1 a background of black, a color of white, and a font size of 2em</li>

 <li>Give the paragraph right after the h1 a color of white (“+” selector” is good if you want to use it)</li>

 <li>Give each div a background color of “#ccc”</li>

 <li>Each h2 should be centered aligned and have a font size of 1.4em</li>

 <li>Each paragraph should have a line height of 1.3</li>

 <li>Content inside of Div with the class of “firstDiv” o The h2 and span tags should have a color of blue o The span tags should have a white background color and a 1px solid blue border o The unordered list should have its list-style-type property changed to square o The unordered list items should have the odd list items appear with a blue background and white text (nth-child selector on li tag – 1<sup>st</sup>, 3<sup>rd</sup>, 5<sup>th</sup> list items targeted)</li>

 <li>Content inside of Div with the class of “secondDiv” o The h2 and span tags should have a color of green

  <ul>

   <li>The span tags should have a white background color and a 1px dashed green border</li>

   <li>The table, th, and td tags should have a black background, white color for the text, and a solid white 1px border. The th and td tags should have 4px of padding added to them.</li>

  </ul></li>

</ul>










<h2><u>Extra Credit </u></h2>

Complete the assignment without using any classes in your CSS file. This means you would only use element names and no classes or ids in your CSS selectors. You will need to utilize various pseudo-classes such as nth-child, nth-of-type, etc. in your CSS selectors to do this. This is a bit tougher and requires that you be creative with your selector choices. There are also many routes to getting it done, feel free to use whatever selectors you need.




<h3>Part 2</h3>

Open a web page of your choosing and inspect it as shown earlier in class. To inspect a page, you can right-click the page and select “Inspect” or you can use F12 on a PC. If you’re in Safari, you might have to activate the developer tools options in your preferences.




After you’ve opened a web page and inspected it, a panel should appear which displays HTML and CSS. Your task for this part is to alter the CSS for various elements on the page so that it is significantly different than the original version. There is no right or wrong process here, your goal is simply to play with the styles you see and change the page. If you see a style you don’t understand, look it up and try something new.




The main thing I want to see is that you’ve experimented with different CSS property/value combinations and have documented the changes. After you’re done making your changes, take a screenshot of the new version of the page and attach it with your submission. You can write a list to document your changes instead of in a paragraph.




<u>Tips</u>

<ul>

 <li>Change the values for properties (feel free to try the ones listed here) o Font-size o Font-family o Color o Background-color o Border o Margin o Padding o Text-align o Text-decoration o Line-height</li>

 <li>Uncheck some boxes for styles</li>

 <li>Target large items on the page for more visible changes</li>

 <li>Use the selector tool (box with an arrow – furthest left icon) to pick items to change</li>

 <li>Don’t refresh the page or your changes will be lost</li>

</ul>




<h2><u>First CSS Exercise – </u></h2>

<ul>

 <li>Part 1: 8pts o Live link was submitted: 1pt o CSS is externally placed: 1pt o CSS is organized/nested neatly: 1pt o All required styles are included: 5pts</li>

 <li>Part 2: 2pts o Numerous changes were made: .5pt</li>

</ul>

o Explanation of changes/website name included: .5pt o Screenshot of changes included: 1pt




<h1>Participation Questions 9/30</h1>

To receive credit for participation in today’s class, please answer all the questions in the Google Form linked below. If you don’t want to answer the final question (fun), simply put N/A (not applicable) for your answer and that will count.




<h2>This Week’s Participation Questions: <u>https://forms.gle/rMaLpfDhz1gT7UgJ7</u></h2>




<strong>Previous Participation Questions/Responses </strong>These are the participation questions from last week:

<u>https://forms.gle/W6dBh1R4NCAfwN7T8</u>




This link has the responses to the fun question from last week. Feel free to look over the responses from myself and your peers.  <u>https://docs.google.com/spreadsheets/d/1QLoQzbO-</u>

<u>Er7ARIECl0aPvY1lKUyZTdYeuwsn4g0XEAk/edit?usp=sharing</u>



HTML (hyper text markup laungage)  
-it is a laungauge for creating webpages  

◯ diffrence between element and attribute :-   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Element - An element is a complete HTML part that contains a tag and content.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;e.g. - p Hello /p    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Attribute: An attribute gives extra information about an HTML element.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;e.g. - p class="text" Hello /p     → class="text" is an attribute.  

◯ sementic elements :-  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;article - it is used for independent content that can stand on its own, such as a blog post, news article.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;aside - it is used for extra content related to the main content, such as a sidebar, quote, or advertisement.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;details - it is used to show extra information that the user can click to open or hide, such as FAQs or expandable sections.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;figcaption - is used to add a caption or description to a figure, such as an image or diagram.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;figure - it is used for self-contained content, such as an image, diagram, or code, often with a figcaption for its caption.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;footer - it is used for the bottom part of a page or section, usually containing copyright, contact information, or links.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;header - it is used for the top or introductory part of a page or section, usually containing headings, logos, or navigation.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;main - it is used for the main content of a webpage, excluding headers, footers, and sidebars. There should be only one main element per &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; page.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;mark - it is used to highlighted the text.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;nav - it is used to contain important navigation links, such as a website menu.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;section - it is used to group related content into a section, usually with a heading.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;summary - it is used to create a visible heading that users can click to open or close the details content.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;time - it is used to show specific date or time, and the datetime attribute gives the date or time in a format that computers can understand.   

◯ block level element :-
it start on a new line and usually take the full available width They are used for things like headings, paragraphs, and &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sections. e.g. - div, p, h1-h6, ul, ol, form, section, article  

◯ inline element :-
do not start on a new line and take only the space they need. They are used for small parts of content, like words or links. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; e.g. - span, a, strong, em, img, b, i, q, abbr.  

◯ class and id attributes :-  
class - it gives an element a name, so you can style or control multiple elements together.   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (it can be used multiple times, it is used to styling the elements)  
id - gives an element a unique name so you can style or control that specific element    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(it can be mut unique, it is used to linking a specific elements)  

◯ iframe :-  
it is used to show content from another website inside your webpage, such as a webpage, video, or map.  
src → Tells what content to show.  
width → Sets the width of the iframe.  
height → Sets the height of the iframe.  
name → Gives the iframe a name so links or scripts can target it.  
frameborder → Controls whether the iframe has a border.  
allow → Gives permission for features like fullscreen or microphone.  
sandbox → Adds security restrictions to the iframe.  
title → Gives a description of the iframe for accessibility.    

◯ meta tags :-  
are always placed inside the head section of your HTML document and primarily handle four critical tasks :  
1. Search Engine Optimization (SEO - SEO helps search engines understand your website and helps users find your pages easily) & Indexing (indexing is the process where a search engine stores and organizes the content it finds so it can be shown in those results)  
2. Responsive Web Design (Viewport Control - it instructs mobile browsers how to control a webpage's dimensions and scaling behavior)   
3. Character Encoding (it is a system that pairs human-readable letters, numbers, and symbols with unique numerical values so a computer can store, process, and display text)  
4. Browser & HTTP Directives (they are specific instructions sent in HTTP headers that tell browsers and servers how to handle cached content, security policies, and data transmission)  

◯ quoatation and citation elements :-  
blockquote - is used for long quotes from another source  
q - it is used for a short quote, usually with quotation marks around it  
abbr - it is used for short forms and the title attribute shows the full meaning when you hover over it.  
address - it is used to show contact information, such as an email, phone number, or address  
cite - is used for the title of a creative work, such as a book, movie, article, or course, usually shown in italic.  
bdo - it changes the direction of text, such as making text go left-to-right or right-to-left.   

◯ html list attributes :-  
ul - Defines an unordered list, typically displayed with bullet points.  
ol - Defines an ordered list, typically displayed with numbers or letters.  
li - Defines a list item within ul or ol.  
dl - Defines a description list for terms and their descriptions.  
dt - Defines a term in a description list.  
dd - Defines a description for a term in a description list.  

◯ tabel elements :-  
tabel - Defines the table.  
tr - Defines a table row  
th - Defines a table header cell (bold and centered by default)  
td - Defines a table data cell   
caption - Defines a table caption, typically displayed above the table.  
thead - Groups header content together, mainly to give the page a clear structure.  
tbody - Groups the main body content together to give the page a clear structure.  
tfoot - Groups footer content together, usually for contact details, copyright, or links.  

◯ image tags and attributes :-  
src - it specifies the path of image file to be displayed   
alt - it provides the alternative text for the image and it is used to screen displayed if the image fails to load  
width - it is use to set image's width   
height - it is use to set image's height  
loading - it is used to imporove page load perfomane by maning image load behaviour  
    lazy : it Delays loading the image until it is near the viewport    
    eager - Loads the image immediately, even if it is far down the page. This is the default behavior when loading is not specified.  
    auto - The browser decides when to load the image based on the situation. It can load it now or later.  
title - it provides a tooltip that appears when the user hovers over the image.  
usemap - it is used to link an image to a map so that different parts of the image can be clicked.    
map - It makes different parts of an image clickable, and each part can open a different link.  
srcset - it gives the browser different image options, so it can choose the best image for the screen.  

◯ form elements :-
input - it is used to take input from the user, such as text, email, password, number, or date.  
label - is used to give a name or description to a form input, making it easier for users to understand what to enter.    
select - it is used to create a drop-down list where the user can choose an option.  
textarea - it is used to create a multi-line text box where users can enter longer text.  
button - 
fieldset - it is used to group related form elements together, such as fields for personal information.  
legend - it is used to add a title or caption to a fieldset.  
datalist - it provides a list of pre-defined options that the user can choose from when typing in an input.  
output - it is used to show the result of a calculation or user action.  
option - it is used to define an option that the user can choose in a select or datalist.  
optgroup - it is used to group related options together in a select drop-down list.  

◯ formating elements :-  
b - bold   
i - italic  
strong - it shows important text, usually displayed in bold.  
em - it give extra importance to a word or text in italic  
mark - highlighted text  
small - it makes text smaller, usually for fine print or extra notes.   
del - deleted text  
ins - it shows newly added text, usually displayed with an underline.  
sub - makes text smaller and lower than normal text, often used in chemical formulas.  
sup - it makes text smaller and higher than normal text, often used for powers/exponents.    

◯ style  attribute :-  
text color -   
background colour -   
font family -    
font size -   
text align - left, right, center(Text is aligned in the middle), justify(Text is aligned evenly on both the left and right sides) 
padding - it adds space inside an element, between the content and the border.  
margin - it adds space outside an element’s borders   
border -   

◯ audio attributes :-  
src: Specifies the path or URL to the video file (used when no source elements are provided).   
controls: Displays browser-native video controls (play, pause, volume, etc.).   
autoplay: Plays the video automatically on page load (often requires muted).   
loop: Repeats the video indefinitely.   
muted: Mutes the video by default.  
poster: Specifies an image to display before playback starts.  
width: Sets the video width in pixels or percentage.   
height: Sets the video height in pixels or percentage.   
preload: Suggests how the browser should load the video (none, metadata, auto).  
crossorigin: Specifies CORS settings for fetching the video (anonymous, use-credentials).   
playsinline: Allows the video to play inline on mobile devices (avoids fullscreen).  
disablePictureInPicture: Disables the picture-in-picture option in browsers.  
mediagroup: Groups media elements for synchronized playback (non-standard, rarely used).  

◯ computer code elements :-
code - it is used to show small pieces of code, such as function names, variables, or commands, usually in monospace font.  
pre - it shows preformatted text and keeps the same spaces, tabs, and line breaks as written in the HTML. It is commonly used for multi-line code.  
kbd - it is used to show what the user should type or press, such as keyboard keys, shortcuts, or commands.  
samp - it is used to show output from a computer program or system, such as messages, results, or error messages.  
var - it is used to show a variable or placeholder, such as a variable in code or a math formula.  

◯ html links :-  
a - it is use to create a link  
href - it Specifies where the link will take you.  
target - it Specifies where the link will open, such as in the same tab or a new tab.  
        _self : Opens the link in the same tab/window   
        _blank : Opens the link in a new tab or window  
        _parent : Opens the link in the parent frame  
        _top :  Opens the link in the full body of the window  
title - it Provides additional information about the link, shown as a tooltip on hover.  
download - it Makes the browser download the file instead of opening it.  

◯ link colours :-  
By default, browsers style links with colors: blue for unvisited, purple for visited, and red for active. These can be customized using CSS by targeting the a tag and its pseudo-classes:  
:link – Unvisited link.  
:visited – Visited link.  
:hover – Mouse over link.  
:active – Link being clicked.  

◯ heading and paragraph tags :-    
heading tags : h1 to h6, p  
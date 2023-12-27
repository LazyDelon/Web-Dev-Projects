# Getting Started with Web Development

### 🎓 Topics

**1. Introduction to development environment, installation & basic syntax**  
**2. xxx**


## 📋 Setting up your environment 

**This curriculum has a development environment ready to go! As you get started you can choose to run the curriculum in a  [Codespace](https://github.com/features/codespaces/) (_a browser-based, no installs needed environment_), or locally on your computer using a text editor such as [Visual Studio Code](https://code.visualstudio.com/?WT.mc_id=academic-77807-sagibbon).**


### Running the curriculum locally on your computer

**To run this curriculum locally on your computer, you will need a text editor, browser and command line tool. Our first lesson, [Introduction to Programming Languages and Tools of the Trade](https://github.com/microsoft/Web-Dev-For-Beginners/tree/main/1-getting-started-lessons/1-intro-to-programming-languages), will walk you through various options for each of these tools for you to select what works best for you.**

**Our recommendation is to use [Visual Studio Code](https://code.visualstudio.com/?WT.mc_id=academic-77807-sagibbon) as your editor, which also has a built-in [Terminal](https://code.visualstudio.com/docs/terminal/basics/?WT.mc_id=academic-77807-sagibbon). You can download Visual Studio Code [here](https://code.visualstudio.com/?WT.mc_id=academic-77807-sagibbon).**

### Download Visual Studio Code

**1. Open the web page https://code.visualstudio.com/：** 

&nbsp; <img src="./Images/vscode - download step0.png" alt="Download step0"/>

**2. Click `Download for Windows` to download the installation file. After the download is complete, open the installation file：** 

&nbsp; <img src="./Images/vscode - download step1.png" alt="Download step1"/>

**3. Click I agree, then click Next：** 

&nbsp; <img src="./Images/vscode - download step2.png" alt="Download step2"/>

**4. Click next：** 

&nbsp; <img src="./Images/vscode - download step3.png" alt="Download step3"/>

**5. Click next：** 

&nbsp; <img src="./Images/vscode - download step4.png" alt="Download step4"/>

**6. Installing, waiting for installation to complete：** 

&nbsp; <img src="./Images/vscode - download step5.png" alt="Download step5"/>

**7. The installation is complete, click Finish：** 


➤  **資料來源：** [**在 Windows 10 安裝 Visual Studio Code**](https://etrex.tw/free_chatbot_book/windows_dev/vscode.html)   

## 🎓 CSS Selectors

In CSS, selectors are patterns used to select the element(s) you want to style.

Selectors, whether used in CSS or JavaScript, enable targeting HTML elements based on their type, attributes, current states, and even position in the DOM. Combinators allow you to be more precise when selecting elements by enabling selecting elements based on their relationship to other elements.



### Group selectors: [selectors A], [selectors B]
**Use a comma to separate two selectors, which means that the same style will be attached to the elements that match any one of them. In this way, multiple selectors can be circled to avoid writing the same rules repeatedly.**



### Composite class selector: [selectors A][selectors B]
**If an element has more than one category, and we want to distinguish it by the category it has, we can choose to use a compound class selector. For example, today there is a div that has additional categories in addition to the basic component category, such as width-2x or width-3, etc., then we can mark .component.width-2x or .component.width-3x Make a distinction.**



### Subpoint selectors: [selectors A] > [selectors B]
**When we want to change the attributes of some sub-elements under an element, we can use the sub-point selector to help us quickly apply to all sub-elements that meet the conditions of selector B.**

**What needs to be noted here is that the so-called children only cover the first level of child nodes under the element, and the elements below each node are not within the scope of the child selector.**



### Descendant point selectors: [selectors A] [selectors B]
**Since the child point selector can only select the first level of child points, what if we want to apply the style to the DOM tree rooted at a certain element (such as setting font-size)? At this time we can use the descendant point selector to achieve this goal.**

**A reminder here is that there is no blank space between the two selectors of a composite selector, while descendant selectors must be separated by at least one blank space.
That is: .classA.classB is not equal to .classA .classB**



### Adjacent selectors: [selectors A]+[selectors B]
**Since there are selectors for selecting descendant points, of course there is also a way to select neighbors (siblings), and the first one to appear is the adjacent selector. The scope of application of this selector is: if there is an element that meets condition A, and the first neighbor below it also meets condition B, then this style will be applied to that neighbor.**

**To be honest, I don't use this selector very often at the moment. When I use it, I usually have to make sure that the two elements are adjacent in the web page structure. The simplest way I can think of is <img> and <figcaption> in <figure>. After all, they usually exist at the same time and are adjacent.**


### Post-selectors: [selectors A]~[selectors B]
**The restriction of adjacent selectors is that they must be adjacent to be effective, while the posterior selector is applied to all sibling elements on the same layer.**

**So if you only want to apply to adjacent elements, use the adjacent selector. If you want to apply to all elements at the same level, you can use the trailing selector.**

➤  **資料來源：** [**CSS Selector Reference**](https://www.w3schools.com/cssref/css_selectors.php)   


## 🎓 HTML Input Types

| **Value** |	**Description** |
| ---- | ---- |
| **button**	| **Defines a clickable button (mostly used with a JavaScript to activate a script)** |
| **checkbox**	| **Defines a checkbox** |
| **color**	| **Defines a color picker** |
| **date**	| **Defines a date control (year, month, day (no time))** |
| **datetime-local**	| **Defines a date and time control (year, month, day, time (no timezone)** |
| **email**	| **Defines a field for an e-mail address** |
| **file**	| **Defines a file-select field and a "Browse" button (for file uploads)** |
| **hidden**	| **Defines a hidden input field** |
| **image**	| **Defines an image as the submit button** |
| **month**	| **Defines a month and year control (no timezone)** |
| **number**	| **Defines a field for entering a number** |
| **password**	| **Defines a password field** |
| **radio**	| **Defines a radio button** |
| **range**	| **Defines a range control (like a slider control)** |
| **reset**	| **Defines a reset button** |
| **search**	| **Defines a text field for entering a search string** |
| **submit**	| **Defines a submit button** |
| **tel**	| **Defines a field for entering a telephone number** |
| **text**	| **Default. Defines a single-line text field** |
| **time**	| **Defines a control for entering a time (no timezone)** |
| **url**	| **Defines a field for entering a URL** |
| **week**	| **Defines a week and year control (no timezone)** |

**The ‵<input>‵ HTML element is used to create interactive controls for web-based forms in order to accept data from the user; a wide variety of types of input data and control widgets are available, depending on the device and user agent. The <input> element is one of the most powerful and complex in all of HTML due to the sheer number of combinations of input types and attributes.**

➤  **資料來源：** [**Input Types - Steam 教育學習網**](https://steam.oxxostudio.tw/category/html/tags/input.html)   


## 🎓 CSS Box Model 

**The essence of the CSS box model is a box that wraps each HTML element. It refers to the area occupied by an element in the screen. Its components include: `margins`, `borders`, `padding` and `content`, and each HTML element is a box model. , the picture of a complete web page is composed of many elements.**


**Content refers to the real content of the element, such as the real content of text or pictures. We can adjust the `width` and length of the content through width and `height`. Inside the border is the padding. If you increase the padding, the distance between the content and the border will become larger; and outside the border will be the margin. If you want to space it out from other elements The distance needs to be achieved by setting the distance.**

**In fact, in the history of browsers, there are two kinds of box models, one is `content-box` (W3C standard box model), and the other is `border-box` (IE box model). At present, the box model can be freely set through the `box-sizing` of css. If not set, the default value will be `content-box` (after all, IE has already retired).**

**The difference between the two is that the two box models have different standards for calculating the width and height of the box. The width and height of the `content-box` box will only contain content, not padding and border; but the box model of `border-box` will include content, padding and border, as shown in the figure below.**

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




**Post-selectors: [selectors A]~[selectors B]
The restriction of adjacent selectors is that they must be adjacent to be effective, while the posterior selector is applied to all sibling elements on the same layer.**

**So if you only want to apply to adjacent elements, use the adjacent selector. If you want to apply to all elements at the same level, you can use the trailing selector.**

➤  **資料來源：** [**CSS Selector Reference**](https://www.w3schools.com/cssref/css_selectors.php)   



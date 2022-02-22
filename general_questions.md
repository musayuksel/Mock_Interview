# General

## HTML / CSS

<details>
<summary>What is the meaning of semantic HTML?</summary>
 Semantic markup isn't about performance, it's about meaning.
 In HTML, for example, the h1 element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."<br>
 Search engines will consider its contents as important keywords to influence the page's search rankings<br>
 Screen readers can use it as a signpost to help visually impaired users navigate a page<br>
 Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes<br>
Suggests to the developer the type of data that will be populated
Semantic naming mirrors proper custom element/component naming
</details>

<details>
<summary>Which elements in HTML are non-semantic? And why do we need them?</summary>
block: div
inline: span
They don’t tell anything about the content they contain. They can be used with different attributes to mark up semantics common to a group.
</details>

<details>
<summary>What is the meaning of accessibility?</summary>
Accessibility is the practice of making your websites usable by <strong> as many people as possible.</strong> We traditionally think of this as being about people with disabilities, but the practice of making sites accessible also benefits other groups such as those using mobile devices, or those with slow network connections.
</details>

<details>
<summary>What is the meaning of specificity in CSS?</summary>
Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.
When an <i>!important</i> rule is used on a style declaration, this declaration overrides any other declarations.</br>
Although technically <i>!important</i> has nothing to do with specificity, it interacts directly with it. 
<strong>bad practice</strong></br>
<h3>The hierarchy of highest to lowest<h3>
<ul>
<li>Inline Styles</li>
<li>ID Selectors</li>
<li>Classes, Attributes, and Pseudo Classes</li>
<li>Elements and Pseudo Elements</li>
<li>The Last Rule Wins</li>
</ul>
</details>

## Javascript

- What is the difference between npm and npx?
- What is the difference between package.json and package-lock.json?
- What is the meaning of asynchronous programming?

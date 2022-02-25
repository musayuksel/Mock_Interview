# General

## HTML / CSS

<br>
<details>
<summary>What is the meaning of semantic HTML?</summary>
 Semantic markup isn't about performance, it's about meaning.
 In HTML, for example, the h1 element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."
 <ul>
 <li>Search engines will consider its contents as important keywords to influence the page's search rankings</li>
 <li>Screen readers can use it as a signpost to help visually impaired users navigate a page</li>
 <li>
Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes</li>
 <li>Suggests to the developer the type of data that will be populated</li>
 <li>Semantic naming mirrors proper custom element/component naming</li>
 </ul>
</details>
<br>
<details>
<summary>Which elements in HTML are non-semantic? And why do we need them?</summary>
block: div
inline: span
They don’t tell anything about the content they contain. They can be used with different attributes to mark up semantics common to a group.
</details>
<br>
<details>
<summary>What is the meaning of accessibility?</summary>
Accessibility is the practice of making your websites usable by <strong> as many people as possible.</strong> We traditionally think of this as being about people with disabilities, but the practice of making sites accessible also benefits other groups such as those using mobile devices, or those with slow network connections.
</details>
<br>
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
<hr>

## Javascript

<br>
<details>
<summary>What is the difference between npm and npx?
</summary>
</details>
<br>
<details>
<summary>What is the difference between package.json and package-lock.json? </summary>
<strong>package.json</strong> is a file that contains information about your project (name, version, etc) and it lists the packages that your project is dependent on.
When you install any package in your project it will install the exact latest version of that package in your project and save the dependency in package.json with a carat (^) sign. etc ^ 5.2.3 <br>
5=MAJOR; incompatible API changes are made.<br>
2=MINOR;  It's safe to update to a new minor version without requiring code changes.<br>
3=PATCH;  bug fixes<br>
Carat (^) means it will support any higher version with major version 5 like 5.3.1 and so on. Here, package-lock.json is created for locking the dependency with the installed version.
</details>
<br>
<details>
<summary>What is the meaning of asynchronous programming?</summary>
In general JavaScript is running code in a non-blocking way. This means that code which is is taking some time to finish (like accessing an API, reading content from the local file system etc.) is being executed in the background and in parallel the code execution is <br> 
<code>
const getTodo = () => {
    setTimeout(() => {
        return { text: 'Complete Code Example' }
    }, 2000)
}<br>
const todo = getTodo()
console.log(todo.text)
</code>
<br><mark>How can we deal with it?</mark><br>
<code>
const getTodo = callback => {
    setTimeout(() => {
       callback ({ text: 'Complete Code Example' })
    }, 2000)
}<br>
getTodo(todo => {
    console.log(todo.text)
})
console.log("This is the first output")
</code><br>
<mark>There are 3 ways you can solve</mark>
<ul>
<li>Callbacks</li>
<li>Promises</li>
<li>Async/Await</li>
</ul>
</details>

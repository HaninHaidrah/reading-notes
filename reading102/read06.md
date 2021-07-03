# The Summury
## Table of  Content
1. *What is CSS*
2. *CSS Selectors*
3. *CSS Syntax*


###  CSS
CSS (Cascading Style Sheets) allows you to create great-looking web pages, but how does it work under the hood? This article explains what CSS is, with a simple syntax example, and also covers some key terms about the language.
documents in *HTML* will be readable in a web browser. Headings will look larger than regular text, paragraphs break onto a new line and have space between them. Links are colored and underlined to distinguish them from the rest of the text

### CSS syntax
CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large red text."

The following code shows a very simple CSS rule that would achieve the styling described above:


 ![logo](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/CSS3_logo_and_wordmark.svg/1200px-CSS3_logo_and_wordmark.svg.png)

> h1 {
    color: red;
    font-size: 5em;
}

### CSS Selectors
1. tags
2. class
3. id
> The id is the most important selector <

### Three Ways to Insert CSS
There are three ways of inserting a style sheet:

* External CSS
    * With an external style sheet, you can change the look of an entire website by changing just one file!
    An external style sheet can be written in any text editor, and must be saved with a .css extension.




* Internal CSS
    * An internal style sheet may be used if one single HTML page has a unique style.

    The internal style is defined inside the <style> element, inside the head section.
* Inline CSS
    * An inline style may be used to apply a unique style for a single element.

    To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.
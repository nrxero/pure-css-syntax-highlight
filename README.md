# pure-css-syntax-hightlight
A pure CSS HTML syntax highlighter

Import the CSS file to start:
```html
  <link rel="stylesheet" href="./syntax.css">
```

Use HTML classes to hightlight elements. Start with the "syntaxbox" code element class.

## Classes:

<table>
  <tr><th>Class</th>
  <th>Usage</th></tr>
  
  <tr>
    <td>syntaxbox</td>
    <td>Use on a "code" element. This is the wrapper for everything</td>
  <tr>
  <tr>
    <td>identifier</td>
    <td>Use on a "span" element. Creates an HTML element identifier.</td>
  <tr>
  <tr>
    <td>identifier end</td>
    <td>Writes a /end identifier element</td>
  <tr>
  <tr>
    <td>value</td>
    <td>Creates a value. Position after an attribute span.</td>
  <tr>
  <tr>
    <td>value link</td>
    <td>Creates a link value. Position after an attribute span.</td>
  <tr>
  <tr>
    <td>attribute</td>
    <td>Creates an HTML attribute. Put this span inside an identifier span.</td>
  <tr>
  <tr>
    <td>newline</td>
    <td>A "span" element. Creates a new line. Enclose each line of elements within it.</td>
  <tr>
  <tr>
    <td>comment</td>
    <td>A "span" element. Put the comment text within it.</td>
  <tr>
    
</table>
  
## Example:

![syntax example](https://user-images.githubusercontent.com/62193848/163313767-1e08799d-2e29-4119-8c41-b2cf907c119c.PNG)

```html
<code class="syntaxbox">

  <span class="newline"><span class="comment">Add the "link" class to value hightlights the link</span></span>
  <span class="newline"><span class="identifier">a<span class="attribute">href</span><span class="value link">https://github.com/nrxero/pure-css-syntax-hightlight</span></span>Github<span class="identifier end">a</span></span>
  <span class="newline"></span>


  <span class="newline"><span class="comment">Textbox syntax</span></span>

  <span class="newline"><span class="identifier">input<span class="attribute">type</span><span class="value">text</span></span><span class="identifier end">input</span></span>

  <span class="newline"></span>

  <span class="newline"><span class="comment">Syntax for the above element</span></span>

  <span class="newline"></span>


  <span class="newline"><span class="identifier">span<span class="attribute">class</span><span class="value">newline</span></span></span>

  <span class="newline" data-level='1'>
    <span class="identifier">span<span class="attribute">class</span><span class="value">identifier</span></span><span class="identifier">span<span class="attribute">class</span><span class="value">attribute</span></span>type<span
      class="identifier end">span</span><span class="identifier">span<span class="attribute">class</span><span class="value">value</span></span>text<span class="identifier end">span</span><span class="identifier end">span</span></span>

  <span class="newline" data-level='1'>

    <span class="identifier">span<span class="attribute">class</span><span class="value">identifier end</span></span><span class="identifier end">span</span>


  </span>

  <span class="newline"><span class="identifier end">span</span></span>

</code>
```

# Attributes of an element - Classes

Technically, you could use those attribute methods we saw (`getAttribute`, `setAttribute`, `hasAttribute`) to work with an element's classes.

However, the classList property offers a better approach. It's an object with the following methods pertaining to classes:


```add(className, className, ...)
remove(className, className, ...)
toggle(className)
contains(className)
replace(oldClass, newClass)
```
```
document.querySelector("h1").classList.add("class", "header");
```

# Selecting multiple elements
Before we checkout selecting multiple elements, let's add the following HTML below the existing <p> element:

```
<ul id="comments">
  <li class="comment">first comment</li>
  <li class="comment">second comment</li>
  <li class="comment">third comment</li>
</ul>
```

VS Code includes Emmet, which is a great tool for quickly generating markup. Type the following to generate most of the markup above: `ul#comments>li.comment{comment}*3`

The following methods can be used to select multiple elements:

`getElementsByTagName(namesString)`

`getElementsByClassName(namesString)`

The above methods return a live HTMLCollection.

Although it's pretty cool that the returned list is automatically updated to include/exclude DOM elements as the DOM is updated, the above methods are not as flexible as the `querySelectorAll` method...

Like `querySelector`, the `querySelectorAll(selector)` method uses the power of CSS3 selectors to specify which DOM elements we want returned. Of course, like the name says, it selects all DOM elements that match the selector. By itself, `querySelectorAll` actually provides all the DOM selection power a web dev needs!

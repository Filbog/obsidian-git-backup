15-11-2024

Using hx-trigger attribute. We can have multiple event triggers on one element. It has multiple modifiers etc, good to look up docs to unleash its full power. In the *Hypermedia* book, we have example of making the keyboard shortcut work as an event trigger:

```
<div id="main">

  <button hx-get="/contacts" hx-target="#main" hx-swap="outerHTML"
    hx-trigger="click, keyup[ctrlKey && key == 'l'] from:body"> <1>
    Get The Contacts
  </button>

</div>
```
the "from:body" makes it so that the whole body listens to the keyboard shortcut, not only when the button is focused (using the **event bubbling**)


### Hashtags:
#webdev #coding #htmx 

### References (source material, similar notes):
https://hypermedia.systems/extending-html-as-hypermedia/
[[Event bubbling in DOM]]
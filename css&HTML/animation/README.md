# The four principles


The WCAG are organized around four, core principles (POUR) that should be kept in mind when implementing any sort of accessibility feature:

1. **Perceivable**: Users must be able to perceive the information or user interfaces being presented. For example, light text on a light background could be difficult for some users with a visual impairment to perceive.

2. **Operable**: Users must be able to operate any user interfaces or navigation, and interfaces cannot require an interaction which the user cannot perform. A navigation bar with drop-down menus that only expand when a mouse cursor hovers over them, for example, would not be operable by keyboard users giving those menu items focus.

3. **Understandable**: Users must be able to understand any information or user interface that is presented to them. For example, if a user tried submitting a form and received an error such as “Error 113: Bad data”, they wouldn’t be able to understand what the error actually means or how to fix whatever caused the error.

4. **Robust**: Content must be accessible by current assistive technologies and other user agents, and must remain accessible as those technologies advance.

```
<aside>
<footer>
<form>
<header>
<main>
<nav>
<section>
```


# responsive design

1. The viewport meta tag

```
    <meta name="viewport" content="width=device-width, initial-scale=1">
```
2. **Avoid fixed width and height**
3. **Avoid heights all together**
In most cases, you should avoid setting a height altogether. There are some exceptions to this rule (headers and footers perhaps)
4. *When fixed widths are appropriate*
Obviously there are cases when a fixed width is appropriate. It’s hard to make a universal rule, but in general the smaller your widths the more likely it’s fine to make them fixed. For example, a 32px icon on your page isn’t going to benefit from using max-width because you probably don’t want it to shrink. Likewise a 250px sidebar probably needs to always be 250px
5. **Use flex and grid**
Here’s a statement so obvious that it sounds like a joke: flexbox was created to enable the creation of flexible layouts. Simply using flex and grid doesn’t necessarily guarantee perfect responsiveness, but they are really helpful tools. You’ve already learned about the relevant properties here, but things like flex-wrap and grid’s minmax, auto-fill and similar properties can make some impressively responsive layouts without much extra work.

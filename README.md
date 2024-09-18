# Style Guide

Formatting of Bot development guides is now normalized across the board, this will allow us to have a consistent presentation across the website and we will also be able to let a creator know to fix stuff in their guide if their formatting does not exactly make our life easy.
---
## Format Tags

We will be using the following tags to format, in rare instances we'd use other formatting if required:

```<h1>This is a Title</h1>, <h3>This is a sub-title</h3>, <p>Your average text</p>```

Those three tags will be our bread and butter, a less used one might be ```<pre>``` Which is a pre-formatted tag, in very difficult guide structures we might use this but it limits the amount of styling we can apply to a certain degree and the formatting in there is absolute, meaning you cannot put a Header inside of a Pre-Formatted tag.

Example uses:

```<h1>The Scenario</h1>``` - Titles, etc should use H1

```<h3>Writing Scenarios</h3>``` - Subtitles, Say you have "The Scenario" and within that part of the guide you have multiple different points the creator touches, each point starts with it's own sub-title, that's where H3 comes in.

```<p>Lorem Ipsum</p>``` - Your everyday text, nothing special, just text that is NOT a title xD.
---
## Advanced Formatting

If you're feeling fancy and want to do the entire formatting, I have the guide for that as well! Though this one's a LITTLE bit more complicated due to the nature of HTML.

Let's start with a short explanation of how the guide format works using a real HTML setup:

```html
<div class="guideBox">
    <H1>Guide Title</H1>
    <div class="plainTextBox">
        <h1>Section Title</h1>
        <H3>Subtitle 1</H3>
        <P>Lorem Ipsum dolor sit amet</P>
    </div>
    <div class="botCodeBox">
        <P>Any Bot code and ONLY BOT CODE</P>
    </div>
</div>
```

This is the most BASIC of setups, the bigger the guide the bigger this will get and the more complex the setup, some guides will most certainly require multiple <div> tags inside of <div> tags, etc. 

But generally that is it. 

### How it works?
*I'm glad you asked*

```guideBox``` is the class that encompasses the entire guide, everything inside of there is THE guide, the entire thing. It's for all intents and purposes the box that holds it all together and allows for quick movement if I need to move shit around.

```plainTextBox``` I mean... it's plain text, not code, not script, just the plain text part of the guide, like how I'm writing now.

```botCodeBox``` This class is ONLY for the bot's code. If there are any comments for the code WITHIN it, that also counts as bot code in this instance.
# Accessibility Assessment

## Overview

This project was to take a page about bears with accessibility issues and resolve a number of them.

To run the project, download the files and run with a locally hosted live server.  I used the Live Preview extension of Visual Studio to run it.

## Accessibility Lab Answers

- Color
    I ran a contrast test using WebAIM's extension WAVE.  It found 19 errors in the page when it comes to color contrast stemming from the light background with light page title and the dark backgrounds with dark headers and text.  I solved this by changing the lighter background color to be dark and darker background color to be light.
- Semantic HTML
    1. When you navigate with a keyboard you skip straight from the search all the way down to the audio player.  You then tab through each part of the audio player.  Eventually you loop back up to the related links.
    2. Yes, by adding proper elements.  Screen-readers are built to understand and associate some elements together in context.  By making sure we use the appropriate elements we can provide users of screen-readers with a better user experience.  If for whatever reason we are unable to use these elements, we need to add in aria labels to provide the context for the screen-readers manually.
    3. It should be in a <nav> element instead of being labeled as one.
- The Images
    Yes we can add alt descriptors to the <img> elements to make them accessible for screen-readers.
- The Audio
    1. We can add a transcript of the audio.
    2. We can add a hyperlink element to direct to the mp3 itself instead of the audio player.
- The Forms
    1. We can add an aria-label to it.
    2. We achieve it by adding a label element and using the 'for' property to associate it with the name of the input element that it is a label for.
- The Show/Hide Comment Control
    We make the div a role of button, give it a tab index value and add some code to our script to listen for keydown events from the enter key on the document.  We then fire off the selected element's click event.
- The Table
    Yes, we can add th elements and utilize their scope attribute to provide context for a screen-reader and we can include either a summary or caption of the table.
- Other considerations
    1. As nice as the cursive titles and headers look, they could be hard to read for some populations.  It would be better to use a simpler font with higher readability.
    2. While this isn't a particularly large page, it could still be nice to add on page navigation to jump to the different sections.  This would have the potential to make navigation of the page easier for screen-reader users.

## Sources and Credits

- HTML: A good basis for accessibility: https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML
- WAI-ARIA basics: https://developer.mozilla.org/en-US/docs/Learn/Accessibility/WAI-ARIA_basics
- Accessible multimedia: https://developer.mozilla.org/en-US/docs/Learn/Accessibility/Multimedia

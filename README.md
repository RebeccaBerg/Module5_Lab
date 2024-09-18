# Web Dev Starter Code

## Overview

TODO: Write a project description

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
    1. 
    2. We can add a hyperlink element to direct to the mp3 itself instead of the audio player.

## Sources and Credits

TODO: You must credit the sources and authors of any code, libraries, or other
assets you use in your project. If you leave this section blank, your project
will be considered in violation of the Academic Honesty policy unless you truly
created everything from scratch with no outside help. If you need to use a
source that you cannot credit (e.g. a classmate's work), you must get explicit
permission from your instructor.

A simple bulleted list below is sufficient. For example:

- Bootstrap: https://getbootstrap.com/
- jQuery: https://jquery.com/
- Background image: https://unsplash.com/photos/...
- Sound effects: https://freesound.org/people/...
- Icons: https://fontawesome.com/
- Fonts: https://fonts.google.com/
- etc.

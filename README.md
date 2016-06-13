# legendary-telegram

I'm learning JavaScript and so obviously I've set myself a rather daunting task. Because the simple version would be "too easy" or something. :eyeroll:

The idea is that this will become a choose-your-own-adventure kind of deal, using JS (and jQuery) to navigate the different story blocks. I've done a little just on text editors offline, but I wanted to pull it onto GitHub so I could try different branches, etc.

---
6/4/16 1:37pm
TimeSpace GameBook part 1:

Okay. So Codecademy has this “final project” for their JS track that is making a simple choose-your-own-adventure program, largely using prompt boxes. Only I don’t really want to use the prompt boxes. Because they’re not pretty. I would rather do everything within a web page. And of course I want to make a story that’s significantly more complicated than I think the project is expecting. Because *points at self* writer.

So I want to look into the possibility of formatting the pop-up windows, but what I’m likely to do instead is use buttons or form inputs to progress the story, and basically append on the new narrative/question/button(or)input to the end of the page, while also hiding whatever buttons or input were leftover from the last question. Obviously I don’t want to write a new long line of code every time there’s a new story block, so I’m going to want to write up a couple of functions where I can just plug in (narrative, question, button1, button2 etc) and a second one for anything that needs an actual input instead of buttons.

I’d like to eventually have it set up so that you can choose from a few different characters and play the story out from different perspectives, but that’s wayyyyyy too much work for now.

I also want to have the ability to loop back around to an earlier choice without loosing the narrative on the screen of what’s happened so far, which is why I don’t really want to go with the un-hiding already-written divs in the html.

Oh, also I thought it might be fun to change the background to red-tinted when big things happen. idk.

4:01pm
I think I have the button function set up. (After a few hours of work! Because I don’t know what I’m doing! I still don’t understand how to use mutliple js files at once.....) Now I’m going to set up the input function, which I believe will be a little quicker now that I know what I’m doing with the buttons.


---
6/6/16  1:39pm
I’m going through a different course (on Udacity) that’s actually doing a better job explaining the linked js file hierarchy, so hopefully I can use some of this knowledge to streamline this gamebook deal.

In the resume building js hierarchy, the links are ordered as follows: After the css, the html links to “jQuery.js” (which is LONG and I don’t think I understand all of what it’s doing yet), then the “helper.js” (this holds a lot of variables containing lines of html that can be altered and put into the html doc later, and also more js and jQuery code that seems to relate directly to the content of the page). After that is a map script, and then the body of the html. After all the divs (but before the closing body tag) is a link to “resumeBuilder.js” (which alters the variables in “helper.js” as needed, and appends them to the page), and then a script tag for javascript, which hides various elements if they’re empty.

AT LAST SOMEONE EXPLAINS THE HIERARCHY! Now I can figure out how to implement that to this gamebook project.

I may write up a short version of a CYOA (say, 3-4 story blocks, 2-3 different endings?) just to get the hang of it, before writing up the long version.

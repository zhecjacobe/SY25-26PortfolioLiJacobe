Step 1 (Static vs Relative):

    Add in css position: relative; top: 20px; left: 20px; to .sidebar.

    Guided Question: What changed compared to the default static positioning? Try to give different values to top and left or you can change it to bottom, right.

*Answer: The position of the sidebar turned relative and was offset by 20 pixels from the top and the left from where it would be if it was static.*

Step 2 (Fixed):

    Add in css position: fixed; bottom: 0; width: 100%; to .footer.

    Guided Question: What happens when you scroll the page? Why does the footer behave differently from position relative?

*Answer: The position of the footer follows you when you scroll and it behaves differently because the position is fixed to the bottom.*

Step 3 (Absolute):

    Add in css position: absolute; top: 66px; left: 200px; to .content.

    Guided Question: What is the effect of position: absolute on an element? How is it different from fixed?

*Answer: The position absolute affects an element by moving/formatting it to a previously formatted element. It is different from a fixed element as they would have different reference points. Absolute wold be fixed to a previous element while fixed would be fixed to the entire webpage.*

Step 4 : (Absolute)

    Add in html <div class="notice">Notice!</div> and include the css below:

.notice {
    position: absolute;
    top: 60px;
    left: 400px;
    background: orange;
    padding: 10px;
    z-index: 2;
}

    Give .content a z-index: 1.

    Guided Question: Why does the notice appear on top of the content? What happens if you swap the z‑index values?

*Answer: The notice appears on top if the content because it has a higher z-index value. If we swap the z-index values, the content will now appear in front of the notice as .content has a higher z-index value which means it will be the layer on top of .notice.*

    Challenge:
        What changes that you have to do on the code that will position .notice box on the top right corner of the .content box? 
*Answer: I could make its position absolute to the .content box and set it to top: 65px; and left: 430px.*
The code would be

    .content {
      background: lightyellow;
      width: 300px;
      height: 200px;
      position: absolute; 
      top: 66px; 
      left: 200px;
      z-index: 2;
    }    

    .notice {
    position: absolute;
    top: 65px;
    left: 430px;
    background: orange;
    padding: 10px;
    z-index: 3;
    }

Try to change the position of .content to relative then to fixed. What do you observed each time?

Answer: The notice doesn't stay at the top right corner anymore..

 What do you observe on about the effect of z-index on .notice and .content boxes?

 Answer: Changing the values changes the layers which means whichever has the higher value will be on top.

    Please answer the following reflection questions (15 minutes)

    a. Could you summarize the differences between the CSS position values (static, relative, absolute, fixed)?

    Answer: Static is the normal position, relative is when you offset it to the static position, absolute is when you adjust it to the position of the parent ancestor, fixed is when it stays fixed when you scroll.

    b. How does absolute positioning depend on its parent element?

    Answer: It needs an element because without it just becomes relative.

    c. How do you differentiate sticky from fixed (you can research on sticky)?

    Answer: Sticky means that once it hits a border it stas fixed at that position.

    d. If you were designing a webpage for a school event, how might you use positioning to highlight important information? Please give concrete examples.

    Answer: I would use the positionings to make sidebars or pop ups.

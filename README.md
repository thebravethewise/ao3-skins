# ao3-skins

Hiding Works

Hides works that include ships involving  Brendon “The Park” Shark

.blurb:has(a.tag[href*=”*s*Brendon%20%22The%20Park%22%20Shark"]) {
  display: none !important;
}
.blurb:has(a.tag[href*=”Brendon%20%22The%20Park%22%20Shark*s*"]) {
  display: none !important;
}

Hides works containing the  Suicide Attempt  tag

.blurb:has(a[href*="/tags/Suicide%20Attempt/works"]) {
  display: none !important;
}

Hides works that have a tag containing  “drinking”

.blurb:has(a.tag[href*="drinking"]) {
  display: none !important;
}
You can also make this have case sensitivity by adding  i  after the quotes

.blurb:has(a.tag[href*=”Drinking” i ]) {
  display: none !important;
}




Customization :P

If you are combining this with another skin add  !important  to the end of every line (before the semi-colon) so that it will override the other code

this will make any tag containing  “lesbian”  have a flag gradient towards the right, make the text color black, give it a white border with a curved corners, and add 2px of padding to the sides

a.tag[href*="Lesbian"] {
  background: linear-gradient(to right, #d62800, #ff9b56, #ffffff, #d462a6, #a40062);
  color: black;
  border-radius: 4px;
  border: 1px solid white;
  padding: 0px 2px;
}

Makes the specific  Friends to Lovers  tag green

a[href*="/tags/Friends%20to%20Lovers/works"] {
  background: green;
}

This can also be used to customize the entire blurb/box of a fic

Makes the background of the fic blurb red if it contains the  AI-Generated Content  tag

.blurb:has(a[href*="/tags/AI-Generated%20Content/works"]) {
  background: #ff0000;
}

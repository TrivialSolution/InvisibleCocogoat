# InvisibleCocogoat
Like Find the Invisible Cow, but Cocogoat.

Inspired by: https://findtheinvisiblecow.com/
Based on the "Cocogoat" joke explained here: https://tvtropes.org/pmwiki/pmwiki.php/Memes/GenshinImpact
I wanted "Cocogoat" to reflect the energy here: https://www.youtube.com/watch?v=8VABEN3mUcM, but I think I failed.

Unlike invisible cow which plays different sound files based on cursor distance from the cow,
this game plays a single file with varying volume and L-R pan depending on position relative to the cocogoat.

The image of Ganyu is covered by a blank div "cover" because:
- click events on hidden elements don't work
- opacity 0 images can be interacted with in unexpected ways.

In other words, an additional element z-indexed on top of the image was required. 
Or I could have simply made the image not even exist and only added the content when the mouse was clicked at certain coordinates,
but this way is easier to debug. I'm not terribly concerned about people using debug tools to cheat, given there's an instant win button.

The whole thing is one HTML file for no particular reason. Maybe a bit easier for the network this way since the individual JS and CSS files would be small?

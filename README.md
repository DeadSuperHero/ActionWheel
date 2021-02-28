# ActionWheel
ActionWheel is an open source game template for Adventure Game Studio. The goal
of this design project is three things:

1. **Visual Simplicity** - in point-and-click adventure games, it's sometimes easy
to end up in a situation where the game UI elements take up way too much space.
Worse yet, sometimes there's a significant amount of distance between the
 _thing you want to click_ (a verb icon, like "Use") and a _the thing you need to
 click afterwards_ (an object, like a lever)

 ActionWheel attempts to solve this problem by putting everything you need in
 one place, at the shortest possible distance from where you clicked. The idea
 is similar to VerbCoin by LucasArts, which was used in some of their most
 popular games. However, the design is also highly influenced by the Sierra
 Creative Interpreter, courtesy of Sierra On-Line. My design intention was to
 put both systems together into something new.

 2. **Context-Driven Indication** - ActionWheel uses several different kinds of
 labels to indicate to players certain kinds of context:

 * Cursor Label - A hovering label next to the mouse pointer appears when
 all interfaces are closed, showing Characters, Hotspots, and Objects in a given
 room. This easily shows to players what things in an environment can be
 interacted with.
 * Wheel Label - The Wheel Label clearly explains the buttons on the wheel.
 Additionally, the label will contextually update for certain kinds of
 properties - for example, the "Use" icon can change to "Pick Up" or "Touch" to
 indicate what kind of action is available for that button.
 * Inventory Label - Finally, the inventory window shows what icon is currently
 under the mouse.

 3. **Integration of Elements** - ActionWheel aims to design a new kind of
 point-and-click interface that incorporates traditional pop-up windows into
 a stationary cursor area, based on where the player clicks. Similar to the first
 principle, the intention is to keep the most important, most-accessed functions
 within immediate reach for the player. In addition, this particular design is
 intended to be friendly to both traditional desktop inputs, as well as mobile
 tablets.

 ## Current Status
 A very basic demo game has been put together with a 1.0 release of the GUI's
 functions. Although the code is a little ugly and a little hacky, it works well
 enough to release as a template.

 There are a few future goals that I want to explore for the project:
 * **Custom Dialog Rendering** - I'd love to figure out how to incorporate
 custom dialog buttons with icons into the UI. This is somewhat harder, and
 requires the use of dynamic sprites, but it's 100% possible that speech options
 could also be factored into the UI somehow.
 * **Tablet Optimization** - I have a few ideas on how AGS might be optimized
 for touch interfaces, and want to experiment with them in the near future. The
 biggest two things are: representing touch inputs to an engine designed around
 mouse clicks, and visually showing to players exactly where fingers are positioned
 using the AGS Camera API.

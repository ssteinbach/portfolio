# Completed Games

*Click the thumbnail to play online!*

## Quadplay

### [Beat the Gobblins](https://stephan-gfx.itch.io/beat-the-gobblins)

|[![BEAT THE GOBBLINS](https://img.itch.zone/aW1hZ2UvNTY0MTkyLzI5NjMzMjUuZ2lm/794x1000/JhQtF5.gif)](https://stephan-gfx.itch.io/beat-the-gobblins)|
|-------------------------------|
|[Post Mortem](https://docs.google.com/document/d/1Z8iBf_VUf_26AmKrWBJ9THso-UCqWl5NsIOpnSF9-1s/edit#)|
|2/15/2020|
|Started as a jam game w/ Ed Luong, features awesome music by Marlena Fecho.|
|[Source](https://github.com/morgan3d/quadplay/tree/master/games/beat_the_gobblins)|

### [Across The Lake](https://stephan-gfx.itch.io/across-the-lake)

|[![Across The Lake](https://img.itch.zone/aW1hZ2UvNjE2MDMwLzMyOTA3NTQuZ2lm/347x500/O%2F6yeI.gif)](https://stephan-gfx.itch.io/across-the-lake)|
|-----------------|
|[Post Mortem](https://stephan-gfx.itch.io/across-the-lake/devlog/141410/ludum-dare-46-post-mortem-across-the-lake)|
|4/20/2020|
|Ludum Dare game jam game for LD46, finished 27th overall and 12th in mood (out of 3576 submissions).  Theme was "Keep it Alive"| 
|[Source](https://github.com/morgan3d/quadplay/tree/master/games/across_the_lake)|

## Pico8

Pico8 projects done either in collaboration w/ Steve Lavieties or based on
co-developed basecode.

|Picotris Attack|Pentomino|Pushback|Dead Man's Slope|Pico De Pon|
|-----|----|----|----|----|
|[![Picotris Attack](https://www.lexaloffle.com/bbs/thumbs/pico37969.png)](https://www.lexaloffle.com/bbs/?tid=2925)|[![Pentomino](https://www.lexaloffle.com/bbs/thumbs/pico37638.png)](https://www.lexaloffle.com/bbs/?tid=28815)|[![Pushback](https://www.lexaloffle.com/bbs/thumbs/pico40479.png)](https://www.lexaloffle.com/bbs/?tid=29285)|[![Dead Man's Slope](https://www.lexaloffle.com/bbs/thumbs/pico46800.png)](https://www.lexaloffle.com/bbs/?tid=30307)|[![Pico De Pon](https://www.lexaloffle.com/bbs/thumbs/pico8_picodepon-2.png)](https://www.lexaloffle.com/bbs/?tid=37280)|
|12/21/2015|2/12/2017|5/7/2017|11/29/2017|04/07/2020|
|Based on Tetris Attack, first shipped project in pico8.|Done right before GDC in 2017|Attempt at a small game done quickly, wanted to try and do something that wasn't an adaptation.|Started while snowed in one winter and thinking back on ski free (although plays nothing like that game).|Steve and I returned to Tetris Attack after having worked on a megadrive version, as an homage to the awesome pico8 community.  Features music by tesselode and art from a variety of great games from the pico8 community that inspired us!|
|[Source](https://github.com/stevelavietes/pico8carts/blob/master/picotrisattack.p8)|[Source](https://github.com/stevelavietes/pico8carts/blob/master/pentomino.p8)|[Source](https://github.com/stevelavietes/pico8carts/blob/master/mazeburger.p8)|[Source](https://github.com/stevelavietes/pico8carts/blob/master/pushback.p8)|[Source](https://github.com/stevelavietes/pico8carts/blob/master/dead_mans_slope.p8)|[Source](https://github.com/stevelavietes/pico8carts/blob/master/picodepon.p8)|

# Tests/Demos/Utilties/Examples/Other

## Tests (Quadplay)

|[Acceleration Demo](https://morgan3d.github.io/quadplay/console/quadplay.html?game=examples/accel_demo)|[Bounce Demo](https://morgan3d.github.io/quadplay/console/quadplay.html?game=examples/sproing)|[Camera Shake](https://morgan3d.github.io/quadplay/console/quadplay.html?game=examples/camera_shake)|[Transition/Sequence](https://morgan3d.github.io/quadplay/console/quadplay.html?game=examples/sequence_demo)|
|----|----|----|----|
|![Acceleration Demo](img/Acceleration_Library_Demo_2020-08-19_21h03.gif)|![Bounce Demo](img/Squash_and_Stretch_Example_2020-12-06_20h12.gif)|![Camera Shake](img/camera_shake_2020-07-05_14h21.gif)|![Transition/Sequence](img/Reach_2020-06-20_09h26.gif)|
|While struggling with Beat the Gobblins, I stumbled across a GMTK video about [celeste's game feel](https://www.youtube.com/watch?v=yorTG9at90g&vl=en), and after seeing the graphs I  realized I could model those accelerations really simply using an ADSR model inspired by Steve Swink's [Game Feel](http://www.game-feel.com) book.  This test proved to be super useful, and I've cleaned it up into a very simple module I've since used on a number of projects.  Its driven off just three parameters: acceleration time from 0 to full speed (in frames), deceleration time from full speed to 0 under no acceleration (in frames) and maximum speed (in px/f).  You can see the table [here](https://github.com/morgan3d/quadplay/blob/2bc3f95cc5ce6960b6071d82b494b65428fb9ffd/examples/accel_demo/accel_lib.pyxl#L90) and further explanation [here](https://github.com/morgan3d/quadplay/blob/2bc3f95cc5ce6960b6071d82b494b65428fb9ffd/examples/accel_demo/accel_lib.pyxl#L1).|The bounce demo is based on @fourbitfriday's bounce demo from [a stream](https://www.twitch.tv/videos/576377070).  Again, it is built into an easy to integrate library and features a similar "profile" system as the acceleration library.|Every game needs camera shake!  This is a library for doing a simple nuclear throne/[vlambeer](https://www.youtube.com/watch?v=AJdEqssNZ-U) inspired screen shake that restores|A simple turn transition library that also serves as a nice demo for using quadplay's `sequence` feature.|
| [Source](https://github.com/morgan3d/quadplay/tree/master/examples/accel_demo)|[Source](https://github.com/morgan3d/quadplay/tree/master/examples/sproing)|[Source](https://github.com/morgan3d/quadplay/tree/master/examples/camera_shake)|[Source](https://github.com/morgan3d/quadplay/tree/master/examples/sequence_demo)|

## Pico8

* Stdlib (basecode for our projects):
    * [Source](https://github.com/ssteinbach/pico8carts/blob/master/stdlib.p8)

|One Euro Filter|Performance Tests|Easing Function Gallery|
|-----|----|----|
|[![One Euro Filter](https://www.lexaloffle.com/bbs/thumbs/pico42459.png)](https://www.lexaloffle.com/bbs/?tid=29646)|[![Performance Tests](https://www.lexaloffle.com/bbs/thumbs/pico44897.png)](https://www.lexaloffle.com/bbs/?tid=30032)|[![Easing Function Gallery](https://www.lexaloffle.com/bbs/thumbs/pico44294.png)](https://www.lexaloffle.com/bbs/?pid=41657&tid=29488)|
|07/14/2017|10/4/2017|09/18/2017|
|[Source](https://github.com/stevelavietes/pico8carts/blob/master/one_euro_filter.p8)|[Source](https://github.com/stevelavietes/pico8carts/blob/master/performance_test_gallery.p8)|[Source](https://github.com/stevelavietes/pico8carts/blob/master/easing_gallery.p8)|

## Tweet Carts

|Conway's Game Of Life Tweet cart|
|--------------------------------|
|[![Conway's Game of Life](https://img.itch.zone/aW1nLzIxMjQ0MTkuZ2lm/315x250%23cm/41ASDq.gif)](https://stephan-gfx.itch.io/conways-game-of-life)|
|5/19/2019|
|Done as an intro/invitation cart for an Alife interest group meet up|

# Unfinished Prototypes

|Space flight FX test|"Reach"|"Into the Pitch"|
|----|----|----|
|![Flying Around](img/PICO-8_31.gif) ![Shootin](img/PICO-8_38.gif)|![Map Movin'](img/reach_production_cost.gif)|![Movin' and Turnin'](img/pitch.gif)|
|Pico8|Quadplay|Quadplay
| |4x-ish|Originally for 7drl|

|Planet Generator|Climbing Violets|Baseball Prototype|
|----|----|----|
|Screen shot of C++ version, click image to see on shadertoy:[![View on Shadertoy](img/in_motion_ufo50.mov)](https://www.shadertoy.com/embed/MlyyzK?gui=true&t=10&paused=true&muted=false)|![Climbin'](img/PICO-8_41.gif) ![Editin'](img/PICO-8_26.gif)|![Swingin'](img/PICO-8_21.gif)|
|C++/GLSL/ISPC|Pico8|Pico8|
|wanted to learn about procedural generation and raymarching.  planet generation algorithm is my interpretation of an algorithm from star control 2.  All of the generation was done offline in C++ and then ported to ISPC.  The rendering is entirely in a GLSL shader.|Had a cool level editor by @stevelavietes| |

|[Word Game](https://morgan3d.github.io/quadplay/console/quadplay.html?game=examples/word_game)|
|-------|
|![Word Game](img/word_game_2020-09-12_16h26.gif)|
|Quadplay|
|This was a test for making a game entirely out of words, looking at how easy it would be for me to add content to a game with such minimal aesthetics.  Links: [Post Mortem](https://docs.google.com/document/d/1pkV4FL_167ArQkXBkH9Njl_4P4Eq3-UYK7MJegNddvA/edit?usp=sharing), [Source](https://github.com/morgan3d/quadplay/tree/master/examples/word_game)|

# Engines Used

* Quadplay (by @casualeffects): [![quadplay✜](https://morgan3d.github.io/quadplay/console/logo-116x20.png)](https://github.com/morgan3d/quadplay)
* Pico8: [![Pico8](https://www.lexaloffle.com/gfx/lexaloffle-pico8.png)](http://www.lexaloffle.com/pico-8.php)


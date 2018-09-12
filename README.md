# UNREAL_TUTORIAL_3

## What I Learned
I learned how to correctly overload a C++ function with Blueprints and use timers effectively.

## Notes
In order to use UTextRenderComponent, you need to have 
#include "Components/TextRenderComponent.h"

However, by doing that, it creates a false positive error with GENTERATE_BODY()
It will compile still, so it’s safe to ignore. Seems adding any lines above UCLASS() creates false positive errors

Seems Intellisense (Visual Studio’s “wonderful” error checking tool) is total bunk. It’s throwing false positives for SetHorizontalAlignment and SetWorldSize for CountdownText, but it still compiles. I did reading and it says that Intellisense is super bad and that it might as well be disabled.

Wow, having comments as the description in the editor is super cool and effortless. Gotta start writing comments in my code again like I should already be doing (^^;

It’s amazing how programmers and non-programmers can work side by side in unreal. By having specific functionality in C++ and enabling it to be used in blueprints, the programmer can create the functionality and the designer can edit when and what happens with blueprints (wish I knew this in team game. I would have picked unreal)

Finally, this tutorial explains how to have a function that can be overridden in a blueprint. Now it makes sense

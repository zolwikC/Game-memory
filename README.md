The program is a memory game written in C# using WPF (Windows Presentation Foundation). The main goal of the game is to find pairs of identical emoji icons. The game tracks the time it takes for the player to find all pairs.

Key elements of the program:
DispatcherTimer:

The timer is used to track the elapsed time since the start of the game.
The timer refreshes every 0.1 seconds and updates the timeTextBlock to display the elapsed time.
SetUpGame:

This function initializes a new game.
A list of emoji is created and shuffled randomly, then assigned to TextBlocks in the mainGrid.
The timer is started, and the tenthsOfSecondsElapsed and matchesFound variables are reset.
TextBlock_MouseDown:

Handles clicks on TextBlocks with emoji.
Checks if two clicked TextBlocks have the same emoji.
If they are the same, hides both and increments the match counter.
If not, reveals both TextBlocks.
TimeTextBlock_MouseDown:

Handles clicks on the timeTextBlock.
If all pairs are found, resets the game.

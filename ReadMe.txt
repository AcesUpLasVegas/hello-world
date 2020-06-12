Found this on Steam support community for The Messenger game. Worked

FIX: Controller not recognized
I spent well over an hour trying to get my controller (the 8BitDo N30 Pro 2) to be recognized in the game and finally found a solution:

1. Download the 64-bit version of the Xbox 360 Controller Emulator from http://www.x360ce.com
2. Extract x360ce_x64.exe to your game folder.
3. Run x360ce_x64.exe. It'll ask to extract xinput1_3.dll. Let it.
4. Configure the application for your controller (i.e. make sure that the buttons are all correct).
5. Press the Save button and then close the application.
6. Rename xinput1_3.dll to xinput1_4.dll. This is the emulator disguised as the XInput library that the game will automatically load. Some games load xinput1_3.dll, but this one loads xinput1_4.dll, so we need to rename it.
7. Run the game.

For some reason, I needed to do this even though my controller is a very new model and supports XInput. Hopefully, if you're encountering the same problem that I was, this will fix it for you.
Last edited by Osprey; Aug 7, 2019 @ 8:22am
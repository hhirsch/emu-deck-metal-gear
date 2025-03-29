# Metal Gear Solid Pressure Sensitive on PCSX2 with Emudeck
The reason for this document is to offer a solution for running Metal Gear 2 and 3 in PCSX2 with Emudeck & Steam Deck ROM Manager with pressure sensitivety.
All I was able to find on the topic were forum threads with instructions that did not work, some that did not even make sense and some where the poster just proclaimed "I fixed it" with no information on how they did it.
## Pressure Modifier Is Not Working In PCSX2
Either the instructions are not good or current Emudeck ships with a broken build. I've tested for two days now and nothing I have tried made the pressure modifier work.
I even reviewed some pull requests and source code for PCSX2. So after all this time I decided to go another route.
One thing I did not try was to set the pressure modifier to an analogue input. I've run out of patience to fiddle with the settings though and the solution I have found works.
## Emulate Pressure-Sensitive Buttons of The DualShock Controller On The Steam Deck In PCSX2
So my solution was to just give up with the pressure modifier completely and I decided to use the analogue output of the **right Trigger** of the SteamDeck instead.
Following steps are required to get this done. In this example I used Metal Gear Solid 2 - Substance. Steps for Metal Gear Solid 3 - Subsistence should be very similar.
- Install Emudeck and Steam Rom Manager and get the game to run. There are plenty good instructions of this relatively easy process so that should be fine without explanation.
- When you added the game to Steam with the Steam Rom Manager and do either of the two:
  - Open the game's controller settings and edit the layout so one of your keys is bound to ESC.
  - Connect a keyboard to the Steam Deck so you can hit the ESC key.
- Start the game.
- Bring up the menu by hitting ESC. It should have entries like **"Resume Game"**, **"Load State"**, **"Save Screenshot"**, **"Change Disc"**, **"Settings"**, **"Close Game"**
- Navigate to the menu entry **"Settings"**.
- Push right on the d-pad until you get to **"Controller Settings"**.
- Navigate to where it says **"Controller Port 1"**.
- Below it you will find a line where it says **"Square"**.
- Select this line. A prompt should appear **"Set Input Binding"**.
- Push the right trigger on the Steam Deck.
- If it worked it should say something like **"SDL-0 RT"** in the line you've just edited.
- Use the d-pad to go up. Save your profile with the "Save Profile" function.
- Close the game.
- Cold start the game. You should now be able to lower your gun again by gently letting go of the right trigger after pulling it.
- You can test if it works for example in the "Alternative Missions" in the "Hold Up" missions.

I try to make these steps as easy to understand as possible but please create a ticket if anything is unclear or if you have alternative ways of getting it to work.

If you want to contribute to this page, please create a ticket or pull request [on github](https://github.com/hhirsch/emu-deck-metal-gear).
This text is licensed under the [Creative Commons Attribution-ShareAlike 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/).

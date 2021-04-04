# bitwig-extensions/.../studiologic

Just a fork for Bitwig and SL Mixface controller users. It contains:

* The sl-mixface.bwextension file needed to enable Bitwig integration for the SL Mixface controller. https://github.com/quimgil/bitwig-extensions-studiologic/raw/main/target/SLMixface.bwextension
  * IMPORTANT! Set the DAW to "REASON" in your controller.
* The two extension source code files found at https://github.com/bitwig/bitwig-extensions/tree/api-13/src/main/java/com/bitwig/extensions/controllers/studiologic (with the minimum customization to run as a standalone extension).
* The little glue needed to build the script from the source code.

## What works

Bitwig support in the SL Mixface controller has a DAW mode and a device mode. The loop button is used to switch between these modes.

The transport buttons (REW, FWD, Play/Stop, and REC) and the master volume work in both modes as you would expect. You can use the big knob to move through tracks. You can play and pause by pressing the big knob.

In DAW mode, the eight first tracks are assigned to the eight knobs, faders and buttons. The Select button is active by default, and you can use it to select a specific track. You can press the Rec, Mute or Solo buttons, and use the button of each track to arm, mute, solo the selected track. If you have more than eight tracks, you can use the bank right/left buttons to navigate through all the tracks.

In device mode, the knobs are assigned to the remote controls, and you can use the bank left/right buttons to navigate between remote control pages. Any customization you have done to the remote pages will just work.

The DAW|CTRL button works as expected. However, you might have no reason to use the CTRL mode (Mixface' s official device mode) unless you have a studiologic keyboard that you want to configure, or you miss the colorful lights (in DAW mode the buttons have only white light).

All in all this controller script is pretty complete and well integrated!

# Room for improvement

The three markers buttons are not assigned to any function. Any suggestions about how could they be used? Maybe use the marker left/right buttons to navigate between scenes, and the marker button to record or play the specific scene where the cursor is in?

Something you might miss is a quick double push of the Play button (and the big knob) to make a full stop and bring the transport to the start of the track. The current behavior only supports pause as far as I can see.

## Feedback

Any thoughts? Share them at

* https://www.kvraudio.com/forum/viewtopic.php?f=268&t=562654
* https://www.reddit.com/r/Bitwig/comments/mjh5r1/unofficial_but_very_complete_bitwig_support_for/

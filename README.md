# BUTT

## Fork notes

This is a fork by ken restivo (ken at restivo dot org) of a project that appears to have been abandoned.

Original README follows.

About:
------
butt (broadcast using this tool) is an easy to use, multi OS streaming tool.
It supports ShoutCast and IceCast.
butt runs on Linux, MacOS and Windows.

If you find any bugs or if butt doesn't behave like you expect, please contact me: butt at danielnoethen dot de

Intro:
------
When you start butt the first time, it will create a default config in your home directory.
In order to connect to server, you need to add a new server in the config window. 
To do that open the settings window and click on [ADD].
Now fill in the input fields with the server data and press [ADD].

Adding Stream Infos is not necessary for connecting to a server.

By clicking on the [Save Settings] button, butt will save all changes
you have made.

butt will remind you about unsaved changes when you close it.


Streaming:
----------
To start streaming just klick the [play] button.
butt will try to connect to the server until you press the stop button.

You can change the audio settings (bitrate, channels) while you are streaming.
(Works only for mp3)

Unfortunately, it is not possible to update the Stream Infos while streaming.
You need to reconnect for updating the Stream Infos.

However, you can update the current song on the fly.
You only need to type the song into the {Song Name} input field at the 
[Stream] tab and press [OK].

butt can also update the song automatically from a textfile.
The first line of the textfile must be the name of the song.
As soon as butt detects that the file has been changed it updates the
name of the song on the server.
A plugin for the amarok audio player can be found in the player_plugins/
directory.
Don't hesitate to write a plugin for other audio players.
Just mail them to me and I'll add them to the butt package.
:-)


Recording:
----------
butt is able to record and stream simultaneously - in different bitrates.
For example you can stream with 96kbit and record with 192kbit.

To record you need to select the destination folder and specify a filename 
in the [Rec] tab. 
butt will replace the variables %d, %m and %y with the current day, month and year.
e.g. "rec_(%m_%d_%y).mp3" -> "rec_(03_28_2008).mp3".

With the %i variable you can add an index number to your filename.
This means with rec_%i.mp3 butt first tries to open rec_0.mp3. If that
file already exists, butt tries rec_1.mp3 and so on...

If the [start rec. when connected] checkbox is activated butt starts the
recording immediately after being connected to a server.

If this checkbox is deactivated butt only starts recording when pressing the
[rec] button.

To stop recording simply click on the [record] button again.

butt supports recording in mp3 and ogg and wav.
When recording to wav the stream and record samplerates are linked together.


Display:
--------
Symbols:

The [>] symbol shines yellow if butt is connected to a server.

The [O] symbol shines orange if the [start rec. when connected] checkbox is activated.
The [O] symbol shines red if butt is currently recording.

- You can toggle the Info on butts display by clicking the left mouse button
- The display colors can be changed in the GUI tab of the settings menu


Contact:
--------
butt at danielnoethen dot de

http://sourceforge.net/projects/butt

irc.freenode.org #butt




# yad-twitch-streamlink
yad-twitch-streamlink is a bash script that uses yad for a GUI.  It lists the users followed Twitch streams.  
After selecting a stream, yad-twitch-streamlink opens Streamlink with the configured player and also opens the configured chat program.
Streamlink path and arguments, chat program and arguments, and video player program and arguments are all configurable in the GUI or in the conf file.
Dependencies: Streamlink (optional; mpv can also be used directly for stream playback), yad, GNU coreutils, curl, wget

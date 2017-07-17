# yad-twitch-streamlink
yad-twitch-streamlink is a bash script that lists your live followed streamers from Twitch for playback using Streamlink. After selecting a stream, yad-twitch-streamlink opens Streamlink with the configured player and also opens the configured chat program.

Streamlink path and arguments, chat program and arguments, and video player program and arguments are all configurable in the GUI or in the conf file.

The config file is stored in `~/.config/yad-twitch-streamlink/yad-twitch-streamlink.conf` and pictures for the stream list are temporarily stored in `~/.config/yad-twitch-streamlink/cache/` while the stream list is open.

`streamlink --twitch-oauth-authenticate` is used to get your Twitch token for the stream list and for authenticating when viewing streams.  

If you do not have Streamlink installed, [an alternate site](http://twitchapps.com/tmi/) will be opened for you to get your Twitch token.  The token from this site will not work with Streamlink, so if you wish to use Streamlink later, you will have to generate a new token in yad-twitch-streamlink's settings menu.

yad-twitch-streamlink can also play Twitch streams without Streamlink by using mpv directly, although Streamlink usually provides less delay and better playback in general than using mpv alone.

Supported chat programs are Chatty and Chrome/Chromium.  Other Twitch chat apps or web browsers should also work with the proper arguments for them.  You can also choose to not have chat launched when the stream is opened.

Dependencies: Streamlink (optional; mpv can also be used directly for stream playback), yad, GNU coreutils, curl, wget



Stream list:

![yad-twitch-streamlink stream list](/screenshots/streamlist.png)



Settings menu:

![yad-twitch-streamlink settings menu](/screenshots/settings.png)



Help window (opens a browser for help pages for Streamlink, mpv, and Chatty):

![yad-twitch-streamlink help window](/screenshots/help.png)

[yad-twitch-streamlink preview video](https://raw.githubusercontent.com/simoniz0r/yad-twitch-streamlink/master/yad-twitch-streamlink.webm)

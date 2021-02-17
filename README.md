# SiriusXM

This script creates a server that serves HLS streams for SiriusXM channels. To use it, pass your SiriusXM username and password and a port to run the server on. For example, you start the server by running:
`python3 sxm.py myuser mypassword -p 8888`

You can see a list of the channels by setting the -l or --list flag:
`python3 sxm.py myuser mypassword -l`

Then in a player that supports HLS (QuickTime, VLC, ffmpeg, etc) you can access a channel at http://127.0.0.1:8888/channel.m3u8 where "channel" is the channel name, ID, or Sirius channel number.

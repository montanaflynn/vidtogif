# vidtogif

A simple shell script I wrote to learn more about creating command line tools in various shells. It works by converting the video to images using ffmpeg and then converting those images into an animated gif with imagemagick.

Of course you could always do it in a oneliner:

`ffmpeg -i input.mp4 -vf scale=600:-1 -r 5 -f image2pipe -vcodec ppm - | convert - gif:- | convert -layers Optimize - output.gif`

But then you miss out on

- Dependency checking
- Usage and help information
- Nice error notifications

TL;DR

`vid2gif -w 600 -r 5 ./screencast.mov ./output.gif`

Here's an example of a gif created with the command above:

![gif of me making vidtogif](http://i.imgur.com/RwESKPg.gif)
# vidtogif

A simple shell script I wrote to learn more about creating command line tools. It works by converting the video to images using ffmpeg and then converting those images into an animated gif with imagemagick.

```
Usage: 
    vidtogif [-r <integer> -w <integer> -h <integer> -u -v] input.mp4 output.gif

Options: 
    -r: Framerate per second <integer>
    -w: Set max width <integer>
    -h: Set max height <integer>
    -u: Print usage information
    -v: Version

Example:
    Example: vidtogif -r 10 -w 600 input.mp4 output.gif


Here's an example of a gif created with vidtogif:

![gif of me making vidtogif](http://i.imgur.com/RwESKPg.gif)
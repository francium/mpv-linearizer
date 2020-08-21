## What is this?
Basically allows you to make a playlist out of time ranges in a single file. Or
to put it another way, this allows you to consume a media file in a particular
order. For example, watch a video that has a non-linear storyline in a linear
fashion.

You can define a `playlist.txt` file,
```
/home/francium/long-lecture.mp3

# Skip intro and play first part
00:00:30 00:20:00

# Play last 5 minutes
00:55:00 00:59:59

# Play middle part
00:20:01 00:54:59
```

And then run this script to watch/listen to it in the defined order,
`./mpv-linearizer playlist.txt` (make sure `python-mpv` is either installed
globally or virtualenv with it install is activated)


## Requirements
- `mpv`
- `python3.7+`
- `python-mpv` Python module
- A file that can be played by `mpv`

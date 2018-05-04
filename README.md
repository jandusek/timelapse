# timelapse
Tool for processing GoPro Timelapses

This script depends on [VidStab library](https://github.com/georgmartius/vid.stab). To install ffmpeg with it, use the `--with-libvidstab` flag, e.g:

```
$ brew reinstall ffmpeg --with-libvidstab --with-x265
```

The `directory` argument needs to contain GoPro image files with the filenames in format `Gxxxxxxx.JPG`.

### Usage:

```
Usage:
timelapse [-o outfile] [-r resolution] [-f fps] [-5] directory

  -o  define output filename
  -r  output file resolution, e.g. 1280x720, default: 1920x1080
  -r  frames per second, default: 30
  -5  encode the output file using x265 (default is x264)
```

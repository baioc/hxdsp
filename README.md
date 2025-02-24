hxdsp
======

![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/baioc/hxdsp)

A simple FFT library implemented in Haxe for cross-platform signal processing.
<br/>
Contributions are more than welcome!


Usage
------

You can use [haxelib to install this library straight from the git repo](https://lib.haxe.org/documentation/using-haxelib/#git):

```sh
haxelib git hxdsp https://github.com/baioc/hxdsp
```

For more details, check out the [current API docs](https://www.baioc.dev/hxdsp/).


Example
------

A ~~unsuccessful~~ modest attempt at a [melody extraction program](examples/Melody.hx) is provided in this repository.
On unix systems having `ffmpeg` and `gnuplot` installed, you only need to add an audio file of your own to the path `res/track.mp3` and, after `haxelib install format`, run

```sh
haxe examples/example.hxml
```

| Sample spectrogram data displayed with the help of `gnuplot` |
|---|
| ![spectrogram](https://user-images.githubusercontent.com/27034173/137220034-0d8361d0-7401-45d1-87ad-87dba4f7bd7f.png) |

The example program will also synthesize the extracted melody and place it into `res/synth.wav`.
You can then play it and check for yourself what the result sounds like (I suggest lowering your volume, just in case).

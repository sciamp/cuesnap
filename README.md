# CueSnap

Snapping MP3s with [cue files](http://en.wikipedia.org/wiki/Cue_sheet_(computing))
faster than your mom pops Pringle cans.

## Setup

_Tested on Mac OS X 10.7 (Lion)._

**Prerequisites**
 1. [Ruby 1.9.2 or Greater](https://rvm.io/)

**Okay, let's go**

 1. `brew install libmp3splt` _Install the mp3 clipping lbrary, it does the heavy-lifting._
 1. `gem install cuesnap`
 1. `cuesnap phattrack.mp3 phattrack.cue` _*snap -- zzrgt -- crack*_
 1. `open phattrack` _Gaze into the eyes of your slim mp3 files_

## Usage

**Run**

`cuesnap supercool_but_so_large.mp3 supercool.cue`

**and you get**

```
  supercool_but_so_large\
    |
    |- 01 Intro.mp3
    |- 02 Holy Crap - So Cool.mp3
    |- 03 Slower Crap - Pretty Coo.mp3
    |- 04 It's On - Like Donkey Kong.mp3
```

## Command Line Options

```
  --no-spaces (-ns) -
    White space in file names, ARE YOU FUCKING INSANE?
      e.g. 02_Holy_Crap_-_So_Cool.mp3
  --no-numbers (-nn) -
    Because, fuck sorting.
      e.g. Holy Crap - So Cool.mp3
```

## Setup for Development

 1. `git clone http://github.com/mutewinter/cuesnap` _Clone this repo, duh._
 1. `cd cuesnap` _Change directory into the folder._
 1. `brew install libmp3splt` _Install the mp3 clipping lbrary, it does the heavy-lifting._
 1. `bundle` _Setup those pretty Ruby gems._
 1. `cuesnap phattrack.mp3 phattrack.cue` _*snap -- zzrgt -- crack*_
 1. `open phattrack` _Gaze into the eyes of your slim mp3 files_

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

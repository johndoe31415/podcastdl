# podcastdl
Script that retrieves the RSS feeds of your favorite podcasts and downloads the
MP3 files neatly named so you can access them offline (while on the road or on
a plane).

## Usage
```
usage: podcastdl [-h] [-m days] [-o dir] [-v] sources [sources ...]

Download podcast audio files from a XML RSS feed.

positional arguments:
  sources               Podcast definition source file(s) that should be
                        polled

optional arguments:
  -h, --help            show this help message and exit
  -m days, --max-age-days days
                        Maximum age in days of the podcasts that should be
                        downloaded. By default, no restriction is applied to
                        the download.
  -o dir, --output dir  Directory which all podcast files are written to.
                        Defaults to podcasts/.
  -v, --verbose         Increases verbosity. Can be specified multiple times
                        to increase.
```

Where the source JSON files look like this:

```
[
    {
        "name":     "Heavyweight",
        "rss":      "https://feeds.megaphone.fm/heavyweight"
    }
]
```

Also, if you don't know it yet, listen to Heavyweight. It's a great podcast.

## License
GNU GPL-3.

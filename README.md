# Songbook Library

Songs with guitar chords (ChordPro) for the KOReader plugin
[Songbook](https://github.com/mzimandl/songbook.koplugin), which adds this
repository as its default song server.

- `songs/<id>.cho`: the songs; the id (file name) is lowercase ASCII with hyphens.
- `index.json`: the song list the plugin reads, built by `tools/build_index.py`
  (the *Build song index* workflow runs it after every push).
- `songbook.json`: the repository's name shown in the plugin.
- `template.cho`: every supported ChordPro directive, a start for a new song.

Chords use the international notation (B, Bb, Am, F#) and every song says so
with `{meta: notation en}`; the plugin shows them in Czech (H, B, Ami) when the
reader chooses it.

Copy this repository to start your own song server, then add its GitHub address
in the plugin (Settings → Song repositories → Add repository…).

## License

The song texts are traditional or in the public domain. The transcriptions,
chords and tools of this repository are dedicated to the public domain under
[CC0 1.0](LICENSE): you may copy, change and share them without asking.

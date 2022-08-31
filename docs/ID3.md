ID3 is a standard for encoding [metadata](metadata "wikilink") into
[MP3](MP3 "wikilink") files.

## Header

### Version 1

ID3 version provides minimal information. The first 128 bytes of the
file contain title, artist, album, year, genre and comment information.
The [header](header "wikilink") begins with the string "TAG".

### Version 2.xx

ID3 Version 2+ is much more complicated than v1, and may contain a wide
variety of information, including attached pictures, lyrics, encoding
software, file owner and payment data. In practice, the most commonly
used fields however tend only to list such information as album, artist
and track details.

The header may be placed anywhere in the file, being preceded by the
string "ID3".

## External Links

- [ID3 Standard Homepage](http://www.id3.org)
- [id3lib](http://id3lib.sourceforge.net/), a widely-used open source
  C/C++ ID3 implementation.
- [Java library MP3](http://www.vdheide.de/projects.html)
- [MP3::Info](http://search.cpan.org/dist/MP3-Info/) (Perl)
- [MPEG::ID3v2Tag](http://search.cpan.org/dist/MPEG-ID3v2Tag/) (Perl)
- [getID3() - The PHP media file parser](http://getid3.sourceforge.net/)
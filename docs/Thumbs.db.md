Thumbs.db is a file created by [Windows](Windows "wikilink") when
[thumbnail](Thumbnails "wikilink") view is used. It is a hidden file not
viewed by most users and not updated when files are moved from a folder
which images have passed through or deleted. This gives a secondary
chance that someone will leave behind at least partial evidence of an
image in their [Windows](Windows "wikilink") folders.

The [thumbnails](thumbnails "wikilink") in Thumbs.db are stored in the
[OLE Compound File](OLE_Compound_File "wikilink") format. It's the same
format that [Microsoft Office](Microsoft_Office "wikilink") uses.

There is a forensic open source application developed at sourceforge
called [vinetto](vinetto "wikilink") at
<http://sourceforge.net/projects/vinetto> that can extract them. It does
require a python environment. Additionally, there are several other Java
solutions based around the Jakarta project that is apart of Apache.
Additional resources about thumbs.db can be found in a white paper at
<http://www.accessdata.com/media/en_US/print/papers/wp.Thumbs_DB_Files.en_us.pdf>.

MiTeC Windows File Analyzer [1](http://www.mitec.cz/wfa.html) is a tool
for forensic analysis of Thumbnail Databases,
[Prefetch](Prefetch "wikilink") files, [shortcuts](LNK "wikilink"),
IExplore Index.DAT files and Recycle Bin contents on a
[Windows](Windows "wikilink") system. It will print a report of analyzed
files.

# Windows Vista/7

*See [Vista thumbcache](Vista_thumbcache "wikilink")*

Thumbs.db no longer exists in Vista/7 as individual files. This data has
been moved to a centralized database located in
*\Users\\%username%\AppData\Local\Microsoft\Windows\Explorer*

[Windows](Windows "wikilink") Vista will save thumbnails for files on
mounted encrypted file systems (except
[EFS](Windows_Encrypted_File_System "wikilink")).

In Windows 7, thumbs.db files are not created under normal usage when a
user browses a folder in explorer. However, they are created if the same
folder is browsed through its network path such as via \\\localhost\c\$.
These files do not follow the xp thumbs.db format. The format is still
an OLE container but without the Catalog stream and with a few other
changes.

# Windows 8/8.1

In Windows 8 and 8.1, both thumbcache and thumbs.db are present.
Thumbs.db will only be created in folders which reside under a user
profile folder (C:\Users\USERNAME\\\*). But accessing other folders
using their network paths such as \\\localhost\c\$ will create thumbs.db
in other folders as well. The format of these thumbs.db files is the
same as Windows 7 thumbs.db.

## External Links

- [Windows thumbnail cache
  (thumbs.db)](http://www.thumbnailexpert.com/en/formats/windows-thumbnail-cache/)
- [Windows 7 generated
  Thumbs.db](http://www.swiftforensics.com/2012/07/windows-7-generated-thumbsdb.html)
- [Windows 8 Thumbs.db
  files](http://www.swiftforensics.com/2014/04/windows-8-thumbsdb-files-still-same-and.html)

[Category:File Formats](Category:File_Formats "wikilink")
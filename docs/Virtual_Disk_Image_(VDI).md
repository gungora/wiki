## Image structure

VirtualBox Virtual Disk Image (.vdi) files are structured in essentially
the same way:

- A header descriptor (512 bytes)
- An image block map: If the (maximum) size of the virtual HDD is *N*
  MB, then this map is *4N* bytes long.
- Block alignment padding: The header format allows for padding between
  the image block map and the image blocks, and (as of version 1.6.2)
  the CreateVDI function adds padding after the map to ensure that the
  first image block begins on a 512byte sector boundary. Since the
  allocation unit on both NTFS and Ext3 file systems is 4096 bytes, you
  will therefore get slightly better performance (typically a few %) if
  you make your VDIs (1024N – 128) MByte long.
- Up to *N* x 1MByte image blocks.

## See Also

- [Disk Images](Disk_Images "wikilink")

## External Links

- [1](https://forums.virtualbox.org/viewtopic.php?t=8046), All About
  VDI's (VirtualBox forums)

## Tools

- [libvhdi](libvhdi "wikilink")
- [VDI Data
  Recovery](http://www.bitrecover.com/vdi-recovery-software/) - Data
  recovery software for VDI (Virtual Disk Image) files.

[Category:File Formats](Category:File_Formats "wikilink")
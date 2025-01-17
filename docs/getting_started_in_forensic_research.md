---
tags:
  - No Category
---
Interested in getting involved in computer forensics research? Here's
how to start.

## Recommended Reading

1.  Read the proceedings for the past four years of the
    [DFRWS](http://www.dfrws.org) conference. If a specific article
    looks interesting, download it and read it!

\#\*[DFRWS 2011 Program](http://www.dfrws.org/2011/program.shtml)

\#\*[DFRWS 2010 Program](http://www.dfrws.org/2010/program.shtml)

\#\*[DFRWS 2009 Program](http://www.dfrws.org/2009/program.shtml)

\#\*[DFRWS 2008 Program](http://www.dfrws.org/2008/program.shtml)

\#\*[DFRWS 2007 Program](http://www.dfrws.org/2007/program.shtml)

\#\*[DFRWS 2006 Program](http://www.dfrws.org/2006/program.shtml)

1.  Review the proceedings from the past few years of the IEEE/SADFE
    (Systematic Approaches to Digital Forensics Engineering) workshops.
    The papers do not appear on the website, but you can generally find
    them with Google by searching for the title in quotes
    - [SADFE 2011
      Program](http://conf.ncku.edu.tw/sadfe/sadfe11/program.html)
    - [SADFE 2010
      Program](http://conf.ncku.edu.tw/sadfe/sadfe10/program.html)
    - [SADFE 2009
      Program](http://conf.ncku.edu.tw/sadfe/sadfe09/program.html)
    - [SADFE 2008
      Program](http://conf.ncku.edu.tw/sadfe/sadfe08/program.html)
2.  Review the [IFIP Working Group 11.9 on Digital
    Forensics](http://www.ifip119.org/) website and look at the
    proceedings from the past conferences (unfortunately, you can't
    download the papers and the book costs more than \$100, but if you
    see something interesting it can usually be requested via
    interlibrary loan) (Some higher education libraries subscribe to
    SpringerLink which makes full text of these proceedings available to
    students and faculty as part of the school subscription)
    - [IFIP WG 11.9 publications](http://www.ifip119.org/Publications/)
3.  Search for interesting forensic terms at the [ACM Digital
    Library](http://portal.acm.org/dl.cfm) and
    [CiteSeer](http://citeseer.ist.psu.edu/)
4.  Review the [Sleuth Kit Website](http://www.sleuthkit.org/). In
    particular, review the issues of [The Sleuth Kit
    Informer](http://www.sleuthkit.org/informer/index.php) and download
    a copy of Sleuth Kit for your computer.

## Recommended Mailing Lists

- [sleuthkit-users](https://lists.sourceforge.net/lists/listinfo/sleuthkit-users)
- [linux_forensics](http://groups.yahoo.com/group/linux_forensics/join)
- [cftt](http://groups.yahoo.com/group/cftt/join) (computer forensic
  tool testing)

## Setting up a C++ development environment

Many people working in forensics find it useful to be able to compile
their tools from source code. Most of the tools compile on Linux, Mac,
and within the Cygwin environment under Windows.

Because all of these tools build upon one another, it is important to
compile and install them in the order specified below.

1.  Download a copy of [libewf](http://sourceforge.net/projects/libewf/)
    and install it on your computer. This will allow your forensic tools
    to read and process EnCase [E01](e01.md) disk images.
2.  Download a copy of [Sleuthkit](http://www.sleuthkit.org/sleuthkit/)
    and install it. SleuthKit is the basic open source computer
    forensics tool that allows the extraction of files from disk images.
    You can use it to recover deleted files.

If you are interested in doing file recovery, you may also wish to
explore:

- SleuthKit, above
- [PhotoRec](http://www.cgsecurity.org/wiki/PhotoRec), a file carver.
- [Adroit Photo Recovery](http://digital-assembly.com/), a commercial
  photo recovery tool that's pretty amazing.

If you want to experiment with automated computer forensics research,
try these:

- [Bulk Extractor](bulk_extractor.md), a program from the Naval
  Postgraduate School that searches a disk image for email addresses and
  prints a histogram.
- [fiwalk](fiwalk.md), a program that processes a disk image and
  outputs an XML or ARFF file containing information about all of the
  file system metadata. fiwalk is now part of SleuthKit.

## Exercises for the Reader

1.  Download the file
    [nps-2009-canon2-gen6.raw](http://digitalcorpora.org/corp/images/nps/nps-2009-canon2/nps-2009-canon2-gen6.raw)
    from the Digital Corpora website and try to recover as many files as
    you can. Some of the JPEGs can only be found using file carving, and
    some can only be found with fragment recovery file carving.
    - Can you determine when the photos were taken?
    - Can you determine *where* the photos were taken?
    - Can you determine the username of the person who took the photos?
    - Can you determine the clock offset of the camera from real time?

<!-- -->

1.  Download the file
    [usbnist1.gen3.aff](http://digitalcorpora.org/corp/images/nps/nps-2009-ubnist1/ubnist1.gen3.aff)
    and find the government documents that were stored on the USB
    device.
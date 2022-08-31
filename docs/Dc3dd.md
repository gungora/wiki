**dc3dd** is a patched version of [GNU dd](dd "wikilink") with added
features for computer forensics. It was developed at the [DoD Cyber
Crime Center](DoD_Cyber_Crime_Center "wikilink") by [Jesse
Kornblum](Jesse_Kornblum "wikilink"). The first release, corresponding
to Coreutils version 6.9.91, was published on 1 Feb 2008.

## Comparison to GNU dd

The following features are available in dc3dd that are *not* found in
[GNU dd](dd "wikilink"):

- On the fly [hashing](hashing "wikilink") with multiple algorithms
  ([MD5](MD5 "wikilink"), [SHA-1](SHA-1 "wikilink"),
  [SHA-256](SHA-256 "wikilink"), and [SHA-512](SHA-512 "wikilink")) with
  variable sized [piecewise hashing](piecewise_hashing "wikilink")
- Able to write errors directly to a file
- Combined error log. Groups errors together (e.g.
  `Had 1,023 'Input/ouput errors' between blocks 17-233'`)
- Pattern wiping. Wipe output files with a single hex digit or a text
  pattern
- Verify mode
- Progress reports. See the progress of the operation while it's running
- Split output. Able to split output files into fixed size chunks

The following changes to GNU dd's behavior were made:

- On a partial read, the whole block is wiped with zeros. This allows
  for repeatable reads/hashes of a drive with errors.

## Comparison to dcfldd

Although there are definitely similarities between dc3dd and
[dcfldd](dcfldd "wikilink"), the programs are based on slightly
different code bases and have different feature sets. dcfldd is a fork
of GNU dd, whereas dc3dd is a patch to the current version. This means
that dc3dd will be updated every time GNU dd is updated, whereas dcfldd
has its own release schedule. Certain features added to GNU dd after
dcfldd forked, such as direct input/output mode, are not found in
dcfldd.

On the other hand, dcfldd supports more hashing algorithms than dc3dd,
allows the user greater control over how hashes are displayed, supports
wiping output files with random patterns, and is supported on the
[Cygwin](Cygwin "wikilink") platform.

## See Also

- [dcfldd](dcfldd "wikilink")

## External Links

- [Official web site](http://dc3dd.sf.net/)
- [Sourceforge project page](http://sourceforge.net/projects/dc3dd/)
- [Step by step how-to for
  dc3dd](http://www.myfixlog.com/fix.php?fid=33)
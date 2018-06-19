# scanit
A customizable distributed IPv4/TCP/UDP scanner for discovering services

_Needs at least:_
- csv2html: git clone https://github.com/Gangerl/csv2html.git
- diff2html: git clone https://github.com/EugenDueck/diff2html.git

these should be installed in parallel to the scanit-Directory, i.e. where you did the git clone Gangerl/scanit.git
- zmap installed, with privileges (set by setcap, see in the file)
For more scanners see file :-)

_Usage:_
scanit needs 2 parameters: <Option> <Projectname>
Options: scanhere, scan, eval, create, clone, delete

_Example:_
1.) Create a new project, e.g. "myhomenet":
scanit create myhomenet

2.) Edit the created myhomenet.conf to suit your network and ports you want to scan:
vi myhomenet.conf

3.) Run the scanner, in this example at the same machine:
scanit scanhere myhomenet

4.) Start the evaluation with generating html output:
scanit eval myhomenet

You find the generated files under out/myhomenet/

Done.

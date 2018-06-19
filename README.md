# scanit
A customizable distributed IPv4/TCP/UDP scanner for discovering services

Needs at least:
zmap installed, with privileges (set by setcap, see in the file)
For more scanners see file :-)

Usage: 
scanit needs 2 parameters: <Option> <Projectname>
Options: scanhere, scan, eval, create, clone, delete

Example:
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

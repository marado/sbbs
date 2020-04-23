The files in this archive consist of the run-time files necessary to run a
current Synchronet development build, from scratch (plus a whole bunch of files
you don't actually need, but might want).

This archive includes everything also included in the following smaller
archives:
	sbbsexec.*
	sbbstext.*
	sbbsctrl.*
	
So if you have this archive, you do not need those.

This archive is intended for a fresh-install of Synchronet, so if you're
performing a manual update of an existing install, you might want to just
download and use the smaller archives in the future.

This archive and the others mentioned above are recreated *daily* on
cvs.synchro.net and may include new files and exclude old files when compared
with previous versions of the archives.

The CVS sub-directories are included so that if you have a CVS client
installed on your system you can just run "cvs update -d" at a later date and
receive updates to the files via anonymous-CVS. Use care when performing CVS
updates (or don't) in any sub-directory where you may have modified files
(e.g. ctrl and text).

If you are extracting this archive into an *existing* Synchronet installation,
be careful *not* to overwrite any files in your Synchronet "ctrl" directory
without careful consideration (usually, you don't want to do this) or any other
directory where you may have modified files (e.g. text). Some
exceptions include:
	- an *unmodified* text.dat file may be overwritten safely
	- *unmodified* .ini files may be overwritten safely

Normally, any modified files from "exec" should have been moved to your
"mods" directory, so as to not be susceptible to over-write.  So long as you
do this (or don't modify any files in exec/*), you should be fine to overwrite
any existing file in "exec" or its subdirectories (e.g. "load").

This archive does not contain any executable binaries or libraries. You will
need to get those from either sbbs_dev.tgz (for Linux-x64) or sbbs_dev.zip
(for Win32) or build them yourself from source (e.g. checked-out via CVS).

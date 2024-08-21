# MSXMake

Buildable version of make for MSX from 1994 created by the MSX Maniac.

## Description

MAKE takes a description of file-dependencies as input.  
Normally, a makefile will contain these descriptions but if no makefile is specified,  
MAKE can read from the standard input just as well.A description of a file-dependency  
contains subsequent filenames in the master-slave format:  

	MASTER: SLAVE.1 SLAVE.2 … SLAVE.n operation1 operation2

MAKE checks whether one of the slaves has been modified by comparing the time & date  
of the slaves against the time & date of the master.  
If the master is older then one of the slaves, the operations will be send to the standard output.  

Besides outputting these make operations, MAKE can also output backup commands.  
When youre using MSX-DOS2, MAKE checks the archive attribute of every file to determine  
if the file has been modified. If the file has been modified,  
the copy command will be send to the standard output.  

## Build

TODO, old bats

	B.BAT
	meek make /mbb:\make | command2
	
	M.BAT
	meek make > temp.bat
	temp.bat

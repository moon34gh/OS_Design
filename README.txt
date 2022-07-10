Programming Assignment #1 - Creating a Shell Using Java, Operating Systems Design

17102047 Jihoon Moon

-----------------------------------------------------------------------------------------------------
+ Program Explanation
	
	- Typing “ls” command with a specific directory is to show all files in its directory.
	- Typing “pwd” command is to show a current working directory.
	- Typing “ps” command is to show process status.
	- Typing “cat” command with a specific file is to show all contents of its file.
	- Typing “cd” command alone is to change a current directory to a user home directory. (1)
	- Typing “cd” command with “..” is to show an upper directory of the current directory. (2)
	- Typing “cd” command with a specific directory is to change the directory to entered directory. (3)
	- Typing “cd” command with “/home” is to change a current directory to home directory. (4)
	- Typing “history” command alone is to show all records of what you ran before. (5)
	- Typing “history” command with “!!” is to execute a previous command. (6)
	- Typing “history” command with “!(integer)” is to execute (integer)th command. (7)
	- Typing “exit” or “quit” command makes program power off. (8)
	
-----------------------------------------------------------------------------------------------------
+ Code Explanation
	
	+ Variables 
	- absolutePath is a user home directory.
	- path is a current working directory.
	- history is ArrayList that stores history.
	- hisCheck is a boolean value which decide to execute history code.
	- hisCode is a code that will be executed.
	- dList is ArrayList that stores a current command.

	+ cd_f 
	- it gets ArrayList and path.
	- Line 13 to 15 (1,4)
	- Line 21 to 24 (3)
	- Line 25 to 33 (2)
	- Line 34 to 38 (3)
	- Line 41 to 47 is to check whether a file exists or not.

	+ history_f
	- it gets ArrayList.
	- Line 51 to 55 (5)
	- Line 56 to 62 (6)
	- Line 63 to 81 (7)

	+ main
	- Line 90 to 96 is to check whether history code is executed or not.
	- Line 98 to 103 is to store an entered command into ArrayList.
	- Line 104 to 107 (8)
	- Line 108 to 112 is a condition statement to execute “cd” function.
	- Line 113 to 116 is a condition statement to execute “history_f” function.
	- Line 119 to 133 is to execute ProcessBuilder and to show its result.

-----------------------------------------------------------------------------------------------------
17102047 Jihoon Moon


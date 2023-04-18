0x03. Shell, init files, variables and expansions :
0-	Create a script that creates an alias:
#!/bin/bash
alias ls="rm *"

1-	Create a script that prints hello user, where user is the current Linux user:
#!/bin/bash
echo "hello $USER"

2-	Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program:
#!/bin/bash
export PATH=$PATH:/action

3-	Create a script that counts the number of directories in the PATH:
#!/bin/bash
echo $PATH | tr ':' '\n' | wc -l

4-	Create a script that lists environment variables:
#!/bin/bash
Printenv

5-	Create a script that lists all local variables and environment variables, and functions:
#!/bin/bash
Set

6-	Create a script that creates a new local variable:
•	Name: BEST
•	Value: School
#!/bin/bash
BEST=School

7-	Create a script that creates a new global variable.
•	Name: BEST
•	Value: School
#!/bin/bash
export BEST="School"

8-	Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line:
#!/bin/bash
echo $((128+ $TRUEKNOWLEDGE))

9-	Write a script that prints the result of POWER divided by DIVIDE, followed by a new line.
•	POWER and DIVIDE are environment variables
#!/bin/bash
echo $((POWER / DIVIDE))

10-	Write a script that displays the result of BREATH to the power LOVE
•	BREATH and LOVE are environment variables
•	The script should display the result, followed by a new line
#!/bin/bash
echo $((BREATH**LOVE))

11-	Write a script that converts a number from base 2 to base 10.
•	The number in base 2 is stored in the environment variable BINARY
•	The script should display the number in base 10, followed by a new line
#!/bin/bash
echo $((2#$BINARY))

12-	Create a script that prints all possible combinations of two letters, except oo.
•	Letters are lower cases, from a to z
•	One combination per line
•	The output should be alpha ordered, starting with aa
•	Do not print oo
•	Your script file should contain maximum 64 characters
#!/bin/bash
echo {a..z}{a..z} | tr " " "\n" | grep -v "oo"

13-	Write a script that prints a number with two decimal places, followed by a new line.
The number will be stored in the environment variable NUM
#!/bin/bash
print "%.2f\n" $NUM

14-	Write a script that converts a number from base 10 to base 16.
The number in base 10 is stored in the environment variable DECIMAL
The script should display the number in base 16, followed by a new line
#!/bin/bash
printf "%x\n" $DECIMAL

15-	Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII :
#!/bin/bash
tr 'A-za-z' 'N-ZA-Mn-za-m'

16-	Write a script that prints every other line from the input, starting with the first line:
#!/bin/bash
paste -d, - - | cut -d, -f1

17-	
#!/bin/bash
echo $(printf %o $(($((5#$(echo $WATER | tr 'water' '01234'))) + $((5#$(echo $STIR | tr 'stir.' '01234'))))) | tr '01234567' 'bestchol')


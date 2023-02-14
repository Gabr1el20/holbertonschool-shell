alias ls="rm *" : creates an alias that will do the command described in the quotes
echo hello $USER : prints hello following by the current user
export PATH="$PATH:/action" : creates a directory in PATH.
echo $PATH | tr -s ":" '\n' | wc -l : shows the PATH, replace the ":" with a new line and then count the words by lines.
printenv : shows all the environmental variables
set :  lists all local variables and environment variables, and functions.
BEST=School : creates the local variable "BEST" with te "School" value.
export BEST=School : the same, but a global variable.
echo $((TRUEKNOWLEDGE+128)) :arithmetic expression, adding the value of TRUEKNOWLEDGE plus 128
echo $((POWER/DIVIDE)) : Divide two variables.
echo $((2#$BINARY)): converts a number from base 2 to base 10.
echo {a..z}{a..z} |tr ' ' '\n' | grep -v oo : match all the combinations between a..z and z..a. then replace the spaces with a new line. finally select selects all characters except those mentioned below.
printf '%.2f\n' $NUM : prints the float (with two characters") of the variable.
printf '%x\n' $DECIMAL : prints the hexadecimal version of the variable mentioned.
tr 'A-Za-z' 'N-ZA-Mn-za-m' : decode rot13
paste - - | cut -f1 : with paste - - you put the lines between each other. then select with -f 1 the first lines.
printf '%o\n' $(( 5#$( echo $WATER | tr water 01234 ) + 5#$( echo $STIR | tr stir. 01234) )) | tr 01234567 bestchol : prints the octal value of the sum of the translated version of the WATER and STIR variables, then translate the result to bestchol.

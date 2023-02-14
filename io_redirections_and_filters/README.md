echo "Hello, World" : prints the message in the quotes.
echo "\"(Ôo)'" : echoes that message. the backslash prevent the next character to be interpreted as a special character.
cat /etc/passwd : Shows all the files and directories inside the path described.
cat /etc/passwd/ /etc/hosts : The same but this time shows two paths.
tail /etc/passwd : Displays the last 10 lines of the file mentioned.
head /etc/passwd : Displays the first 10 lines.
cat iacta|head -3|tail -1 : Shows iacta, then shows the first three lines. Finally, with tail show only the last line.
echo -e "Best School" > "\*\\\'\"Best School\"\'\\\*\$\?\*\*\*\*\*:)" : creates a file with some text inside. Again, backslash act prevents the next character to be a special character
ls -la > ls_cwd_content : Shows the result of the command in the file after the ">".
tail -1 iacta >> iacta : with tail -1 select the last line. The ">>" put the result in the last line, duplicating that.
find . -type f -name "*.js" -delete : "." is the current directory. "-type f" choose only the files. "*.js" wildcard. "-delete" erase the files founded.
find . -mindepth 1 -type d | wc -l : "-mindepth 1" causes the current directory no to be counted. "-type d" is like "f" but for the directories. "wc -l" displays the result in number of lines.
ls -t | head : "ls -t" display the newest archives in the directory. with head you display only the 10 newest files.
sort | uniq -u : sort the content alphabetically. Then with "uniq -u" you display only the unique content.
grep -i root /etc/passwd : search for the "root" pattern in the /etc/passwd directory.
grep -i bin /etc/passwd | wc -l : with the result from the pattern search in the described path, you count the words.
grep "root" -A 3 /etc/passwd : with "-A 3" show the next 3 lines after the encountered pattern.
grep -v "bin" /etc/passwd : the option -v select all the non-matching lines that are described in the argument.
tr Ac Ze : replace the first arguments (Az) with the seconds (Ze).
tr -d Cc : with the option -d you delete the argument described.
rev : reverse lines characterwise.
cat /etc/passwd | cut -d ":" -f1,6 | sort : with "cut -d" you delimit, then with -f select the fields resulting from delimitation.
find . -empty -printf %f'\n' : "-empty" selects the empty files. "%f\n" makes a new line.
find . -type f -name "*.gif" |rev| cut -d "/" -f1 | cut -d "." -f2,3|rev|sort -fV : select the files with .gif extension. then rev and cut/delimit the "/" and select the field 1. cut/delimit the "." and select the fields 2 and 3. Reverse and finally sort alphabetically case sensitive.
cut -c 1|paste -s -d ' ' | tr -d ' ' : cut the first character. select and delimit the spaces with paste and then remove them.
tail -n +2|cut -f -1|sort -k 1| uniq -c| sort -n -r| head -n 11| cut -b 9- : display the last 2 lines. 

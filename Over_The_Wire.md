#Bandit
###Level0
pw: bandit0
Used: ls, cat
Got: boJ9jbbUNNfktd78OOpsqOltutMc3MY1

###1-2
The File has "-" for a name, due to that I have to specify the full location of
the file when using cat:
used: cat
cat ./-
pw: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

##2-3
Spaces are in the file name that hold the password
to do this you can either use escape character "\ " to indicate the space
e.g: cat file\ name\ with\ spaces
or you can wrap the filename in double quotes""
cat "file name with spaces"
also typing the first word then hitting space might autocomplete it for you to
the file you want

used: cat
cat file\ name\ with\ spaces
pw: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

###3-4
stored in a hidden file with a . infront of the filename

used: cat
cat .hidden
pw: pIwrPrtPN36QITSp3EQaw936yaFoFgAB

###4-5
files have a - infront of them, use the ./

used: cat
cat ./-file07
pw: koReBOKuIDDepwhWk7jZC0RTdopnAYKh

###5-6
File is human readable and 1033 bytes in size, as well as not executable

use: ls to find human readable, du
du -ab | sort h
cat : cat inhere/maybehere07/.file2
pw: DXjZPULLxYr17uwoI01bNLQbtFemEgo7

##6-7
Find is used a lot here as it displays the permissions for the files
There is one we have access to that has the password

use: find, size, cat
find / -user bandit7 -group bandit6 -size 33c
cat that file
pw: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

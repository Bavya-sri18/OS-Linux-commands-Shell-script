# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files

### cat < file1
<img width="266" height="170" alt="image" src="https://github.com/user-attachments/assets/3f01a7e0-8547-44d3-9fce-77c8f16098c9" />



### cat < file2

<img width="238" height="186" alt="image" src="https://github.com/user-attachments/assets/7cfb35e9-a9f1-4c5b-a146-34fcd9c9cce0" />


# Comparing Files
### cmp file1 file2

 <img width="371" height="73" alt="image" src="https://github.com/user-attachments/assets/588997a9-9e56-4ae4-979c-70fc7971e67b" />

### comm file1 file2
 
<img width="365" height="356" alt="image" src="https://github.com/user-attachments/assets/397cd5ba-4486-4ea3-a5ea-cb4c809cf83d" />

 
### diff file1 file2

<img width="312" height="348" alt="image" src="https://github.com/user-attachments/assets/ef473b3b-bbf7-4c25-afa6-35f5e05628f6" />


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```

## OUTPUT
### cut -c1-3 file11

<img width="285" height="177" alt="image" src="https://github.com/user-attachments/assets/35223d95-e07c-4613-a31a-b703c876fd31" />




### cut -d "|" -f 1 file22

<img width="292" height="168" alt="image" src="https://github.com/user-attachments/assets/867fdef3-2a17-4ad5-8daf-ee2369e0c7b5" />



### cut -d "|" -f 2 file22

<img width="303" height="172" alt="image" src="https://github.com/user-attachments/assets/74e148af-af6b-4bb5-bc05-44aa4c805667" />


cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world

## OUTPUT
 
### grep Hello newfile 
<img width="302" height="52" alt="image" src="https://github.com/user-attachments/assets/4cab2167-b2a6-42ad-bdcc-a925d9e6ffd1" />


### grep -v hello newfile 

<img width="282" height="76" alt="image" src="https://github.com/user-attachments/assets/2ee48064-5be9-4470-97c0-ca3271c8d619" />

### cat newfile | grep -i "hello"
<img width="398" height="83" alt="image" src="https://github.com/user-attachments/assets/e5e2f4f1-b40b-45a6-803a-ade01ed22886" />


### cat newfile | grep -i -c "hello"
<img width="432" height="81" alt="image" src="https://github.com/user-attachments/assets/3238b0be-761e-421c-b99f-e5668c25f6dd" />


### grep -R ubuntu /etc

<img width="938" height="323" alt="image" src="https://github.com/user-attachments/assets/ccd07de2-5b07-4d72-98af-bc0a45a47561" />

### grep -w -n world newfile   

<img width="341" height="77" alt="image" src="https://github.com/user-attachments/assets/6076164a-63f8-4922-9521-61dd51d5e108" />

cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```

### egrep -w 'Hello|hello' newfile 

<img width="382" height="78" alt="image" src="https://github.com/user-attachments/assets/61610730-6bdf-495b-a8da-f13f6f3fe8d8" />


### egrep -w '(H|h)ell[a-z]' newfile 

<img width="412" height="82" alt="image" src="https://github.com/user-attachments/assets/50fa270a-e5e5-433b-8850-9f75abd6d44c" />

### egrep '(^hello)' newfile 

<img width="353" height="73" alt="image" src="https://github.com/user-attachments/assets/0ebb3324-e0d4-4b62-94ec-2d1850975395" />

### egrep '(world$)' newfile 

<img width="341" height="75" alt="image" src="https://github.com/user-attachments/assets/2b72e4ed-9fc3-42e1-b9d7-56918534c671" />

### egrep '((W|w)orld$)' newfile 

<img width="366" height="97" alt="image" src="https://github.com/user-attachments/assets/601960ca-5123-4979-adc7-df8053f81149" />

### egrep '[1-9]' newfile 

<img width="287" height="53" alt="image" src="https://github.com/user-attachments/assets/9d91194b-f23d-4a62-a8df-e9e92efe96ba" />

### egrep 'Linux.*world' newfile 

<img width="377" height="61" alt="image" src="https://github.com/user-attachments/assets/4572697f-bfae-4ed4-8525-6c948c7027a7" />


### egrep l{2} newfile

<img width="283" height="52" alt="image" src="https://github.com/user-attachments/assets/473eab02-071a-48a8-8fb6-dada3d1b1d2f" />

### egrep 's{1,2}' newfile

<img width="307" height="103" alt="image" src="https://github.com/user-attachments/assets/c4fe5745-d7ae-4a0d-9d2b-338b317e3337" />


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```
## Output

## sed -n -e '3p' file23
<img width="295" height="80" alt="image" src="https://github.com/user-attachments/assets/810467bc-8915-4d91-bdba-20f4ccf6bea0" />

### sed -n -e '$p' file23
<img width="315" height="75" alt="image" src="https://github.com/user-attachments/assets/c487b11d-4b17-41b9-a605-216a7596e5b9" />

### sed  -e 's/Ram/Sita/' file23

<img width="346" height="251" alt="image" src="https://github.com/user-attachments/assets/032255f7-7b03-473d-ac05-98322a7efb09" />


### sed  -e '2s/Ram/Sita/' file23

<img width="358" height="252" alt="image" src="https://github.com/user-attachments/assets/a433805a-fff2-4ded-a814-4951d2220b81" />

### sed  '/tom/s/5000/6000/' file23

<img width="395" height="247" alt="image" src="https://github.com/user-attachments/assets/77cce062-c9c8-4b80-958e-84e053a10f6e" />

### sed -n -e '1,5p' file23
<img width="326" height="178" alt="image" src="https://github.com/user-attachments/assets/6ea6f6ac-2fde-4c44-9d16-940067132012" />


### sed -n -e '2,/Joe/p' file23

<img width="357" height="137" alt="image" src="https://github.com/user-attachments/assets/79c92ea7-c4e4-46e0-b58e-883e5c8146cc" />

### sed -n -e '/tom/,/Joe/p' file23

<img width="391" height="96" alt="image" src="https://github.com/user-attachments/assets/4df59614-0295-416c-a993-8f75a22ef5f3" />

### seq 10 

<img width="277" height="288" alt="image" src="https://github.com/user-attachments/assets/c46ae2ef-c68e-41a0-b79f-c72c4e676f1a" />


### seq 10 | sed -n '4,6p'
<img width="315" height="132" alt="image" src="https://github.com/user-attachments/assets/51f8bff7-b48e-48f8-b32e-40674091b954" />

### seq 10 | sed -n '2,~4p'
<img width="323" height="132" alt="image" src="https://github.com/user-attachments/assets/012aca22-cead-4a7b-beb5-acf254907139" />


### seq 3 | sed '2a hello'
<img width="297" height="145" alt="image" src="https://github.com/user-attachments/assets/37202c5a-32f6-4ee0-b920-aca16aacbc9b" />


### seq 2 | sed '2i hello'
<img width="337" height="127" alt="image" src="https://github.com/user-attachments/assets/476c1989-f6a6-489f-92b3-3acbb72d9e51" />


### seq 10 | sed '2,9c hello'
<img width="345" height="142" alt="image" src="https://github.com/user-attachments/assets/ff34dd83-d32e-4299-a140-1607554d679e" />


### sed -n '2,4{s/^/$/;p}' file23
<img width="410" height="132" alt="image" src="https://github.com/user-attachments/assets/42db06b4-e4c2-4e89-b293-c73e25a749df" />


### sed -n '2,4{s/$/*/;p}' file23
<img width="393" height="136" alt="image" src="https://github.com/user-attachments/assets/f4f172c6-8ed8-4844-b0d3-4fd5dbab04cb" />


# Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
## OUTPUT
### sort file21
<img width="332" height="178" alt="image" src="https://github.com/user-attachments/assets/5aea872d-f11f-4762-964b-0aafea63488a" />

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
### uniq file22
<img width="341" height="176" alt="image" src="https://github.com/user-attachments/assets/d3298691-91b8-40c9-bc59-f45e7dff05f3" />


## Using tr command

### cat file23 | tr [:lower:] [:upper:]
 <img width="433" height="248" alt="image" src="https://github.com/user-attachments/assets/d969cd8c-6561-4578-88bb-50cae64c06ce" />

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
### cat urllist.txt | tr -d ' '
<img width="373" height="128" alt="image" src="https://github.com/user-attachments/assets/d5b4c79b-9970-46ab-9120-b9e36ee37377" />

### cat urllist.txt | tr -d ' ' | tr -s '.'
<img width="477" height="128" alt="Screenshot 2025-09-13 084424" src="https://github.com/user-attachments/assets/5b035961-a76f-469a-bcc9-a2b48433d183" />


## Backup commands
### tar -cvf backup.tar *
<img width="297" height="371" alt="image" src="https://github.com/user-attachments/assets/a142c1e1-9952-4575-b9aa-9f299efdb075" />

### mkdir backupdir
 <img width="262" height="78" alt="image" src="https://github.com/user-attachments/assets/dca965f1-7405-489e-b791-a0b570aeeb7d" />

### mv backup.tar backupdir
<img width="327" height="81" alt="image" src="https://github.com/user-attachments/assets/b92bb4c3-1c1e-4f89-a680-80b0da3fba04" />

### cd backupdir
<img width="323" height="82" alt="image" src="https://github.com/user-attachments/assets/8f57ca1e-d0b5-4929-abda-ee73a5015148" />
 
### tar -tvf backup.tar
<img width="902" height="546" alt="image" src="https://github.com/user-attachments/assets/da7573f0-8054-4ea7-8b85-b3f4f191bb0e" />

### tar -xvf backup.tar
<img width="317" height="627" alt="image" src="https://github.com/user-attachments/assets/e54743c3-3062-44d0-96a9-dda9e2fb8e1e" />

### gzip backup.tar
<img width="341" height="81" alt="image" src="https://github.com/user-attachments/assets/1a732d5e-598a-4006-8e0e-73c667ee4c6f" />

### ls *.gz
<img width="353" height="82" alt="image" src="https://github.com/user-attachments/assets/b19135dd-ab1a-4f49-bc24-c08a72c3eb25" /> 

### gunzip backup.tar.gz
<img width="360" height="78" alt="image" src="https://github.com/user-attachments/assets/ddab4e10-f0f5-4383-936b-17a3040244b4" />

### Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
### chmod 755 my-script.sh
./my-script.sh
<img width="412" height="203" alt="image" src="https://github.com/user-attachments/assets/7d14c52d-e1f8-4bc3-8734-8d874fd74696" />

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

### cat herecheck.txt
<img width="353" height="160" alt="image" src="https://github.com/user-attachments/assets/ea8ae1e3-2adc-413f-a1db-163d189db8c2" />

cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
### chmod 777 scriptestest.sh
 <img width="377" height="51" alt="image" src="https://github.com/user-attachments/assets/87a641ab-ae7b-41ae-979c-2c025123417f" />

### ./scriptest.sh 1 2 3
<img width="617" height="412" alt="image" src="https://github.com/user-attachments/assets/c05a6b61-748c-4ffa-b89f-60be47330465" /> 

### ls file1
<img width="372" height="106" alt="image" src="https://github.com/user-attachments/assets/f4ad319a-8ede-4d11-ad1e-0c07ce7f00bf" />

### echo $?
<img width="363" height="77" alt="image" src="https://github.com/user-attachments/assets/18715c20-01e5-4460-8b0e-889d6c8ad6bc" />

./one
bash: ./one: Permission denied
 
### echo $?
 <img width="363" height="77" alt="image" src="https://github.com/user-attachments/assets/596afe71-ee32-486e-87f9-b6924e14141e" />
 
### abcd
 
### echo $?
<img width="363" height="77" alt="image" src="https://github.com/user-attachments/assets/089bd8e5-20ff-485c-95b6-598074ae7a1c" />

 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
## OUTPUT
<img width="367" height="287" alt="image" src="https://github.com/user-attachments/assets/d0a9a7af-0143-4888-acdb-3b15a5c11243" />

chmod 755 strcomp.sh
 
./strcomp.sh 

## OUTPUT
<img width="317" height="97" alt="image" src="https://github.com/user-attachments/assets/e1207fa6-bd8d-48ca-ac00-7a61c96110f0" />

# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT



# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT


# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT



$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 


# RESULT:
The Commands are executed successfully.

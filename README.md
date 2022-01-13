# TSI--Teacher-Student-Interface

Steps to execute the project TSI
Very initial step is to run the command make all which compiles both the codes and creates their corresponding executables.
The very next step, Teacher should open up 2 terminals; One for hosting the Server, Another for joining that server as a Teacher.
In the first terminal, Teacher has to run command ./ser 1234 or ./ser 1234 127.0.0.1 for starting the server at specified PORT & IP ADDRESS. [You can specify any PORT & IP ADDRESS (LAN) as long as systems are in the same NETWORK ].
After Entering name, Teacher has to type set-admin and hit enter and type password as admin@123 for setting Teacher Client as admin of this environment.
In the second terminal, Teacher has to run command ./cli 1234 or ./cli 1234 127.0.0.1 for joining the server created in STEP 3. After that type 1 & hit enter to register yourself as Teacher. And Enter name to continue further.
Now Student has to also run the command make all if on a different machine, for this example it is considered that Student is also on the same machine that's why server is created for localhost (127.0.0.1) on PORT 1234 so no need to run command make all at this moment.
Now Student has to run command ./cli 1234 or ./cli 1234 127.0.0.1 just like what we did at teacher side, but this time type 2 & hit enter to register yourself as Student. Enter name and Roll Number when asked.
After These Steps, the TSI environment should be completely established !

How To Share Files?
A. Student To Teacher File Sharing
Type 'send' and hit enter.
Specify the Name of the File to be sent (Must be in the same directory as the executables).
The file will be sent to the Admin (Teacher).
B. Teacher To Student File Sharing
Type 'send' and hit enter.
Specify Roll Number of Student to whom file supposed to be transfered.
If the Student with a given Roll Number is present in the server, then it will ask for a filename, just specify the Name of the File which is to be shared.
Hit enter and the file will be shared!

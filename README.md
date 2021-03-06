# janellecproject3
The goal of this project is to familiarize yourself with Python syntax, and some basic tasks that are common in systems programming and administration. The program will be invoked from the command line on a fresh Linux machine, so if you introduce any library dependencies beyond the Python Standard Library (not recommended), you must provide very clear instructions to recreate your environment. You should consider using vagrant or a GCP VM to develop in Linux if you are on a Windows machine. It is your responsibility to ensure the program runs as expected in the operational environment described. 

STEPS

Your program will be parsing and analyzing log files from an Apache web server. The first thing your program must do is retrieve the log file across the network. It is available here: https://s3.amazonaws.com/tcmg476/http_access_log

Once you download the file, you will be parsing the file in order to answer several questions:
How many total requests were made in the time period represented in the log?
How many requests were made on each day? per week? per month?
What percentage of the requests were not successful (any 4xx status code)?
What percentage of the requests were redirected elsewhere (any 3xx codes)?
What was the most-requested file?
What was the least-requested file?
 
You will need to output this data to the screen. The format you choose for this is up to you (human readable, machine readable, plain text, JSON, etc), but your decisions and the implementation should be logical and consistent. 

Finally, the logs should be broken into separate files by month. Your program should split the log file into 12 smaller files, where the data stored in each file are the log events for a single month. These should be written to disk in the same directory as your program file, in a logical and consistent manner. 

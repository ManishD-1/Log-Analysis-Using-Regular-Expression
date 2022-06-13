# Log-Analysis-Using-Regular-Expression
## Problem Statement
Imagine a company uses a server that runs a service called ticky, an internal ticketing system. The service logs events to syslog, both when it runs successfully and when it encounters errors.

The service's developers needs help getting some information from those logs so that they can better understand how their software is used and how to improve it. So, for this,I wrote some automation scripts that will process the system log and generate reports based on the information extracted from the log files.

## What Processes I Used

Used regex to parse a log file

Appends and modify values in a dictionary

Wrote to a file in CSV format

Moved files to the appropriate directory for use with the CSV->HTML converter

I have created a script, named ticky_check.py, that generates two different reports from this internal ticketing system log file i.e., syslog.log. This script will create the following reports:

## The ranking of errors generated by the system: 
A list of all the error messages logged and how many times each error was found, sorted by the most common error to the least common error. This report doesn't take into account the users involved.
## The user usage statistics for the service: 
A list of all users that have used the system, including how many info messages and how many error messages they've generated. This report is sorted by username.

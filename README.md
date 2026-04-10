# thread-analyze.sh

Get the PID (Process ID) of the service.
Use the following command to capture a thread dump: sh thread-analyze.sh <pid> <number-of-dumps> <interval>
Use the following command to capture a heap dump: jmap -dump:file=heap_dump-`date +%d-%m-%Y-%H:%M:%S`.bin <pid>

To take 4 thread dumps in one minute interval for java process with pid 1234

sh thread-analyze.sh 1234 4 1m

Available time units

s for seconds (the default), m for minutes,h for hours, d for days

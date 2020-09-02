# shell-data-processing

## Command to retrieve text from URL
* The curl command used to get data from the URL and store in a file is ```curl "http://shakespeare.mit.edu/romeo_juliet/full.html" -O data.txt```

## Commands used to process text data
* ```tr ' ' '\12' < data.txt``` is the command used to map each line into individual words.
* ```tr ' ' '\12' < data.txt | sort``` is the command used to sort the text in data file.
* ```tr ' ' '\12' < data.txt | sort | uniq -c``` is the command used to sort the output based on uniqueness of data
* ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr``` is used to send the output i.e unique words to sort with -nr flag. Where the numerical comparison is done with reversing results.
* ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt``` is used to store the output of previously executed command to result.txt file. 

## Up arrow in Bash
* Up arrow in bash shell is used to view the commands that were executed previously. 

## Bash Shell Commands
1. sort --This command displays arguments that are used while sorting with bash commands. 
1. "-n" - This command is used to sort the data by comparing with numerical value. 
1. "-r" - This command is used to reverse the results. 
1. One dash (-) is used for a single letter flag. 
1. when flag is more than one letter, two dashes (--) are used


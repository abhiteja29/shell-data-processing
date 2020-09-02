# shell-data-processing

## Command to retrieve text from URL
* curl command:
  ```curl "http://shakespeare.mit.edu/romeo_juliet/full.html" -O data.txt```

## Commands used to process text data
1. ```tr ' ' '\12' < data.txt``` is the command used to map each line into individual words.
1. ```tr ' ' '\12' < data.txt | sort``` is the command used to sort the text in data file.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c``` is the command used to sort the output based on uniqueness of data
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr``` is used to send the output i.e unique words to sort with -nr flag. Where the numerical comparison is done with reversing results.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt``` is used to store the output of previously executed command to result.txt file. 

## Bash Shell Commands
1. sort --help: This command sorts and displays arguments that are used with bash commands. 
1. "-n" - This command is used to sort the data by comparing it's numerical value. 
1. "-r" - This command reverse the results. 
1. One dash (-) is used for a single letter flag. 
1. two dashes (--) are used when flag is more than one letter 


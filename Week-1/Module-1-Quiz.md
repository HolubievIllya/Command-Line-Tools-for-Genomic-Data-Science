## Module 1 Quiz
#### Q1. Which of the following Unix commands can be used to view the content of a file?
- [x] more
- [ ] gzip
- [ ] ls
- [ ] cp
#### Q2. Which of the following commands can be using to compress the content of a file?
- [ ] rmdir
- [ ] cd
- [ ] top
- [x] gzip
#### Q3. The file "months" lists each of 12 months on a separate line, and no further lines. What would be result if the following command was run:
#### '''cat months | head -1000 | wc -l'''
- [ ] year
- [ ] 50
- [x] 12
- [ ] months
#### Q4. What is the effect of using the pipe operator "|" in a sequence of commands:
- [ ] Re-direct standard error only 
- [x] Re-direct the standard input or standard output of a command
- [ ] Act as a character separator between different shell commands, without any effects on the outcome
- [ ] Replace the ‘;’ sequencing operator in a complex command
#### Q5. If typing 'pwd' produces "/home/userA/Coursera/L1/", which of the following commands will list the file content of the current directory?
- [ ] listdir .
- [ ] more *.txt
- [ ] mkdir L1
- [x] ls /home/userA/Coursera/L1
#### Q6. Suppose you current working directory is "/home/Coursera/L1/", and "peach","apple", and "pear" are subdirectories, each containing a single file named "genome". What would be the current directory, as reported by running the 'pwd' command, after each of the four commands in the sequence below:
'''<ul>
  <li><b>cd apple</b></li>
  <li><b>rm *</b></li>
  <li><b>cd ../..</b></li>
  <li><b>mv apple plum</b></li>
</ul>
'''

- [x] <ul>
  <li><b>/home/Coursera/L1/apple</b></li>
  <li><b>/home/Coursera/L1/apple</b></li>
  <li><b>/home/Coursera</b></li>
  <li><b>/home/Coursera</b></li>
</ul>

- [ ] <ul>
  <li><b>L1</b></li>
  <li><b>Coursera</b></li>
  <li><b>apple</b></li>
  <li><b>plum</b></li>
</ul>

- [ ] <ul>
  <li><b>plum</b></li>
  <li><b>apple</b></li>
  <li><b>pear</b></li>
  <li><b>strawberry</b></li>
</ul>

- [ ]  <ul>
  <li><b>/home/Coursera/L1</b></li>
  <li><b>/home/Coursera/L1/apple</b></li>
  <li><b>L1/apple</b></li>
  <li><b>/home/Coursera/L1</b></li>
</ul>

#### Q7. Consider the file "seasons" with the following columns separated by space '':
#### '''cut -d ' ' -f1,3 seasons | sort -u | wc -l" and "cut -f1 seasons | sort | unic -c | wc -l''' ?
- [ ] 4, 6
- [ ] 12, 20
- [ ] 5, 10
- [x] 12, 12

#### Q8. Your current working directory is named "Plants". Its subdirectory "apple" contains the files "apple.genome", "apple.samples" and "apple.genes". What would be the result of the command '''rmdir apple'''?
- [ ] All files containing the string “apple” in their names will be removed
- [ ] None of these choices
- [x] The command will have no effect, since the directory is not empty
- [ ] The “apple” directory and all of its content will be removed

#### Q9. Suppose that you have two files, A and B, containing experiment data. What would be the sequence of outputs for the commands:
- [ ] 3, 2, 2
- [ ] 5,2,3 
- [x] 3, 1, 3
- [ ] 2, 4, 5

#### Q10. The current working directory contains four subdirectories named "apple", "pear", "peach" and "strawberry", each with the following files: "genome", "genes", and "samples". Which of the following commands wouls extract the top line from all of the "genes" files?
- [ ] cat *p*/genes strawberry/genes | tail -1 
- [x] head -1 *p*/genes strawberry/genes
- [ ] less */g* | head -1
- [ ] cat *p*/genes strawberry/genes | grep –c 1 


# MOSS How-To

## Prep

1. [Download the current version of the submissions script: http://moss.stanford.edu/general/scripts.html](http://moss.stanford.edu/general/scripts.html)
2. __Important__: Modify the submission script, `moss.pl` so that `$userid` is set to the id sent to you

## Comparing Homework Submissions

1. clone the repositories for the homework; __do not map usernames to ids__
2. if the submission folders are in the same directories that `moss.pl` is in, run:
  ```
$ perl moss.pl -l javascript -d homework##/*/src/*.js
```
  * -l : specifies the language, which will always be javascript
  * -d : specifies the files to compare. Compares every file in just src for each student, to avoid tests and/or node_modules
  * -m n : will ignore a file if it appears more than n number of times, this might come up on later homeworks
  * Further moss instructions are in the moss file itself, if any other options end up being needed
3. use the url outputted by the command to view the comparisons
  * __this url lasts for a week__

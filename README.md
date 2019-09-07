# *schl*
## Overview
*schl* is a XeLaTeX  package that provides commands and environments suitable for
document types that appear in a classroom enviromnent. It's development is based on 
the Greek educational practice, but it may be usefull in other contexts also.

Basic macros of the package are the following:

* Mathematics
  * `\sin, \cos, \tan, \cot, \gcd`: *schl* redefines these operators in Greek.
  * `\lcm`: Least common multiple operator.
  * `\limdisplay`: `\lim` operator in display mode.
* Blank space
  * `\lowerdots`: Use dots to designate blank space.
  * `\blankspace`: Use a line for blank space.
* Lists
  * `question, exercise, schltask`: Environments for typesetting questions, exercises and tasks.
  * `multichoice`: An environment for typesetting multiple choice answers.
  * `tickchoice` and `tickchoice`: `itemize` type lists with a square as symbol for each item.
  * `truefalse`: An environment for typesetting true-false type questions.
  * `matchingque`: A macro for typesseting matching questions.
* Answers, solutions and hints
  * `\answer`: For typesetting  the answer of an exercise.
  * `\solution`: For typesetting the solution of an exercise.
  * `\hint`: Typeset a hint for an exercise.
  * `\deadline`: Set the deadline date.
* Headers
  * `\worksheettitle`: Set the title of a worksheet.
  * `\examtitle`: Set the title of a summative test.
  * `\finalexamheader`: Set the header for end year summative tests.
  * `\theorypart, \exercisepart`: Headers for the theory and exercise parts of a document.
* School information
  * `\school, \headmaster, \teacher, \subject, \grade, \schoolyear, \schldate`
* Macros for tests
  * `\examtime`: Print the time of the exam.
  * `\points`: Set the points of an exercise.
  * `\fullname`: A field that accepts a name.
  * `\datefield`: A field for writing the date.
  * `\schoollogo` Prints school, teacher, grade and subject.
  * `\authoritylogo`: Prints a hierarchy of authorities starting from the Ministry of Education.
  * `\examdetails, \examdetailsii`: Print information about an exam.
  * `\signatures`: A field that prints the name of the teacher or the headmaster. 
  * `\wish`: Prints a wish for good luck.

 By default, *schl* prints all macros that accept text as *undefined*. As of this version, Greek
 is the only supported language. You can set it with the option `greek`. Other languages can be supported
 by redefining package's internal macros.

## Requirements
 *schl* loads the packages *fontspec, enumitem, mdframed* and *amsmath*. It is written for XeLaTeX, but
 can be used by any system that supports *fontspec*.

## Installation
### Linux
Save the directory `schl` under `~/texmf/tex/xelatex/`.

## Usage
Load the package in the preable of your document

    \usepackage[greek]{schl}

and use the macros in the `document` environment.

For a quick overview of its use see [schl-tests.tex](). Further examples are in the [`examples`]() directory.

## Contribute
This project is open to contribution. Some of the things you could do are:

- **Use schl**<br/>You could email the maintainer some remarks about it's use.
- **Report issues, errors and bugs.**<br/>If you have a github account, create an *issue*. 
  Otherwise, send an email to the maintainer.
- **Localize the package**<br/>If you 're using /schl/ in a language different than Greek, 
  you could create a file `schl-<you-language>.def` and open a pull request.
- **Write example documents**<br/>
  If you used *schl* in cases that are not similar with those under the directory `examples`, you could
  write a tex document and open a pull request.
- **Help improve the code**<br/>
  Open a pull request with your contribution.
  

## License
[MIT License]()

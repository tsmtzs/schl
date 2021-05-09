# *schl*
## Overview
*schl* is a XeLaTeX  package that provides commands and environments suitable for
document types that appear in a classroom enviromnent. It's development is based on 
the Greek educational practice, but it may be usefull in other contexts also.

Basic macros of the package are:

* Blank space
  * `\lowerdots`: Use dots to designate blank space.
  * `\blankspace`: Use a line for blank space.
* Lists
  * `question, exercise, schltask`: Environments for typesetting questions, exercises and tasks.
  * `multichoice`: An environment for typesetting multiple choice answers.
  * `tickchoice` and `tickchoice*`: `itemize` type lists with a square as symbol for each item.
  * `truefalse` and `truefalse*`: Environments for typesetting true-false type questions.
  * `matchingque`: A macro for typesseting matching questions.
* Answers, solutions, hints...
  * `\answer`: A macro for typesetting  the answer of an exercise.
  * `\solution`: For typesetting the solution of an exercise.
  * `\hint`: Typeset a hint for an exercise.
  * `\deadline`: Set the deadline date.
  * `\remark`: Add a remark to a document.
  * `\reminder`: Write a reminder to a document.
* Headers
  * `\worksheethd`: Set the title of a worksheet.
  * `\examhd`: Set the title of a summative test.
  * `\finalexamhd`: Set the header for end year summative tests.
  * `\theorypart, \exercisepart`: Headers for the theory and exercise parts of a document.
* School information
  * `\school, \headmaster, \teacher, \subject, \grade, \schoolyear, \setdate`
* Macros for tests
  * `\duration`: Set the duration of a test.
  * `\examtime`: Print the time of the exam.
  * `\points`: Set the points of an exercise.
  * `\fullname`: A field that accepts a name.
  * `\datefield`: A field for writing the date.
  * `\schoollogo` Prints school, teacher, grade and subject.
  * `\authoritylogo`: Prints a hierarchy of authorities starting from the Ministry of Education.
  * `\signatures`: A field that prints the name of the teacher or the headmaster. 
  * `\wish`: Prints a wish for good luck.

 By default, *schl* prints all macros that accept text as *undefined*. As of this version, Greek
 is the only full supported language. You can set it with the option `greek`. A partial support for English is provided.  Other languages can be supported by redefining package's internal macros.

## Requirements
 *schl* loads the packages *fontspec, enumitem, calc* and *amsmath*. It is written for XeLaTeX, but
 can be used by any system that supports *fontspec*.

## Installation
### Linux
Save the directory `schl` under `~/texmf/tex/xelatex/`.

## Usage
Load the package in the preable of your document

    \usepackage[greek]{schl}

and use the macros in the `document` environment. 

For a quick overview of the macros see [schl-overview.pdf](schl-overview/schl-overview.pdf). Further examples can be found under the directory [`examples`](examples/).

## Contribute
This project is open to contribution. Some of the things you could do are:

- **Use schl**  
    You could email the maintainer some remarks about it's use.

- **Report issues, errors and bugs.**  
    If you have a github account, create an *issue*. Otherwise, send an email to the maintainer.

- **Localize the package**  
    If you 're using `schl` in a language different than Greek, you could create a file `schl-<your-language>.def` and open a pull request. Follow the 
	template file [schl-template.def](languages/schl-template.def).

- **Write example documents**  
	If you have used `schl` in cases that are not similar with those under the directory `examples`, you could write a `tex` document and open a pull request.

- **Help improve the code**  
  We use the `master` `git` branch for development. Each contribution should be done under a new branch. For code improvements and refinements name 
  branches following the scheme `topic/<someTopic>`. E.x. `topic/refactorSignatures`, `topic/addOverviewDir` etc. For bug fixes name branches as 
  `fix/<whatToFix>`. E.x. `fix/macroAnswer`. Open a pull request with your contribution. 
  

## License
[MIT License](LICENSE)

<!-- -------------------------------------------------------------- -->
<!--							schl							    -->
<!-- A XeLateX package for typesetting classroom related documents. -->
<!-- -------------------------------------------------------------- -->
# Cangelog
Changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased x.y.z] - yyyy-mm-dd
### Added
### Changed
### Removed
### Fixed

## [1.1.0] - 2021-05-09
### Added
- File `schl.ins`.
### Changed
- Macro `truefalselabel` uses a `\makebox` (`schl.dtx` line 182).
- Environment `truefalse*`. Lengths `leftmargin` and `rightmargin` are used to produce	the first line of the output (`schl.dtx` l. 461).
- A `\newcommand` is used to define `\truefalselabel` and `\truefalsesquares`.
### Removed
- The package `mdframed` removed from the dependencies of `schl`.

## [1.0.0] - 2020-06-26
### Added
- `CHANGELOG.md` file.
### Changed
- File `README.md`.
- File `schlNOTES.org`.

## [0.3.1] - 2020-06-23
### Added
- Files `schl-overview/example*.tex`. Each code example  of
`schl-overview/schl-overview.tex` corresponds in an example file.
### Changed
- File `README.md`.
- Improvements in `schl-overview/schl-overview.tex`.

## [0.3.0] - 2020-06-04
### Added
- File `languages/schl-english.def`.
### Changed
- File `schl-tests.tex` renamed as `schl-overview.tex`.

## [0.2.1] - 2020-06-01
### Changed
- Macros refactored: `\answer`, `\points`, `\deadline`, `\duration`,
`\remark` and `\datefield`.

## [0.2.0] - 2020-06-01
### Added
- Macro `\duration`.
- Macro `\remark`.
- Macro `\reminder`.
- Macro `\getdate`.
- Macro `\authority`. Can be used in place of `\authorityi`, `\authorityii`
and `\authorityiii`
- Environment `truefalse*`.
### Changed
- Macro `\worksheettitle` renamed as `\worksheethd`.
- Macro `\examtitle` renamed as `\examhd`.
- Macro `\finalexamtitle` renamed as `\finalexamhd`.
- Macro `\schl@schldate` renamed as `\schl@date`.
- Macro `\schldate` renamed as `\setdate`.
- Macro `\signatures`. A comma seperated list of values can be given as second argument.
### Removed
- Macros `\examdetails` and `\examdetailsii`.
- Macros `\authorityi`, `\authorityii` and `\authorityiii`.


## [0.1.2] - 2019-12-30
### Added
- Macro `\duration@term`.
### Removed
- Option `grmath`.

## [0.1.1] - 2019-11-07
### Added
- New option `grmath`.
- File `grmath.def`.
### Removed
- Greek mathematics operators removed from `languages/schl-greek.def`.

## [0.1.0] - 2019-09-07
### Added
- File schl.dtx.
- File LICENSE
- File README.md
- File examples/endYearTest1.tex.
- File examples/endYearTest2.tex.
- File examples/exercises.tex.
- File examples/exercisesEnglish.tex.
- File examples/myexamdetails.tex.
- File examples/summativeTest.tex.
- File examples/test.tex.
- File examples/worksheet.tex.
- File languages/schl-greek.def.
- File languages/schl-template.def.
- File schl-tests.tex.
- File schl.dtx.
- File schl.idx.
- File schl.ins.
- File schl.pdf.
- File schl.sty.
- File schlNOTES.org.

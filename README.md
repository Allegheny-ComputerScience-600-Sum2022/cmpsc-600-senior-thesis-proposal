# CMPSC 600: Senior Thesis Proposal starter

[![Release Senior Thesis Proposal](../../actions/workflows/main.yml/badge.svg)](../../actions/workflows/main.yml)

This repository contains the starter for the Senior Thesis Proposal document. This
document compiles using GitHub Actions; students should write the entirety of their
document using the [abstract.md](abstract.md) and [proposal.md](proposal.md) files.

The template contains more specific details about using the template. The remainder
of this `README` considers the process of publishing the document via GitHub Actions.

## Introduction

The faculty will reduce a researcher's grade for this assignment if
the pdf of your completed proposal document has not been properly released before the
assignment's due date on `29 June 2022` by `11:59 pm`. Unless
you provide the faculty with documentation of the extenuating circumstances 
that you are facing, no late work will be considered towards your
grade for this project.

## Tagging

Since this repository primarily contains LaTeX source code, the GitHub Actions 
configuration for it will compile the source code and automatically release a
PDF of the main file whenever the last commit is associated with a [Git
Tag](https://git-scm.com/book/en/v2/Git-Basics-Tagging). 

This will build a PDF file available in the "Releases" listing
for this repository. All release numbers for your writing in this repository
should adhere to the [Semantic Versioning](http://semver.org/) standard expected
of GitHub projects. Here this means that:

* `Major version` releases feature a tag number change reflecting full releases; generally these start at `1.0.0`
* `Minor version` releases indicate small changes or additions to documents; typically these increment the second digit in the version (e.g. `1.1.0`)

Please note that your readers will only read the PDF generated from "tagged" releases 
of the file `SeniorThesisProposal.pdf` that has a version number greater than
1.0.0. 

That is:

* if your commit is tagged `SeniorThesisProposal-chompers-1.0.0`, then 
* the file `SeniorThesisProposal.pdf` should be available for download in the "Releases" tab in your GitHub repository for this project under the name
`SeniorThesisProposal-chompers-1.0.0`.

To ensure you can create a release appropriately, make a single small change to the
`SeniorThesisProposal.tex` and:

1. `commit` your file using a `git commit` command
2. create your first tag for this repository: type `git tag senior_thesis_proposal-YOUR_USERNAME-0.1.0`. 
3. You are now ready to push your changes with the tag number using  `git push -u origin main --tags`

The above steps should build a version of your project.

When you make subsequent changes to your files and perform commits and you are
ready to release a new version of `SeniorThesisProposal.pdf`, then you should
again tag your work _before a `push` command_ with a tag that
adheres to the [Semantic Versioning](http://semver.org/) standard. 

Each time that you correctly execute this sequence of commands you will release a new
version of your document to GitHub that is easily accessible as a PDF to you and
to your first and second readers.

## Updates

If a course instructor updates the provided material for this assignment and
you would like to receive these updates, then you can type this command in the
main directory for this assignment:

```
git remote add download git@github.com:Allegheny-ComputerScience-600-Sum2022/cmpsc-600-senior-thesis-proposal.git
```

You should only need to type this command once; typing the command additional
times may yield an error message but will not negatively influence the state of
your repository. Now, you are ready to download the updates provided by the
course instructor by typing:

```
git pull download main
```

This second command can be run whenever the faculty need to provide you
with new source code for this assignment. However, please note that, if you have
edited the files that the course instructor updated, running the previous
command may lead to Git merge conflicts. If this happens, you may need to
manually resolve them with the help of the instructor or a teaching assistant.

## Problems

If you have found a problem with this assignment's provided source code, then
you can go to the [Computer Science 600 Proposal
Starter](https://github.com/Allegheny-ComputerScience-600-Sum2022/cmpsc-600-senior-thesis-proposal)
repository and create an issue by clicking the "Issues" tab and then clicking
the green "New Issue" button. To ensure that your issue is properly resolved,
please provide as many details as is possible about the problem that you
experienced.

Students who find, and use the appropriate GitHub issue tracker to correctly
document, a mistake in any aspect of this laboratory assignment will receive
free laptop stickers and extra credit towards their grade for it.

## Assistance

If you are having trouble completing any part of this project, then please talk
with your first reader. In particular, if you have questions about your research project, please
see your first reader. Alternatively, you may ask questions of your first or second reader.

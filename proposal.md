# Template description

Your training in the conduct of research includes learnining to prepare a 
concise, 
rigorous, scholarly thesis proposal; you will also present it. While There is no
strict length requirement for the senior thesis proposal, faculty anticipate 
that 
most students will need about twenty pages of text to adequately explain the 
motivation and goals of their project, review the relevant literature, and 
describe the feasibility of the proposed work. 

The template specifies various settings in the `config.yaml` file included in 
the
repository. Change the appropriate values under the `Project-specific values` 
heading. Changing other values outside of that section may cause the project to
fail to build. **Modify these values at your own risk.**

Author your proposal in the `proposal.md` document using appropriate markdown
hierarchy and syntax; GitHub Actions will automatically create a PDF from the
`abstract.md` and `proposal.md` files. Consult the `README` of the proposal
repository to learn how to properly build and release this PDFs.

Including references throughout requires a specific pseudo-Markdown tag, 
demonstrated in the following blockquote. (Inspect the `proposal.md` file to 
see the format.)

> A citation, when included correctly, will appear as it does at the end of this
> sentence. [@plaat1996research]

These sources must be added in `bibtex` format to the `references.bib` file for
citation and referencing to occur.

To label a figure (i.e. an image), referencing the image using correct Markdown
will automatically caption the figure:

```markdown
![Label](images/IMAGE_NAME.png)
```

Two things specific to this template to also keep in mind:

1. It is your responsibility to remove this description section before building
the PDF version you plan to defend.
2. References _will only appear if cited correctly_ in the text

## Note on `LaTeX` commands

Documents may include specific `LaTeX` commands _in Markdown_. To render these, surround the commands
with markup denoting `LaTeX`. For example:

```
Checkmark character:   $\checkmark$
Superscript character: $^{\dag}$
``` 

If using a special package not included in the template, add the desired `LaTeX`
package or command/macro to the `header-includes` property in [config.yaml](config.yaml).

Should this package not be included in the environment shipped with this template,
you may also need to add the package to the [GitHub Actions Workflow](.github/workflows/main.yml).

Direct any questions about issues to your first reader.

# Introduction

This section should include a statement of the problem, the overall aims, and 
the background motivating your research. Whenever possible, you should use one 
or more concrete examples
and technical diagrams.

# Related work

This section should include a statement of the problem, the overall aims, and 
the background motivating your research. Whenever possible, you should use one 
or more concrete examples
and technical diagrams.

# Method of approach

This section should answer the "how" question - how will you perform the 
proposed research. It should also describe the feasibility study you have 
conducted to demonstrate that your project is feasible. Use technical diagrams, 
equations, algorithms, and paragraphs of text to describe the research that you 
intend to complete. Be sure to number all figures and tables and to explicitly 
refer to them in your text.

# Evaluation strategy

This section should explain what steps you will take to evaluate your proposed 
method. If you intend to conduct experiments, then you must clearly define your 
evaluation metrics.

# Research schedule

This section identify the main phases and tasks of your research project and 
set deadlines for when you will be able to complete each of these items. Please 
remember that you should aim to complete the project before the middle of March.

# Conclusion

Provide a summary of your proposed research and suggest the impact that it may 
have on the discipline of computer science. In addition, this section should
discuss potential ethical implications or harms which arise from pursuing or
implementing this project. This is your opportunity to think ahead and
contemplate potential misuse or other impacts that any project implies -- no 
matter how seemingly benign.

If possible, you may also suggest some areas for future research.

# References

::: {#refs}
:::

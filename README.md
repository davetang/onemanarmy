## Table of Contents

  - [README](#readme)
  - [General tips](#general-tips)
  - [Linux administration](#linux-administration)
  - [Software development](#software-development)
  - [Programming/scripting](#programmingscripting)
  - [Analysis](#analysis)
    - [Bioinformatics](#bioinformatics)
  - [Misc](#misc)

## README

In most cases, a team of people with different areas of expertise working
together is ideal. More often than not, things goes awry and you just have to
deal with it. This means learning a new set of skills and learning how to work
more efficiently to cope with a lack of a full team. Below are my notes (except
for the last link) on various things I have learned and am continually learning
about.

## General tips

[Trust, but verify](https://en.wikipedia.org/wiki/Trust,_but_verify).

When you have a computational problem to solve, look _extensively_ to see if a
tool already exists that can help you solve your problem. Chances are that a
tool already exists. If a tool does not do exactly what you need, try to break
your problem down into separate parts and use the tool for the sub-problem. Do
not implement your own tool unless it is absolutely necessary.

Similar to the point above, don't start from scratch either. Use a standard
template or layout. This not only saves time but helps you become more
systematic since you are using the same template/layout for your work.

Be systematic. For example, over the years I've started to accumulate more and
more junk at home and I find myself searching for things more often. Where'd I
put the USB-C to HDMI cable!? Where's my 3.5mm audio cable extension cord!?
Finally I got sick of searching for stuff and organised everything in a
systematic way. This applies computationally too. Where's that R function I
wrote for checking if a package is installed!? Where's that analysis I did!?
Organise your functions into a single file or package it. Organise your
analysis files using some directory structure.

When you perform an analysis, try to make the analysis self-contained, which
the Cambridge dictionary defines quite nicely: "containing or having everything
that is needed within itself". Another user (e.g. yourself on another computer)
should be able to clone/copy your analysis, run it, and produce the same
results.

_Always_ try to script everything you do! No pointing and clicking. Use APIs
and command-line tools. (I don't even use a mouse, unless I really need to,
like when a website annoyingly does not work with
[vimium](https://github.com/philc/vimium).)

There's always a better way to do something. If you find yourself continually
doing something inefficiently, it is time to find a better solution.

Focus on results but revise/refactor your code later on when the deadline has
been met! Chances are that you will have to revisit your code that you wrote in
a hurry and it will probably make less sense later compared to when you wrote
it.

## Linux administration

* [Linux networking](https://github.com/davetang/learning_linux/blob/main/networking.md)
* [Debugging with strace](https://github.com/davetang/learning_linux/blob/main/strace.md)
* [Troubleshooting systems](https://github.com/davetang/learning_linux/blob/main/trouble.md)
* [Looking at system logs](https://github.com/davetang/learning_linux/blob/main/logs.md)

## Software development

* [GNU Make](https://davetang.org/muse/2015/05/31/learning-about-makefiles/)
* [DevOps](https://github.com/davetang/learning_linux/blob/main/devops.md)
* [Know how to use Git](https://github.com/davetang/getting_started_with_git)
* [Know how to use Docker](https://github.com/davetang/learning_docker)
* [Know how to use Singularity](https://github.com/davetang/learning_singularity)
* [Run RStudio Server using Docker](https://davetang.org/muse/2021/04/24/running-rstudio-server-with-docker/)

## Programming/scripting

* [Use Bash more effectively](https://github.com/davetang/learning_bash)
* [Learning how R works](https://github.com/davetang/learning_r)
* [Learning how Python works](https://github.com/davetang/learning_python)
* [Learning how C works](https://github.com/davetang/getting_started_with_c)
* [Learning how Rust works](https://github.com/davetang/learning_rust)
* [Learning how Ruby works](https://github.com/davetang/learning_ruby)
* [Data structures](https://davetang.github.io/bioinformatics_tips/data_struct.html)
* [Writing command line scripts](https://davetang.github.io/bioinformatics_tips/get_option.html)
* [Running R in parallel](https://davetang.github.io/muse/parallel.html)

## Analysis

* [Machine learning](https://github.com/davetang/machine_learning)
    * [Random Forest](https://github.com/davetang/learning_random_forest)
    * [Evaluate models](https://github.com/davetang/machine_learning/tree/main/evaluation)
* [Make a heatmap](https://davetang.github.io/muse/pheatmap.html)
* [Make a complex UpSet plots](https://davetang.github.io/muse/complex_upset.html)
* [Investigate how PCA works](https://davetang.github.io/muse/pca.html)

### Bioinformatics

* Analyse DNA-seq data
    * [Part 1](https://davetang.org/muse/2015/07/24/dna-sequencing-data/)
    * [Part 2](https://davetang.org/muse/2015/12/16/getting-acquainted-analysing-dna-sequencing-data/)
    * [Assessing genetic variants](https://davetang.org/muse/2016/10/31/assessing-genetic-variants/)
* [Carrying out reproducible bioinformatics](https://github.com/davetang/reproducible_bioinformatics)
* [Work with VCF files](https://github.com/davetang/learning_vcf_file)
* [Work with BAM files](https://github.com/davetang/learning_bam_file)
* [Analyse RNA-seq data](https://github.com/davetang/rnaseq)
* [Investigate multimapping reads](https://github.com/davetang/multimapping)
* [Analyse SARS-CoV-2](https://github.com/davetang/sars_cov_2)
* [Work with genomic regions](https://github.com/davetang/defining_genomic_regions)
* [Learning how WDL works](https://github.com/davetang/learning_wdl)
* [Working with an ontology (HPO)](https://github.com/davetang/human_phenotype_ontology)
* [Learn how to use Nextflow](https://github.com/davetang/learning_nextflow)
* [Learn how to download publicly available data](https://github.com/davetang/research_parasite)

## Misc

* [Using LaTeX](https://github.com/davetang/getting_started_with_latex)
* [Best Practices](https://berkeleybop.github.io/best_practice/) of the
  Berkeley Bioinformatics Open-source Projects (BBOP), which is based on the
  [best practices](https://github.com/knocean/practises) of Knocean.

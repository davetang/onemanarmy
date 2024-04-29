## Table of Contents

  - [README](#readme)
  - [General tips](#general-tips)
  - [The Pragmatic Programmer](#the-pragmatic-programmer)
    - [Your Knowledge Portfolio](#your-knowledge-portfolio)
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
it. Be disciplined with your coding.

Sometimes the hardest part to doing something is simply getting started. Here's
a tip I learned from [Marilyn vos
Savant](https://en.wikipedia.org/wiki/Marilyn_vos_Savant) a long time ago:
simply make a promise to yourself that you will work on that dreaded task for 5
minutes. More often than not, you will find yourself working for more than 5
minutes. And even if you stop after 5 minutes, you won't feel bad and you got 5
minutes of work done after all, which is better than nothing.

## The Pragmatic Programmer

The Pragmatic Programmer, typically has the following characteristics:

* Early adopter/fast adapter - instinct for tech and methodology with a passion
  for trying new things. Able to distill new things and integrate it.

* Inquisitive - tend to ask questions.

* Critical thinker - rarely take things as given.

* Realistic - understand the nature of a problem and can estimate how long a
  task will take to complete.

* Jack of all trades - familiar with broad range of tech and strive to keep on
  top of new developments.

* Care about your craft - you can only do good work when you care about your
  work.

* Think about your work - ongoing critical appraisal of every decision made
  every day and on every project.

Being a Pragmatic Programmer will help to provide you with a more active
involvement with a job you enjoy, a feeling of mastery over an increasing range
of subjects, and continuous improvement.

The Pragmatic Programmer sees the bigger picture and thinks beyond the
immediate problem, placing it in its larger context. Without the bigger
picture, it is difficult to be pragmatic and to make intelligent compromises
and informed decisions. For example, by understanding the context, you can
decide just how good your software needs to be. Sometimes near-perfection is
necessary but often times you can make trade-offs. This idea is called
good-enough software but it does not imply writing poor code. It simply
advocates that the produced code is good enough for the necessary requirements.
For example, you can trade-off adding new features or further polishing up code
so that other constraints are met. The scope and quality requirements should be
discussed at the beginning of a project.

One of the main philosophy of being pragmatic is the idea of taking
responsibility for yourself: you are in control of your career advancement,
your learning and education, your project, and your day-to-day work.
Furthermore, when you accept responsibility for something, you should expect to
be held accountable for it. When you do make a mistake or an error in judgement
(inevitably), admit it honestly and try to offer options. Don't blame because
while something else may have played a role in the mistake/error, it is up to
  _you_ to provide solutions and not excuses. If there was a risk, you should
  have made a contingency plan.

### Your Knowledge Portfolio

All the facts about programming, the application domains, and experience
constitute the _knowledge portfolio_. Managing a knowledge portfolio is very
similar to managing a financial portfolio:

1. Serious investors invest regularly as a habit (even if it is a small
   amount).
2. Diversification (know more different things) is the key to long-term
   success.
3. Smart investors balance their portfolios between conservative and high-risk,
   high-reward investments. Don't invest all your time on high-risk tech that
   might collapse suddenly nor invest too conservatively and miss out on
   possible opportunities.
4. Investors try to buy low and sell high for maximum return. Learning an
   emerging technology before it becomes popular can be just as hard as finding
   an undervalued stock but the payoff can be just as rewarding. Learning Java
   back when it was first introduced may have been risky but it paid off as it
   became an industry mainstay.
5. Portfolios should be reviewed and rebalanced periodically. The tech industry
   is very dynamic and last month's hot tech might be stone cold now.

The most important point is to invest regularly in your knowledge portfolio.

### The Essence of Good Design

Every design principle is simply a special case of the ETC principle: Easier To
Change. For example, decoupling is good because by isolating concerns, we make
code easier to change. The single responsibility principle is useful because a
change in requirements is mirrored by a change in just one module.

When making changes, asking yourself whether the change made the overall system
easier or harder to change. While it can be subjective on whether something is
easier or harder to change, most times common sense will be correct. If you're
not sure, make sure that your implementation can be replaceable, which is what
you should be doing all the time anyway.

The only way to develop software reliably and to make developments easier to
understand and maintain is to follow the DRY (Don't Repeat Yourself) principle:

>Every piece of knowledge must have a single, unambiguous, authoritative
representation within a system.

DRY is about the duplication of _knowledge_, of _intent_. It is about
expressing the same thing in two different places, possibly in two totally
different ways.

### Orthogonality

Orthogonality is a critical concept that can help produce systems that are easy
to design, build, test, and extend. In geometry, two lines are orthogonal if
they meet at right angles, such as the axes on a graph. In vector terms, the
two lines are _independent_.

In computing, the term is associated with a kind of independence or decoupling.
Two or more things are orthogonal if changes in one of not affect any of the
others. In a well-designed system, the database code will be orthogonal to the
user interface: changing one will not affect the other.

Non-orthogonal systems are inherently more complex to change and control. When
components of any system are highly interdependent, there is no such thing as a
local fix.

The concept of orthogonal systems can also be described as being modular,
component-based, and layered. Systems should be composed of a set of
cooperating modules, each of which implements functionality independent of the
others. Sometimes these components are organised into layers, each providing a
level of abstraction.

To test for orthogonal design, ask: "If I dramatically change the requirements
behind a particular function, how many modules are affected?". In an orthogonal
system, the answer should be one. Also ask yourself how decoupled your design
is from changes in the real world. For example, are you using telephone numbers
as identifiers? What happens when the phone company reassigns area codes? **Do
not rely on the properties of things you cannot control**.

## Linux administration

* [Linux networking](https://github.com/davetang/learning_linux/blob/main/networking.md)
* [Debugging with strace](https://github.com/davetang/learning_linux/blob/main/strace.md)
* [Troubleshooting systems](https://github.com/davetang/learning_linux/blob/main/trouble.md)
* [Looking at system logs](https://github.com/davetang/learning_linux/blob/main/logs.md)
* [Using Ansible for provisioning](https://github.com/davetang/learning_ansible)
* [Using AWS](https://github.com/davetang/learning_aws)

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
* [Learning to use Vim effectively](https://github.com/davetang/learning_vim)
* [Best Practices](https://berkeleybop.github.io/best_practice/) of the
  Berkeley Bioinformatics Open-source Projects (BBOP), which is based on the
  [best practices](https://github.com/knocean/practises) of Knocean.

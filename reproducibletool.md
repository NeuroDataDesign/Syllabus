# Open And Reproducible Tools

The gold standard for a reproducible tool does not only mean that the tool can reproduce the same results given the same data on multiple occassions or systems, but also that:

1. its setup is thoroughly documented
2. its use/execution is thoroughly documented
3. it contains descriptions of expected behaviour
4. it is transparent what is happening "under the hood"

In fact, thorough and clear documentation is often as important as the tool itself. As such, we wish to elaborate on this list of requirements for a tool's documentation in order for us to consider it to be of sufficient detail. It is worth noting: everything enumerated below **must** be web viewable from outside of your tool (i.e. docstrings within the code or instructions only viewable once a web service are good supplements, but not sufficient).

1. **setup is thorougly documented** (i.e. [example](https://github.com/NeuroDataDesign/orange-panda/blob/1351425c5eacbdd407ef50684dad57dbd95de4b3/README.md))
  - setup instructions should be in the form of a *step-by-step* guide that are viewable within the web
  - instructions should live on a documentation page for the tool, (i.e. sphinx docs for a github project), within the code repo itself
  - instructions may be shared and available elsewhere (i.e. docker hub), but the external instructions are **not sufficient**
  - if applicable, screenshots should be included in the instructions (i.e. if there are visual steps/interfaces involved)

2. **its use/execution is thorougly documented** (i.e. [example part 1](https://github.com/NeuroDataDesign/orange-panda/blob/1351425c5eacbdd407ef50684dad57dbd95de4b3/README.md), [example part 2](http://54.88.116.242/#/flow))
  - demonstration data (taking < 10, preferably 3-5 min to process) provided and explained
  - description of the commands/steps being run, how to run them, and why you're running them
  - description of the time it takes to run each step

3. **it contains descriptions of expected behaviour**
  - description of input data to each step, and derivatives at each step
  - visualization of each derivative after an algorithm has been run (both produced by the tool and in the documentation for the demo data)
  - quantitative analysis/result of the outputs when using the demo data

4. **it is transparent what is happening "under the hood"** (i.e. [example](http://54.88.116.242/#/flow))
  - flowchart of contents of pipeline
  - pseudocode for algorithms being deployed
  - explanation of the purpose of using each algorithm as well as an analysis of the efficacy of the algorithm at accomplishing that purpose

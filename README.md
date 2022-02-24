# tutorial-template

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ProjectPythiaTutorials/tutorial-template/HEAD)

The Project Pythia Tutorials organization is designed to be a single place to store all content for Project Pythia's Python Tutorial Seminar Series. Each tutorial seminar will have its own repository within this organization to house tutorial content (notebooks, data, and markdown).


## Overview 

The goal of this organization is to create a common location and environment for Pythia Python tutorials. For the Python learner, this has the benefits of more consistent installation / spin up before jumping in to each lesson. For the Pythia team, this ownership allows us to maintain content long-term so that we can fix things when they break or archive it, as we see fit.

We, the Pythia team, want to lower the barrier of entry for the tutorial speaker to develop and host their tutorial content in this organization. For the speaker's convenience we will provide a simple repository template from which a new repository can be modeled. These new repositories differ from the [pythia-foundations book](https://foundations.projectpythia.org/landing-page.html), which has a high barrier for entry, with its strict and consistent style guide and rigorous review process before merging. Further, the tutorial notebooks in this this organization's repositories are designed to be accompanied by a live speaker or recording. This means that the amount of explanatory text between code cells or excercises may differ between tutorials based on the tutorial speaker and developers' preferred styles.

All tutorials are designed to be hosted on [Binder](https://mybinder.org/v2/gh/ProjectPythiaTutorials/tutorial-template/HEAD) where appropriate.

## Organization
The document tree of each tutorial repositories takes the following format:

```
  TOPIC_YYYY_MM_DD/
   |-  data/
   |    |- `some_data.txt`
   |- tutorial/
   |    |-  `topic_a.ipynb`
   |    |-  `topic_b.ipynb`
   |-  `README.md`
   |-  `environment.yaml`
 
```

Some things to notice:
- Store any necessary data in a `data` directory. If your dataset is too large for GitHub (100 MB limit per file), make a note of its location and how to access it (both remotely and locally) in your repository's `README.md` as well as a `/data/README.md`.
- Within the `tutorials` directory there is a unique directory for every tutorial and a `template` directory, containing a markdown and a notebook template (coming soon). 
- Each tutorial repository is named with its topic and date with the format `TOPIC_YYYY_MM_DD` (e.g.`pandas_2021_08_03`)
- If a new tutorial on the same topic is contributed, a new repository with the new date is added (i.e. the pre-existing repository is not edited). 
- Multi-session tutorials may have a repository directory for each session, preserving the state of the tutorial during each lesson (e.g. `matplotlib_part1_YYYY_MM_DD` and `matplotlib_part2_YYYY_MM_DD`), but multiple notebooks may be presented during a single tutorial (and thus housed in the same repository).
- Each tutorial directory contains a `README.md` file. This `README.md` file should contain all pertinent information that will not be part of the tutorial presentation (e.g. preparation steps, past videos to watch beforehand, and the embedded recording from the tutorial ala the [ESDS blog posts](https://ncar.github.io/esds/blog/)). This should mimic the `README_template.md` file within this repository.
- There is a single environment file for each tutorial repository.

## Contribution

For instructions on how to add your tutorial repository to this organization please visit `contributing.md`.

If you would like to host a tutorial through the Project Pythia Tutorial Seminar Series, please reach out to us here on GitHub via a new issue or by emailing `projectpythia@ucar.edu`.

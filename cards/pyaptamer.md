### Open Source AI for drug discovery

Build open source AI for drug discovery, accelerating aptamer design for diagnostic and medical applications!

#### project summary

Aptamers are highly specific biomolecules, which can pave the way for individualised diagnostics and therapy, allowing personalized treatment of various diseases like cancer, infections or autoimmune disorder. Classically done through in-vitro (lab) experiments, AI-driven in-silico approaches have seen promising advances, fuelled by the success of AlphaFold.

In ESoC 2025, the package `pyaptamer` has been built in collaboration between ecoSPECS and the German Center for Open Source AI, to enable easy use of AI based in-silico aptamer generation.

Join ecoSPECS and the German Center for Open Source AI in this exciting continuation of the successful 2025 project!

#### About ecoSPECS

[ecoSPECS](https://ecospecs.de/en/) is a German engineering service provider, specializing in services such as qualification, validation, consulting, training, and project planning across various industries, with a focus on pharmaceuticals, engineering, and food production.

#### Technical goals and datasets

Aptamer design is a promising approach for personalized diagnostics and therapeutics – including targeted drug delivery to cancer cells, microbial pathogens or interference with other biochemical pathways, e.g. for immunomodulation .

Recent research has seen an explosion of in-silico approaches that is, computer based simulation, driven by a combination of biochemical simulation and modern AI models, inspired by AlphaFold.

While the body of research and successes keeps growing, the research software ecosystem has not kept up with the advances – software and data are scattered, non-interoperable, often requiring undocumented, idiosyncratic and highly manual operator knowledge. There are also no publicly available, standardized benchmark datasets or challenges to test the performance of in-silico aptamer design procedures.

In turn, this prevents application of modern AI technologies in the vein of AlphaFold, which require clear software APIs, consistent data formats, and readily available training data.

ecoSPECS and the German Center for Open Source AI have teamed up in 2025 to create an easily usable, open source software ecosystem for researchers, with the ultimate goal to enable the easy creation of open source AI approaches - resulting in the `pyaptamer` package that is now maintained by a team of developers at ecoSPECS and GC.OS.

Primary goals of the `pyaptamer` project are the design and implementation of open source tooling for a number of state-of-art algorithms, benchmarks, and data repositories under a consistent API, which in turn enables developing state-of-art open source AI approaches for the task of in-silico aptamer design.

On the 2026 roadmap we want to add (or develop) state-of-art algorithms, robustify the API, and increase interoperability, see issue tracker:
https://github.com/gc-os-ai/pyaptamer/issues

Stretch goals – based on speed and success – may include testing and validation of the AI based approaches in a laboratory setting with partners of ecoSPECS in the academic or commercial biopharma space.

Join this project for a unique opportunity to revolutionize ligand development with AI!

### pyaptamer project ideas

In ESoC 2025, the `pyaptamer` package was developed through a collaboration between ecoSPECS and the German Center for Open Source AI to support the easy use of AI-based in silico aptamer generation.

Below are ideas for potential projects for ESoC 2026.

#### Application Prerequisites

These warm-up projects are intended to help applicants become familiar with the `pyaptamer` library. To apply for one of the European Summer of Code 2026 full projects, applicants should first gain familiarity with the library and open at least one substantial pull request, either fixing a bug or contributing a meaningful feature enhancement. The pull request does not need to be merged by the time the application is reviewed.

Applicants are also encouraged to actively use the library and identify bugs or usability issues that may have been missed by contributors. We expect potential applicants to communicate before taking on issues and opening pull requests. For simpler issues, a brief note is sufficient; for more complex ones, we expect a more detailed implementation plan.

The use of AI is permitted. However, relying on automated AI agents, or opening multiple pull requests or issues without verifying their output, may negatively affect an application.

#### Full 2026 Projects

##### Adding the AptaDiff Algorithm

Currently, the suite includes two algorithms, and we would like to expand the algorithmic coverage of the `pyaptamer` repository. This project involves adapting the [AptaDiff](https://github.com/wz-create/AptaDiff) algorithm from scratch to follow the scikit-learn-style API and the existing public API conventions of `pyaptamer`, together with appropriate test coverage.

Goals:

* develop the `pyaptamer.aptadiff` API and integrate it with the current `MoleculeLoader` data loader
* write tests for the implementation
* create a notebook demonstrating the public API on existing and new datasets

**Expected Time**: 300 hours<br>
**Difficulty Rating**: Hard<br>
**Required Skills**: Python, familiarity with deep learning, PyTorch, Lightning, and scikit-learn<br>

##### Adding the DeepAptamer Algorithm

We would also like to expand the algorithmic coverage of the `pyaptamer` repository by adapting [DeepAptamer](https://github.com/TMBJ-lab/DeepAptamer) to follow the scikit-learn-style API and the current public API conventions, together with tests.

For more details, refer to these discussions: [#98](https://github.com/gc-os-ai/pyaptamer/pull/98) and [#110](https://github.com/gc-os-ai/pyaptamer/issues/110)

**Expected Time**: 250 hours<br>
**Difficulty Rating**: Hard<br>
**Required Skills**: Python, familiarity with deep learning, PyTorch, Lightning, and scikit-learn<br>

##### Redesigning the Public and Internal API

As pyaptamer continues to grow with the addition of more algorithms, we would like to standardize the public API and refactor the internal architecture to improve maintainability and align the library more closely with the design principles of sktime and scikit-learn. This project includes work on the data loader, a generalized dataset object, and reusable transformation utilities.

Goals:

* standardize the public API across existing and future algorithms
* refactor internal interfaces to improve maintainability and extensibility
* improve and consolidate the data loading pipeline
* support a generalized dataset object for broader dataset handling
* design and integrate reusable transformation utilities


For more details, refer to these discussions: [#259](https://github.com/gc-os-ai/pyaptamer/pull/259), [#441](https://github.com/gc-os-ai/pyaptamer/pull/441), and [#174](https://github.com/gc-os-ai/pyaptamer/issues/174)

Expected Time: 250 hours<br>
Difficulty Rating: Medium<br>
Required Skills: Python, software design, API design, familiarity with scikit-learn and sktime-style interfaces<br>

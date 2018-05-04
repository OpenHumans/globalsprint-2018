---
layout: post
title:  "Personal Data Notebooks"
date:   2018-05-03 10:36:41 -0700
categories: jekyll update
---
![](https://img.shields.io/badge/difficulty-easy-brightgreen.svg?longCache=true&style=flat) -
![](https://img.shields.io/badge/difficulty-intermediate-yellow.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Python-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-R-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Julia-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/other-Documentation-blue.svg?longCache=true&style=flat)
<br/>
Open Humans runs it's own *JupyterHub* setup which allows people to explore their
personal data in notebooks written in *Python*, *R* and *Julia*. We are looking for
people to write more example notebooks and improve our documentation!

You can [find our example notebook documentation here](http://openhumansfoundation.org/ohjh-example-notebooks/).
The Notebooks [themselves can be found at GitHub](https://github.com/OpenHumans/ohjh-example-notebooks)
too and the notebooks found in the `master` branch of that repository are automatically
provided to each user's notebook server when they start it. This makes it a great
way to showcase your notebooks to many people who are just getting started!

Some new notebook ideas and improvement ideas can be found below and
[in the issues on GitHub](https://github.com/OpenHumans/ohjh-example-notebooks/issues).
To add your own notebook or improvements to existing notebooks just make a pull
request against that repository!

A general reminder for the *perceived difficulty*: If you are writing a notebook
on you own, the difficulty level is highly dependent on the kind of data analysis you want to perform in your notebook.
It could *"just"* be plotting some of the data that people have in their Open Humans
accounts. Or it could be a more complex task that correlates data sources, makes use
of external APIs etc. It's completely up to you.

All the ideas here are just some suggestions to get your own creativity going. 😊

## Ways to contribute

- [Check & extend the documentation](#check--extend-the-documentation)
- [Extend existing notebooks](#extend-existing-notebooks)
- [Write notebooks for other data sources](#write-notebooks-for-other-data-sources)
  * [Writing notebook that explore Runkeeper](#writing-notebook-that-explore-runkeeper)
  * [Writing notebook that explore Moves](#writing-notebook-that-explore-moves)
  * [Writing notebooks that explore genetic data](#writing-notebooks-that-explore-genetic-data)

## Check & extend the documentation
![](https://img.shields.io/badge/difficulty-easy-brightgreen.svg?longCache=true&style=flat)
The *Personal Data Notebooks* have been released only 3 weeks ago. As a consequence
the documentation is still rather new and not well tested. There are some ways you can
test and extend the documentation:

- [Follow the getting started guide](http://openhumansfoundation.org/ohjh-example-notebooks/) for
the notebooks and see whether anything is missing. If things are missing or unclear you can
[propose changes to the README.md](https://github.com/OpenHumans/ohjh-example-notebooks/blob/gh-pages/README.md)
- [Each of the example notebooks](https://github.com/OpenHumans/ohjh-example-notebooks) comes with inline comments
about what is done and more or less how it works. Are these useful and correct? If not you can edit them in your own notebook instance, download the fixed notebook and make a pull request.

## Extend existing notebooks
![](https://img.shields.io/badge/difficulty-easy-brightgreen.svg?longCache=true&style=flat) -
![](https://img.shields.io/badge/difficulty-intermediate-yellow.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Python-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-R-blue.svg?longCache=true&style=flat)

Our [existing notebooks](https://github.com/OpenHumans/ohjh-example-notebooks) explore
data from **Fitbit**, **Apple Healthkit** and **Twitter archives**. Some of these analyses are rather basic
at this point.

If you have an interest in extending these notebooks - or are inspired to write your own analyses for these data types -
please go ahead. Some potential ideas:

- Extend the Twitter sentiment analysis to:
  - Which emoji are most often used with the top-people a person replies to?
  - Are there changes in tweets between weekdays & weekends?
- Extend Fitbit/HealthKit:
  - Is there a clear correlation between elevation gains/flights climbed and step counts?
  - Is there a linear relationship between the distances in miles/kilometer and the step counts?

## Write notebooks for other data sources

### Writing notebook that explore Runkeeper
![](https://img.shields.io/badge/difficulty-easy-brightgreen.svg?longCache=true&style=flat) -
![](https://img.shields.io/badge/difficulty-intermediate-yellow.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Python-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-R-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Julia-blue.svg?longCache=true&style=flat)

*Runkeeper* allows people to track their runs and workouts - along with GPS
information. Right now around 200 people have connected their *Runkeeper*
accounts to Open Humans ([see some of the public data sets here](https://www.openhumans.org/api/public-data/?source=direct-sharing-140)).

Here are some ideas for notebooks that use Runkeeper data:
- Basic ideas:
  - generate basic statistics of the data (yearly distance run? Minutes spent working out)
  - visualize the GPS tracks so that people can "re-run" their experiences (`ggplot2` for `R` makes this rather easy, but any other language works too!)
  - advanced: Use the GPS data to get weather information from some 3rd party API and try to correlate if the workout frequency etc. is tied to the weather

### Writing notebook that explore Moves
![](https://img.shields.io/badge/difficulty-easy-brightgreen.svg?longCache=true&style=flat) -
![](https://img.shields.io/badge/difficulty-intermediate-yellow.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Python-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-R-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Julia-blue.svg?longCache=true&style=flat)

*Moves* is a passive GPS application for *iOS* and *Android* that records you movement history.
Besides logging your location it will also try to classify your mode of transportation.
Around 100 people have already connected their Moves accounts to Open Humans and we have
[some public data sets as well](https://www.openhumans.org/api/public-data/?source=direct-sharing-138).

Some ideas for notebooks that use Moves data:
- Visualize the movement patterns over time (`ggplot2` for `R` makes this rather easy, but any other language works too!)
- Analyze as a time series:
  - Do certain movement types (driving a car, public transport, walking, …) fluctuate over time?
  - Are there seasonal changes to these modes of movement? Differences between weekday/weekends?
- advanced: Use the GPS data to get weather information from some 3rd party API and try to correlate if the workout frequency etc. is tied to the weather

### Writing notebooks that explore genetic data
![](https://img.shields.io/badge/difficulty-intermediate-yellow.svg?longCache=true&style=flat) -
![](https://img.shields.io/badge/difficulty-hard-red.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Python-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-R-blue.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/language-Julia-blue.svg?longCache=true&style=flat)

Open Humans hosts genetic data from a variety of sources:
- [23andMe](https://www.openhumans.org/activity/23andme-upload/)
- [AncestryDNA](https://www.openhumans.org/activity/ancestrydna-upload/)
- [Gencove](https://www.openhumans.org/activity/gencove/)
- [Generic VCF data](https://www.openhumans.org/activity/genomeexome-upload/)
- [FamilyTreeDNA](https://www.openhumans.org/activity/familytreedna-integration/)
- [uBiome microbiome data](https://www.openhumans.org/activity/ubiome-upload/)

These data are a bit harder to analyse, especially if you don't have a background in biology/bioinformatics.
With the exception of *uBiome* all of these data sources contain genetic variants called *SNPs* (single nucleotide polymorphisms).
One way to explore these variants would be to use an external API such as [http://myvariant.info/](http://myvariant.info/) to
annotate them with metadata. Metadata could be variant frequencies in different populations, whether variants are coding or not.
Alternatively you could try to use databases to predict phenotypic information such as hair or eye colour.

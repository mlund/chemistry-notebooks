# Faunus Lab

This is a lab for getting started with the simulation package [Faunus](https://faunus.readthedocs.io).

## Getting started

1. Install [Docker Desktop](https://www.docker.com/products/docker-desktop) (Mac, Windows, Linux, ...)
2. Start Docker
3. In a terminal, run `docker run -it -p 8888:8888 mikaellund/faunus:v2.11.0`
4. Copy the generated link, _e.g._ `http://127.0.0.1:8888...`, into a web-browser.
   This loads a _Jupyter Notebook_ environment - here's
   [one of many](https://www.youtube.com/watch?v=jZ952vChhuI) introductory videos for how to use it.

### Expert mode (not recommended)
If you are more adventurous, you may also install Jupyter Notebook and Faunus
on your local system by the following commands, assuming you have anaconda or miniconda installed:

~~~ bash
git clone https://github.com/mlund/chemistry-notebooks
cd chemistry-notebooks
conda env create -f environment.yml
source activate LUchem
jupyter-lab
~~~

## Topics

Pair up or work individually.
You are free to pick a system of interest from e.g. the
[faunus example folder](https://github.com/mlund/faunus/tree/master/examples) or of your own choice.
But I also have some suggestions:

- The water example (isobaric ensemble, density, effect of dipolar strength, freezing?).
  [Initial Notebook exists](https://github.com/mlund/chemistry-notebooks/tree/master/liquid-monte-carlo) 🥕
- Interactions between patchy particles (potential of mean force, dipole alignment, scattering)
  [Initiual Notebook exists](https://github.com/mlund/chemistry-notebooks/tree/master/patchy-particle-interactions) 🥕
- A flexible polymer (collapse, radius of gyration, electrostatics)
  [Example input](https://github.com/mlund/faunus/blob/master/examples/polymers/polymers.yml) 🥕🥕
- Alchemical reactions (proton titration in bio-molecules and grand canonical ensembles)
  [Example input](https://github.com/mlund/faunus/blob/master/examples/fasta-titration.yml) 🥕🥕

*You* decide what to investigate, but please consult with a teacher what you plan to do.
More carrots mean more difficult, but mostly because no initial notebook exists.

## Coverage

Run simulations and report your findings in a Jupyter Notebook; here are some guidelines for what to include:
- [ ] Introduction
      Description of the studied system and what and how you plan to investigate it. Also include a <em>snapshot</em> or configuration from the simulation.
- [ ] Methodology
      Description and motivation of the energy function used, _i.e._ model.
      Description and motivation of the Monte Carlo moves used, i.e. sampling technique
- [ ] Results and discussion.
      Analysis of displacement parameters, acceptance, and convergence using e.g. the
      system energy as a function of steps. Discussion of results incl. plots.

## Self Check
  
Can you explain the following simulation jargon?
  
- [ ] move acceptance
- [ ] trial energy
- [ ] displacement parameter
- [ ] convergence
- [ ] equilibration run
- [ ] production run
- [ ] sampling
- [ ] steps
- [ ] trial move
- [ ] random number seed
- [ ] restart file
- [ ] trajectory
  

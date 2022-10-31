# Faunus Lab

## Getting started

1. Install [Docker Desktop](https://www.docker.com/products/docker-desktop) (Mac, Windows, Linux, ...)
2. Start Docker
3. In a terminal, run `docker run -it -p 8888:8888 mikaellund/faunus:latest_x86`
   Omit `_x86` if using a newer mac with "Apple silicon", _i.e._ with an M1 ARM processor.
4. Copy the generated link, _e.g._ `http://127.0.0.1:8888...`, into a web-browser.

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
      This loads a _Jupyter Notebook_ - here's
      [one of many](https://www.youtube.com/watch?v=jZ952vChhuI) introductory videos for how to use it.

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
  

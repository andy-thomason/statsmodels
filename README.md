# statsmodels

A slavish translation of the python statsmodels library

## Objective

To incrementally port the Python statsmodels library to Rust.

To improve performance where possible, for example using JIT compiled models,
custom mathematical functions and less LAPACK/ndarray.

To test rigorously against the python model.

To support different numerical types such as fp16 and qd.

## Picking initial targets

As we have limited resources, we will need to port incrementally
picking a set of initial targets. We have been canvasing data scientists
for a list of "must haves" so that we can prioritise this.

## Using automatic translation tools.

There are existing Python to Rust translators, I wrote a basic one for an Ethereum
hackathon to translate the Ethereum specification a few years ago, for example.

There is a pytho package called pyrs, for example, but it seems limited.

statsmodels does not use the Pytho 3.5 types, which makes this more challenging.

Probably doing the initial ports manually would be better.


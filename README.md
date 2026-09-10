# Lab 1 - Reproducible Computing Setup - Benjamin Wilson

This is the first lab of Applied Computing in Health Data Science. At the graduate level, this lab gave me the goal of constructing a reproducible computing setup using Python and R.

## Project Structure

src/ contains the scripts for this computing setup. One file was coded in R, and the other in Python. This was important to show that the setup could be reconstructued through the yml file.
data/ would contain the data for this project, but the dataframes for this assignment were created within the script themselves.
environment.yml contains the information concerning the Python, Conda, and Mamba specification.
renv.lock contains the information concerning the R package and environment specification.
Dockerfile consists of the container defintion and is required for the graduate addendum of this assignment.

## Python Environment

Create the Mamba environment:

mamba env create -f environment.yml
mamba activate repro-demo
python src/analyze.py

## R Environment

renv::restore()
source("src/analyze.R")

## Docker

docker build -t lab1 .
docker run --rm lab1

## Comparing Workflows

The key difference I noticed between the R and Python environment workflows was the time it took to deconstruct and reactivate them. In my opinion, the Python workflow was much more elaborate, and many more things went wrong in the process of trying to reach the finish line. The few R commands I needed to utilize to snapshot and create a lockfile certainly caused me less of a headache, and I think I would rather use renv for future projects solely on that reason.
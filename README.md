# How To Set Up an Environment for Machine Learning with Conda and Pip-Tools

## Overview
This is the repository for my Youtube Video that you can check out [here](https://www.youtube.com/watch?v=-lcJhz795H0&t=7s), also in article form [here](https://lucas-soares.medium.com/setting-up-an-environment-for-machine-learning-with-conda-pip-tools-9e163cb13b92) where I go through how to set up a nice and robust machine learning environment using [conda](https://docs.anaconda.com/) and [pip-tools](https://github.com/jazzband/pip-tools).

## 1. Create conda environment
a. Specify Python version

---

## 2 Activate the environment

---

## 3. Install the right cuda tool for our Pytorch environment 

(optional)

---

## 4. Export the environment to an `environment.yml` file

---

## 5. Create the requirements folder with the necessary `.in` files
- `dev.in` and `prod.in` for both development and production environments
- We will put our dependencies in these files

---

## 6. Write a MakeFile with 3 basic commands:
- `help`: (to print the makefile commands)
- `conda-update` to update our environment
- `pip-tools` to install, compile and sync our dependency requirements in 
both development and production environments

---

## 7. Run `make conda-update`

---

## 8. Run `make pip-tools
- installs all the packages in the `.in` files and takes care of any potential
conflicts that might exist

---

## 9. END! :)

---

### Credits

- https://github.com/full-stack-deep-learning/fsdl-text-recognizer-2021-labs
- https://github.com/full-stack-deep-learning/conda-piptools
- https://github.com/jazzband/pip-tools

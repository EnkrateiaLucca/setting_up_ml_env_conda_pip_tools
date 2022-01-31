---
marp: true
class: invert
color: white
---


# Setup a hybrid conda & pip-tools environment for Machine Learning

---


# 1. Create conda environment
a. Specify Python version

---

# 2 Activate the environment

---

# 3. Install the right cuda tool for our Pytorch environment 

(optional)

---

# 4. Export the environment to an `environment.yml` file

---

# 5. Create the requirements folder with the necessary `.in` files
- `dev.in` and `prod.in` for both development and production environments
- We will put our dependencies in these files

---

# 6. Write a MakeFile with 3 basic commands:
- `help`: (to print the makefile commands)
- `conda-update` to update our environment
- `pip-tools` to install, compile and sync our dependency requirements in 
both development and production environments

---

# 7. Run `make conda-update`

---

# 8. Run `make pip-tools
- installs all the packages in the `.in` files and takes care of any potential
conflicts that might exist

---

# 9. END! :)








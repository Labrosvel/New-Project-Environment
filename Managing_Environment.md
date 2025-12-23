## Python environment
1. **python3 -m venv <env_name>**                    *# create env*
2. **source <env_name>/bin/activate**                *# activate it*
3. **deactivate**                                    *# deactivate it*
4. **pip list**                                      *# see what's in the environment*
5. **pip freeze > requirements.txt**                 *# export environment*
6. **source <env_name>/bin/activate**                *# return to venv*
7. **pip install -r requirements.txt**               *# clone to new environment*
8. **rm -rf <env_name>**                             *# remove environment*

## Conda environment
1. **conda create --name myenv python=3.10**                            *# Create new environment*
2. **conda activate myenv**                                             *# Activate it*
3. **conda deactivate**                                                 *# Deactivate it*
4. **conda list**                                                       *# See what's in the base environment*
5. **conda activate base**                                              
6. **conda env export > base_environment.yml**                          *# Export env to a file*
7. **conda activate myenv**
8. **conda env create --name clonedenv --file base_environment.yml**    *# Clone base into a new env*
9. **conda env create -f <file.yml>**                                   *# Create env from file.yml*
10. **conda remove --name myenv --all**                                  *# Remove env*
11. **conda env update --name myenv --file environment.yml --prune**    *# Update env removing packages not in YAML*
12. **conda env list**                                                  *# conda environment list*
13. **conda install -c conda-forge <package_name>**

## Kernel
1. **jupyter kernelspec list**    *# lists all available kernels*
2. **jupyter kernelspec remove <kernel_name>**    *# removes the kernel*
3. **python -m ipykernel install --user --name=<kernel_name> --display-name 'Python (kernel_name)'**    *#(Re-)registers a kernel*




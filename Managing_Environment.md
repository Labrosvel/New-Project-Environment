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
1.**conda env list**                                                    *# conda environment list*
2. **conda create --name myenv python=3.10**                            *# Create new environment*
3. **conda activate myenv**                                             *# Activate it*
4. **conda deactivate**                                                 *# Deactivate it*
5. **conda list**                                                       *# See what's in the base environment*
6. **conda activate base**                                              
7. **conda env export > base_environment.yml**                          *# Export env to a file*
9. **conda env create --name clonedenv --file base_environment.yml**    *# Clone base into a new env*
10. **conda env create -f <file.yml>**                                   *# Create env from file.yml*
12. **conda remove --name myenv --all**                                  *# Remove env*
13. **conda env update --name myenv --file environment.yml --prune**    *# Update env removing packages not in YAML*
15. **conda install -c conda-forge <package_name>**

## Kernel
1. **jupyter kernelspec list**    *# lists all available kernels*
2. **jupyter kernelspec remove <kernel_name>**    *# removes the kernel*
3. **python -m ipykernel install --user --name=<kernel_name> --display-name 'Python (kernel_name)'**    *#(Re-)registers a kernel*




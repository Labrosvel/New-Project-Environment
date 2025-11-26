## Python environment
1. python3 -m venv <env_name>                    # create env
2. source <env_name>/bin/activate                # activate it
3. deactivate                                    # deactivate it
4. pip list                                      # see what's in the environment
5. pip freeze > requirements.txt                 # export environment
6. source <env_name>/bin/activate                # return to venv
7. pip install -r requirements.txt               # clone to new environment
8. rm -rf <env_name>                             # remove environment


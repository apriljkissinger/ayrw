# Austin Youth River Watch Jupyter Lab

## Setup

1. Clone the repository and navigate to the `ayrw` directory

```
git clone https://github.com/apriljkissinger/ayrw.git && cd ayrw
```

2. Install [pipenv](https://pipenv.pypa.io/en/latest/installation/)

```
pip3 install pipenv --user
```

3. Check [pipenv](https://pipenv.pypa.io/en/latest/installation/) installation. If the following command works, skip to step 5.

```
pipenv
```

4. If the `pipenv` command failed in step 3, add the following to `~/.zshrc` replacing `3.11` with your version of python. To check your version of python run `python3 --version`.

```
# Add python user bin directory
export PATH="$HOME/Library/Python/3.11/bin:$PATH"
```

5. Install any known project dependencies. Project dependencies are specified within [Pipfile](./Pipfile). Two files should be creating after running the following command: Pipfile and Pipfile.lock.

```
pipenv install
```

6. Add "jupyterlab = "*"" to the [packages] section of the Pipfile and please rerun the following command

```
pipenv install
```  

7. To activate this project's virtual environment, pleasse run the following.

```
pipenv shell
```
## Install new packages

To install new packages, please run the following replacing $PACKAGE_NAME with the name of the package.

```
pipenv install $PACKAGE_NAME
```
## Run

To run Jupyter Lab, please run the following.

```
pipenv run jupyter lab
```



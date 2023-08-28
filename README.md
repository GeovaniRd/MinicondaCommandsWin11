# Miniconda Commands on Windows 11

A simple reference for the most commonly used Miniconda commands on Windows 11. This guide is intended to help beginners get started and serve as a quick reference for more experienced users.

## Table of Contents

* Installation
* Managing Conda
* Managing Environments
* Managing Packages
* Conda Info & Help

## Installation

1 . **Download Miniconda for Windows:** Visit the **[official Miniconda page](https://docs.conda.io/en/latest/miniconda.html)**  and download the appropriate version for Windows.

2 . **Install Miniconda:** Double click the installer and follow the on-screen instructions.

3 . **Install Miniconda with a specific Python version:** You could also install miniconda with a specific Python version, for that you can use the command:
```
conda install python=[python_version]
```
For example, if you wanted to install Python 3.8 using Miniconda, you'd use:
```
conda install python=3.9
```

## Managing Conda
***- Using Conda from the Command Prompt:***

When you open the Command Prompt in Windows, you can activate the base conda environment by simply typing:
```
conda activate
```
This will allow you to use conda and any tools or libraries installed in the base environment directly from the Command Prompt.

***- Update Conda to the latest version:***

```
conda update conda

```

***- Update all packages in the current environment:***
```
conda update --all
```

## Managing Environments

***- Create an environment with a specific Python version:***
```
conda create --name [env_name] python=[python_version]
```

***- Set a specific Python version as the default for an environment:***

First, activate your environment:
```
conda activate [env_name]
```

Then, install the desired Python version:
```
conda install python=[python_version]
```

***- List all conda environments:***
```
conda env list
```

***- Activate an environment:***
```
conda activate [env_name]
```

***- Deactivate the current environment:***
```
conda deactivate
```

***- Remove an environment:***
```
conda env remove --name [env_name]
```

***- Clone an environment:***
```
conda create --name [new_env_name] --clone [existing_env_name]
```

## Managing Packages
***- Install a package in the current environment:***
```
conda install [package_name]
```

***- List all packages in the current environment:***
```
conda list
```

***- Remove a package from an environment:***
```
conda remove --name [env_name] [package_name]
```

***- Search for a package:***
```
conda search [package_name]
```

***- Install a package from a specific channel:***
```
conda install --channel [channel_name] [package_name]
```

***- Updating all environments:***

Sometimes you might want to update all packages across all environments. This can be done by:
```
conda update --all --all
```
***- Clean up any cached downloaded packages and remove unused packages:***
```
conda clean --all
```

## Conda Info & Help
***- Get information about conda:***
```
conda info
```
***- Check the Python version:***
```
python --version
```

***- Get help on any command:***
```
conda [command] --help
```

## Contribution

If you find any mistakes or have suggestions to improve this reference, please create an issue or submit a pull request.

##

Remember to adjust the **'[placeholders]'** in the commands with your desired values. This should give a good start for anyone looking to get familiar with Miniconda on Windows 11!

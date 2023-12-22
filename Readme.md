# Tensorflow Installation Guide

This is a [Tensorflow](https://www.tensorflow.org/) installation guide which will help to setup Tensorflow with [GPU support](https://www.tensorflow.org/install/source_windows) in a windows machine(windows 10 and 11).

![Tensorflow icon](https://miro.medium.com/v2/resize:fit:1200/1*HMCIHPssGii0Zk1CfLTrVA.png)


## Table of contents

- [Tensorflow Installation Guide](#tensorflow-installation-guide)
- [Important](#important)
- [Prerequiste](#prerequisite)
- [Installation](#installation)
- [Error Guide](#error-guide)
- [Contact & support](#contact--support)
- [License](#license)

## Important

Tensorflow for GPU support was removed after TF 2.10 version. The last supporting version of Tensorflow for GPU is 2.10 and below. Further documentation regarding the same is given in their official installation document. If you are not familiar with tensorflow, it is recommended to read this [document](https://www.tensorflow.org/install) before proceeding further


## Prerequisite

You need [python](https://www.python.org/) installed in your system. The following installation will be successfull with python version 3.10 to 3.7 . For <b>GPU support</b> , your need to download cuda 11.2 and its respective cudNN files.

- [CUDA 11.2](https://developer.nvidia.com/cuda-11.2.0-download-archive)
- [cudNN 8.1](https://developer.nvidia.com/rdp/cudnn-archive)

The notebook contains the same documentation on the requirements. For the necessary dependecies required for the installation, you can go through the [requirements.txt](./requirements.txt) file. For smooth installation, <b>do not use</b> the [requirements.txt](./requirements.txt) for installing the dependencies before hand.

## Installation

Clone this repository
```bash
git clone https://github.com/pratham-ak2004/Tensorflow-installation-guide
```

Navigate the the repository
```bash
cd Tensorflow-installation-guide
```

Using command prompt, create local python environment with version [3.10.11](https://www.python.org/downloads/release/python-31011/) . Replace `python` with the path of the interpreter with the required python version and `env_name` with your virtual environment name.
```bash
python -m venv env_name
```

Activate the python environment
```bash
.\env_name\scripts\activate ## for windows
```

Open the folder in jupyter notebook or any IDE
```bash
pip install jupyter-notebook ipykernel
python -m ipykernel install --user --name=env_name
jupyter notebook
```

Run the cells in `Tensorflow installation.ipnb` .

The installation is successfull when you get the below output when running the verification script<br>
![Verification script output](https://github.com/pratham-ak2004/Tensorflow-windows-installation-guide/assets/124170443/9ac2e851-aa49-4cb6-a9f0-3e6e5132bde2)

## Error

There is a possibility that you may encounter a number of errors while running the notebook. It is recommended to refer [Stackoverflow](https://stackoverflow.com/) for solving these error.

<b>Error:</b> No module named ‘xxxxxx’<br/>
<b>Solution:</b> Install that module</br>
<b>Note</b> the name of the module will not always equal the package name
```bash
!pip install xxxxx
```

For further errors you can contact the [owner](#support) of this repository.

## Drawbacks

`Tensorflow 2.10` was released on September 06, 2022. Because of this it might not be compatible with some of the packages and you might encounter warnings. This is normal during installation. For more details refer the original documentation provided by [`Tensorflow`](https://www.tensorflow.org/)

## Contact & Support

Feel free to contact me : )

[![Gmail](https://img.shields.io/badge/Gmail-EA4335.svg?style=for-the-badge&logo=Gmail&logoColor=white)](pratham20442@gmail.com)
[![Github](https://img.shields.io/badge/GitHub-181717.svg?style=for-the-badge&logo=GitHub&logoColor=white)](https://github.com/pratham-ak2004)
[![Linkdin](https://img.shields.io/badge/LinkedIn-0A66C2.svg?style=for-the-badge&logo=LinkedIn&logoColor=white)](https://www.linkedin.com/in/pratham-a-kadekar-8397a7249/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F.svg?style=for-the-badge&logo=Instagram&logoColor=white)](https://www.instagram.com/pratham_ak2004)
[![Twitter](https://img.shields.io/badge/Twitter-1D9BF0.svg?style=for-the-badge&logo=Twitter&logoColor=white)](https://twitter.com/a_kadekar1010)

## License

[![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)

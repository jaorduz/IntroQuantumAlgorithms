<div id="header"><p style="color:#3364ff; text-align:center; font-weight:bold; font-family:verdana; font-size:25px;">Quantum Algorithm Implementation </p></div>

[licenseBDG]: https://img.shields.io/badge/License-CC-orange?style=plastic
[license]: https://creativecommons.org/licenses/by-nc-sa/3.0/deed.en

[mywebsiteBDG]:https://img.shields.io/badge/website-jaorduz.github.io-0abeeb?style=plastic
[mywebsite]: https://jaorduz.github.io/

[mygithubBDG-jaorduz]: https://img.shields.io/badge/jaorduz-repos-blue?logo=github&label=jaorduz&style=plastic
[mygithub-jaorduz]: https://github.com/jaorduz/

[mygithubBDG-jaorduc]: https://img.shields.io/badge/jaorduc-repos-blue?logo=github&label=jaorduc&style=plastic 
[mygithub-jaorduc]: https://github.com/jaorduc/

[myXprofileBDG]: https://img.shields.io/static/v1?label=Follow&message=jaorduc&color=2ea44f&style=plastic&logo=X&logoColor=black
[myXprofile]:https://twitter.com/jaorduc


[![website - jaorduz.github.io][mywebsiteBDG]][mywebsite]
[![Github][mygithubBDG-jaorduz]][mygithub-jaorduz]
[![Github][mygithubBDG-jaorduc]][mygithub-jaorduc]
[![Follow @jaorduc][myXprofileBDG]][myXprofile]
[![CC License][licenseBDG]][license]

---

<p style="text-align:right; font-family:verdana;"><a href="mywebsiteBDG" style="color:#3364ff; text-decoration:none;">@Javier Orduz</a></p>    

---

This repository contains Quantum algorithms implementation.


## Contents
1. [Introduction](#intro)
1. [Installing](#installing)
1. [References](#references)

## 1. Introduction <a name = intro></a>



## 1. Installing <a name = installing></a>

Here you have the packages required to run this notebook.

To install miniconda, create an environment with 

```bash
mkdir -p ~/miniconda3
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh -o ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
source ~/miniconda3/bin/activate
conda env list
conda init --all
```

To install qiskit 
```bash
conda create -n qiskitQntm python=3.10 -y
python3 -m venv qiskitQntm
conda env list
conda activate qiskitQntm
pip3 uninstall qiskit qiskit-terra qiskit-aer qiskit-ibmq-provider qiskit-ibm-provider -y
pip3 install qiskit==1.2.1 qiskit-aer==0.13.3 qiskit-ibm-provider

```
You should probably install ipykernel/jupyter after clicking in the emergent window.



Additionally you will require
```bash
pip3 install matplotlib
pip3 install pylatexenc
```

## 1. Potential errrors <a name = errors></a>

```bash
ImportError: Qiskit is installed in an invalid environment that has both conda Qiskit >=1.0 and an earlier version. You should create a new virtual environment, and ensure that you do not mix dependencies between Qiskit <1.0 and >=1.0. Any packages that depend on 'qiskit-terra' are not compatible with Qiskit 1.0 and will need to be updated. Qiskit unfortunately cannot enforce this requirement during environment resolution. See https://qisk.it/packaging-1-0 for more detail.
```
Solution:
Install compatible versions of packages, you should use 

```bash
python version:  3.10.15
qiskit==1.2.1
qiskit-aer==0.13.3
qiskit-ibm-provider==0.11.0
```

## 1. References <a name = references></a>

[1] <a href="https://qaldas.github.io/quaker-ece/">Quantum Computing: A gentle introduction for Liberal Arts Institutions</a>. Levi Goldberg, Shun Suzuki, Javier Orduz. WebBook 2024. 
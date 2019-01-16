# NoahMP-Training

This material helps you compiling and runing the NoahMP land surface model.

## Setting up the Linux environment

NoahMP runs in a Linux environment and requires the [NetCDF4](https://www.unidata.ucar.edu/software/netcdf/) library installed in your system.

If you are using Windows 10, you can either enable [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about) or install a virtual machine using [Oracle VirtualBox](https://www.virtualbox.org).

Following the instructions to enable Windows Subsystem for Linux (WSL). 

Note: Ubuntu is recommonded for this training material.

Once the Linux environment is setted up, install the Fortran compiler and NetCDF4 library by typing the following commands in your terminal:
```
sudo apt update && upgrade
sudo apt install gcc gfortran netcdf-bin libnetcdf-dev libnetcdff-dev
sudo apt install openmpi-bin libopenmpi-dev
```

## Downloading the NoahMP source code and compiling the model

Read `README.md` in the NoahMP source code directory and compile the model following the instructions.

Once the model successfully compiled, the excecutable file `noahmp.exe` is located in the `run` directory.

## Download this repository to your disk

This repository contains all the files needed for running NoahMP.

You can download the files via the link [https://github.com/esmwg/NoahMP-Training/archive/master.zip] or clone this repository using [Git](https://git-scm.com/).

Once downloaded, locate the `NoahMP-Training` directory in your WSL terminal or VirtualBox.

If you are using WSL, all your Windows files are automatically mounted on `/mnt/`.

## Running NoahMP

Copy `noahmp.exe` to the `NoahMP-Training` directory and type `./noahmp.exe` in the Ubuntu command terminal.

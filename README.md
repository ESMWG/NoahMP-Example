# NoahMP-Training

This material helps you compiling and runing the NoahMP land surface model.

## Setting up the Linux environment

NoahMP runs in a Linux environment and requires the [NetCDF4](https://www.unidata.ucar.edu/software/netcdf/) and MPI libraries installed in your system.

If you are using Windows 10, you can either enable [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about) or install a virtual machine using [Oracle VirtualBox](https://www.virtualbox.org).

Following the instructions to enable Windows Subsystem for Linux (WSL). 

In your Linux environment (Ubuntu is recommanded for this training material), type the following commands in the terminal to install the Fortran compiler, NetCDF4, and MPI:
```
sudo apt update && upgrade
sudo apt install gcc gfortran
sudo apt install netcdf-bin libnetcdf-dev libnetcdff-dev
sudo apt install openmpi-bin libopenmpi-dev
```

## Download this repository to your disk

This repository contains all the files needed for running a NoahMP exemplary case.

You can download the files via the link [https://github.com/esmwg/NoahMP-Training/archive/master.zip] or clone this repository using [Git](https://git-scm.com/) [git clone https://github.com/esmwg/NoahMP-Training.git].

Once downloaded, locate the `NoahMP-Training` directory in your WSL terminal or VirtualBox.

If you are using WSL, all your Windows files are automatically mounted on `/mnt/`.

Note: the example contained in this repository are used for training purpose only, you cannot publish papers using this example.

## Downloading the NoahMP source code and compiling the model

Read `README.md` in the NoahMP source code directory and compile the model following the instructions.

Once the model successfully compiled, the excecutable file `noahmp.exe` is located in the `run` directory.


## Running NoahMP

Copy `noahmp.exe` to the `NoahMP-Training` directory and type `./noahmp.exe` in the Ubuntu command terminal.

# NoahMP-Example

This material helps you compile and run the NoahMP land surface model.

## Set up a Linux environment

NoahMP runs in a Linux environment and requires the [NetCDF4](https://www.unidata.ucar.edu/software/netcdf/) and [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface) libraries installed in your system.

If you are using Windows 10, you can either enable [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about) or install a virtual machine using [Oracle VirtualBox](https://www.virtualbox.org).

Follow the instructions in [doc/enable-wsl.md](doc/enable-wsl.md) to enable Windows Subsystem for Linux (WSL). 

If you are using Ubuntu, type the following commands in a terminal to install the Fortran compiler, NetCDF4, and MPI:
```
sudo apt update && sudo apt upgrade
sudo apt install gcc gfortran
sudo apt install netcdf-bin libnetcdf-dev libnetcdff-dev
sudo apt install openmpi-bin libopenmpi-dev
```

## Download this repository to your disk

This repository contains all the files needed for running an exemplary NoahMP simulation.

You can download the files via the link [https://github.com/esmwg/NoahMP-Example/archive/master.zip] or clone this repository using [Git](https://git-scm.com/) (`git clone https://github.com/esmwg/NoahMP-Example.git`).

Once downloaded, unzip `NoahMP-Example/input/input.zip` into the `NoahMP-Example/input` directory.

Warning: the example contained in this repository are used for training purpose only, you cannot use this example for publications and commercial purposes.

## Download and compile the NoahMP source code

The source code can be found in [https://github.com/esmwg/NoahMP].

Read `README.md` in the NoahMP source code directory and compile the model following the instructions.

Once the model successfully compiled, the excecutable file `noahmp.exe` is located in the `run` directory.


## Run `noahmp.exe`

Copy `noahmp.exe` to the `NoahMP-Example` directory.

Locate the `NoahMP-Example` directory in a command terminal. If you are using WSL, all the Windows files can be accessed via `/mnt`.

In the `NoahMP-Trainig` directory, type the following command:
```
./noahmp.exe
```

Hoo-ha!

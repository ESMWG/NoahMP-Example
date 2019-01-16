# NoahMP-Training

This material helps you compile and run the NoahMP land surface model.

## Set up the Linux environment

NoahMP runs in a Linux environment and requires the [NetCDF4](https://www.unidata.ucar.edu/software/netcdf/) and [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface) libraries installed in your system.

If you are using Windows 10, you can either enable [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about) or install a virtual machine using [Oracle VirtualBox](https://www.virtualbox.org).

Follow the instructions in [doc/enable-wsl.md](doc/enable-wsl.md) to enable Windows Subsystem for Linux (WSL). 

If you are using Ubuntu, type the following commands in the terminal to install the Fortran compiler, NetCDF4, and MPI:
```
sudo apt update && upgrade
sudo apt install gcc gfortran
sudo apt install netcdf-bin libnetcdf-dev libnetcdff-dev
sudo apt install openmpi-bin libopenmpi-dev
```

## Download this repository to your disk

This repository contains all the files needed for running a exemplary NoahMP simulation.

You can download the files via the link [https://github.com/esmwg/NoahMP-Training/archive/master.zip] or clone this repository using [Git](https://git-scm.com/) (`git clone https://github.com/esmwg/NoahMP-Training.git`).

In the `NoahMP-Training/input` directory, unzip `input.zip`.

Warning: the example contained in this repository are used for training purpose only, you cannot publish papers using this example.

## Download and compile the NoahMP source code

Note: The source code will be distributed later and you can skip this section now.

Read `README.md` in the NoahMP source code directory and compile the model following the instructions.

Once the model successfully compiled, the excecutable file `noahmp.exe` is located in the `run` directory.


## Run `noahmp.exe`

Copy `noahmp.exe` to the `NoahMP-Training` directory.

Locate the `NoahMP-Training` directory in a command terminal. If you are using WSL, all the Windows files can be accessed via `/mnt`.

In the `NoahMP-Trainig` directory, type the following command:
```
./noahmp.exe
```

Hoo-ha!

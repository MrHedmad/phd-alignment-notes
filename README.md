# Phd Re-alignment courses notes
Notes and code on the alignment courses for the PhD in Complex Systems for Quantitative Bioscience.

The courses were held during 2023, A.Y. 2022/2023.
There were specific courses for the Math- and Bio- background students.
I (Luca) am a Bio- background student, so only those courses are included here.

Each course has its own folder, and each course folder has a README with further info for that course. As a rule of thumb, there is one subfolder per lesson.

## Course Schedule
For reference, the schedule is stored in its own [SCHEDULE.md](SCHEDULE.md) file.

## System Info
Most (all) of the code and the notes were taken on my laptop:
at the time of writing, it ran Manjanaro Linux, with `zsh` as default shell.

System install of Python was version 3.10.9.
System install of R was version 4.2.2, "Innocent and Trusting". Remember that R needs `gcc-fortran` to compile external packages.
I had Docker installed.

## Prerequisites
There are some prerequisites to fulfill before you can follow along the notes:

#### Mathematical models for Life Sciences
- Install `anaconda`.
  I chose to install `miniconda` instead of the full installation because Anaconda is very bloated.
  To avoid having anaconda fuck up your environment, simply install it as normal, but choose your options wisely:
  - Just [download the installer script from here](https://docs.conda.io/en/latest/miniconda.html#linux-installers) and run it (`bash ./downloaded-script.sh`).
    At the end of installation, it will ask to run `conda init`. **Say NO**.

    Conda lives in a "base" python virtualenv, so it can be started and exited like any other env:
    Add the alias `startconda="source $HOME/miniconda3/bin/activate"` (so you don't have to remember what to type each time), and run `startconda` when you need it.
    If you don't "startconda", the `conda` command is disabled, and there is no change in your system Python installation.

#### Bioinformatics and Computational Models
- Install `GreatSPN` from https://github.com/greatspn/SOURCES/blob/master/docs/INSTALL.md.
  - If you are running Arch, I've uploaded a `PKGBUILD` file that you can use to install the program on your system. It is pretty rough, so take a look at it before installation: https://gist.github.com/MrHedmad/817465ad6c488f03d5cdc17196f561eb


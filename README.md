# Zeldy 

Group project SERI Supelec 2018 : Tangy Renan, Simon Brelivet, Julia Desmazes

Zeldy is an free software project for a small power monitoring system using an
esp32 with custom hardware for data acquisition and sends it to a backend via
HTTPS ( or optionally HTTP ). For the backend we are using a grafana + influxDB solution.

A presentation of the project is available in [`Zeldy slides`](Zeldy_slides.pdf)
in french.

## Project organisation 

This project is organised in different submodules with eatch submodule containing a 
diffrent aspect of the project namely :
- microcontroller code for the esp32
- hardware design files
- backend configurations

### Clone the project

To clone the project, since we are using submodules you will have to intializa your 
local configuration files with `git submodule init` and `git submodule update` to fetch 
all the data from the diffrent submodules.

```bash
git clone https://github.com/Essenceia/Zeldy/stable
git submodule init
git submodule update
```

### Update the project 

If a new push occures on the tracked submodules branches and you are not up to date 
anymore you can update it using :
```bash 
git submodule update
```

### *Devlopper* Add new submodules

Adding a submodule is equivalent in a way as adding a reference to another git within a 
project. You can do this with :
```bash 
git submodule add <git_submodule_address>/<branch>
```

## License

This code is released under the GNU GPL v3 public license.
:smile:

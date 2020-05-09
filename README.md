# Automatic-Control-System-for-Heat-Pump

This system can automatic adjust the heat pump status in real time according to electricity cost and user demands. It contains several modules, the simulation for heat transfer of the room and heat pump and overall system control. For the sumulation for heat transfer of room, there are a Room thermal model to simulate a room thermal change like temperature change. The model will give a visualization temperature change of a room. For the simulation of heat pump, there are heat pump model which is built by TESpy to get some parameters of heat pump and another function model to simulate a real heat pump (energy loss in changing state or other condition) based on parameter data from the previous model. The whole module will give heat energy or cool energy to room thermal model and give the electricity use and state of heat pump to control system. The control system will choose a state (percentage of heat pump working power) base on price change, weather temperature change and solar change to reduce the electricity fee. This module will receive the temperature data of the room module and the work state data of the heat pump module and deal with these data to send control singal to the heat pump module. 

The whole system is a continuted and dynamic model. In building the model, we will build 'time' parameter according to the time in the data set instead of designing "clock" inside the program to calculate time. Therefore, the project is just a simple simulation physical model, and the project team will improve the project based on other assumptions and factors in the future.

This project is to provide simulation kits for heat pumps and room models. With this software package, you can determine the relative reasonable working power of heat pump according to the weather, price data and user demand.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

If you have a working Python3 environment, use pypi to install the latest tespy version:

```
pip install tespy
```

Also, you may need to install the following package using pypi

```
pip install prettytable
```

### Installing

If you have a Git environment, use git to install the latest version:

```
git clone https://github.com/Tianhao-Y/Automatic-Control-System-for-Heat-Pump.git
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Built With

* [TESPy](https://github.com/oemof/tespy) - The Heat Pump Simulation used

## Authors

* **Tianhao Yu** 
* **Mengzhou Wang** 

See also the list of [contributors](https://github.com/Tianhao-Y/Automatic-Control-System-for-Heat-Pump/graphs/contributors) who participated in this project.

## License
Copyright (c) 2020 (Australian National University 2020 year ENGN4221 Heat Pump group)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Acknowledgments

Key parts of this project require the following scientific software packages: Matplotlib[Matplotlib], NumPy [@NumPy], Pandas [@Pandas]. Other packages implemented are Matplotlib and Math.


# Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. 

Please note we have a code of conduct, please follow it in all your interactions with the project.

## Pull Request Process

1. Ensure any install or build dependencies are removed before the end of the layer when doing a 
   build.
2. Update the README.md with details of changes to the interface, this includes new environment 
   variables, exposed ports, useful file locations and container parameters.
3. Increase the version numbers in any examples files and the README.md to the new version that this
   Pull Request would represent. The versioning scheme we use is [Heat pump Landing page](https://u5926427.wixsite.com/mysite-1).
4. You may merge the Pull Request in once you have the sign-off of two other developers, or if you 
   do not have permission to do that, you may request the second reviewer to merge it for you.

## Code of Conduct

### Our Pledge

In the interest of fostering an open and welcoming environment, we as
contributors and maintainers pledge to making participation in our project and
our community a harassment-free experience for everyone, regardless of age, body
size, disability, ethnicity, gender identity and expression, level of experience,
nationality, personal appearance, race, religion, or sexual identity and
orientation.

### Our Standards

Examples of behavior that contributes to creating a positive environment
include:

* Using welcoming and inclusive language
* Being respectful of differing viewpoints and experiences
* Gracefully accepting constructive criticism
* Focusing on what is best for the community
* Showing empathy towards other community members

Examples of unacceptable behavior by participants include:

* The use of sexualized language or imagery and unwelcome sexual attention or
advances
* Trolling, insulting/derogatory comments, and personal or political attacks
* Public or private harassment
* Publishing others' private information, such as a physical or electronic
  address, without explicit permission
* Other conduct which could reasonably be considered inappropriate in a
  professional setting

### Our Responsibilities

Project maintainers are responsible for clarifying the standards of acceptable
behavior and are expected to take appropriate and fair corrective action in
response to any instances of unacceptable behavior.

Project maintainers have the right and responsibility to remove, edit, or
reject comments, commits, code, wiki edits, issues, and other contributions
that are not aligned to this Code of Conduct, or to ban temporarily or
permanently any contributor for other behaviors that they deem inappropriate,
threatening, offensive, or harmful.

### Scope

This Code of Conduct applies both within project spaces and in public spaces
when an individual is representing the project or its community. Examples of
representing a project or community include using an official project e-mail
address, posting via an official social media account, or acting as an appointed
representative at an online or offline event. Representation of a project may be
further defined and clarified by project maintainers.

### Enforcement

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting the project team at [INSERT EMAIL ADDRESS]. All
complaints will be reviewed and investigated and will result in a response that
is deemed necessary and appropriate to the circumstances. The project team is
obligated to maintain confidentiality with regard to the reporter of an incident.
Further details of specific enforcement policies may be posted separately.

Project maintainers who do not follow or enforce the Code of Conduct in good
faith may face temporary or permanent repercussions as determined by other
members of the project's leadership.





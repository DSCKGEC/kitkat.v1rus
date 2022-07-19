# kitkat.v1rus

[![Contributors](https://img.shields.io/github/contributors/dsckgec/kitkat.v1rus.svg)](https://github.com/dsckgec/kitkat.v1rus/graphs/contributors) [![Forks](https://img.shields.io/github/forks/dsckgec/kitkat.v1rus.svg)](https://github.com/dsckgec/kitkat.v1rus/network/members) [![Issues](https://img.shields.io/github/issues/dsckgec/kitkat.v1rus.svg)](https://github.com/dsckgec/kitkat.v1rus/issues) [![Pull Request](https://img.shields.io/github/issues-pr-closed-raw/dsckgec/kitkat.v1rus)](https://github.com/dsckgec/kitkat.v1rus/pulls)

A python implementation of a keylogger, that can act as a payload or a subroutine to another program.

### NOTE
while downloading the code or running it locally please disable your anti-virus or windows protection or put the files into an exception in your antivirus software.

## Contents

1. [Description](#description)
1. [Project structure](#project-structure)
1. [Project roadmap](#project-roadmap)
1. [Getting started](#getting-started)
1. [Working](#working)
1. [Built with](#built-with)
1. [Contributing](#contributing)
1. [Authors](#authors)
1. [License](#license)
1. [Acknowledgments](#acknowledgments)

## Description

### What's the problem?
We often forget what we type in our day to day lives, it maybe the last password you used to login into your bank account or maybe a certain website your kid visited and now you can't check on it because either it was opened on incognito or the history has been deleted. Or even in large organisation/schools it becomes hard for IT managers to check on their employees/students and what they've been texting or typing and to whom using the organisation computers. It's a real world problem that many face while excercising discipline and monitoring.

### How can this project help?
Keystroke logging, often referred to as keylogging or keyboard capturing, is the action of recording the keys struck on a keyboard, typically covertly, so that a person using the keyboard is unaware that their actions are being monitored. Data can then be retrieved by the person operating the logging program. 

### The idea

Most workstation keyboards plug into the back of the computer, keeping the connections out of the user's line of sight. A hardware keylogger may also come in the form of a module that is installed inside the keyboard itself. When the user types on the keyboard, the keylogger collects each keystroke and saves it as text in its own hard drive, which may have a memory capacity up to several gigabytes. The person who installed the keylogger must later return and physically remove the device to access the gathered information. There are also wireless keylogger sniffers that can intercept and decrypt data packets transferred between a wireless keyboard and its receiver.

A common software keylogger typically consists of two files that get installed in the same directory: a dynamic link library (DLL) file that does the recording and an executable file that installs the DLL file and triggers it. The keylogger program records each keystroke the user types and periodically uploads the information over the internet to whomever installed the program. Hackers can design keylogging software to use keyboard application program interfaces (APIs) to another application, malicious script injection or memory injection.

Screenshot of data captured from keylogger software
Data keyloggers can capture various information from its targets.
There are two main types of software keyloggers: user mode keyloggers and kernel mode keyloggers.

A user mode keylogger uses a Windows API to intercept keyboard and mouse movements. GetAsyncKeyState or GetKeyState API functions might also be captured depending on the keylogger. These keyloggers require the attacker to actively monitor each keypress.

A kernel mode keylogger is a more powerful and complex software keylogging method. It works with higher privileges and can be harder to locate in a system. Kernel mode keyloggers use filter drivers that can intercept keystrokes. They can also modify the internal Windows system through the kernel.

Some keylogging programs may also include functionality to record user data besides keystrokes, such as capturing anything that has been copied to the clipboard and taking screenshots of the user's screen or a single application.

## Project structure

``` 
  ├── logger.py               Code and Definition of keylogger with which you can record the keystrokes
  ├── requirements.txt        For python module imports          
```

## Project roadmap

The project currently does the following things.

- Record keystrokes
- Print it on a console
- Save the strokes in a file using a timestamp

See below for our future steps.

- Record mouse strokes and scrolls
- Send the log files into our email account
- Support multi-lingual keyrecording 

## Getting started


### Prerequisites
**Client:** Python

**Server:** Not used

### Installing

Clone the project

```bash
  git clone https://github.com/DSCKGEC/kitkat.v1rus.git
```

Go to the project directory

```bash
  cd kitkat.v1rus
```

To run this:
```bash
  pip3 install -r requirements.txt
```
## Working
- Initially the keylogger is set to record all the keystrokes and appened the new keys with an intervel of 60 seconds.
- The file will be created in the root directory of the file itself
- The virus is harmless and only collects your keyboard data but can be further customised to record sound and mouse pointing vectors
- To stop the keylogger completely from your local machine use the task manager to kill the event manually


## Built with

- [Python](www.python.org)

## Contributing

Please read [contributing.md](contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

<a href="https://github.com/DSCKGEC/kitkat.v1rus/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=DSCKGEC/kitkat.v1rus" />
</a>

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- (add your name here below this line along with your github profile link)

# Go-Keylogger

## Problem Statement
Keyloggers are built for the act of keystroke logging — creating records of everything you type on a computer or mobile keyboard. These are used to quietly monitor your computer activity while you use your devices as normal. Keyloggers are used for legitimate purposes like feedback for software development but can be misused by criminals to steal your data. The following is an example of a simple keylogger built in Golang.

## Prerequisites
* Go 1.18
* Windows OS

## Working

* Import necessary packages. The following program uses https://github.com/TheTitanrain/w32.
* The variables used are declared.
* The functions used are:
    * getForeGroundWindow() - retreieves a handle to the foreground window (i.e. the window the user is currently using)
    * getWindowText() - copies text of specified window's handle bar into buffer
    * windowLogger() - calls the above defined functions and converts text from UTF16 to String to be stored in a human readable format for the keylogs
    * keyLogger() - reads input and appends to the logs by using above defined functions

## Output

![image](https://user-images.githubusercontent.com/60508605/172185180-5d2939e7-e94e-4a90-829d-ee71e102a04c.png)

## Usage
* Clone the repository
  `git clone https://github.com/Annanya481/Go-Keylogger`
* Run keylogger.go
  `go run keylogger.go`

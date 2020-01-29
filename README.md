# Mac terminal World
This repository has shortcuts that are handy when you want to get all your tasks done using Mac Terminal.
Before we start, lets make sure that your system has [HomeBrew](https://brew.sh/). It is a must when you are software developer and using Mac. They have an interesting description for themselves i.e. 
> The Missing Package Manager for macOS

## Copy output of a command to clipboard
`pbcop` is used to copy content to clipboard. The content can be from a file or output of a command. 
Below I am trying to copy the current directory path to clipboard
```shell
pwd | pbcopy
```
**NOTE**: the last next line character also gets copied. Meaning, the content in clipboard would be similar to `/Users/username/Documents(enter)`.

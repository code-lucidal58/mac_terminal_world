# Mac Terminal World
This repository has shortcuts that are handy when you want to get all your tasks done using Mac Terminal.
Before we start, lets make sure that your system has [HomeBrew](https://brew.sh/). It is a must when you are software developer and using Mac. They have an interesting description for themselves i.e. 
> The Missing Package Manager for macOS

Next thing, the inbuilt Mac terminal has a very bad UI (my opinion, don't get swayed). I prefer using 
[iTerm](https://iterm2.com/). Or, let me admit, I did not try anything else because I was happy with the latter.

## Copy output of a command to clipboard
`pbcop` is used to copy content to clipboard. The content can be from a file or output of a command. 
Below I am trying to copy the current directory path to clipboard
```shell
pwd | pbcopy
```
**NOTE**: the last next line character also gets copied. Meaning, the content in clipboard would be similar to `/Users/username/Documents(enter)`.


## Compare contents of two folders
`diff` is a buitin command that can be used to find difference between folders and files. There are two flags:
* `r`: compare files/folders recursively i.e. find difference in subdirectories as well. 
* `q`: display a brief result
```shell
diff -rq path-to-folder1 path-to-folder2
```
The result of the above command will look something like this:
```shell
Files path-to-folder1/README.md and path-to-folder2/README.md differ
Files path-to-folder1/docs/demoApp.md and path-to-folder2/docs/demoApp.md differ
Only in path-to-folder1/: x.txt
Only in path-to-folder2/: y.txt

```
`diff` can be used to compare content of files.
Additional knowledge base can be found [here](https://ss64.com/osx/diff.html)

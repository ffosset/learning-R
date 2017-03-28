# learning-R
### Functions
- `>` at the beginning of a line is R's prompt for you type something into the console
- `skip()` allows you to skip the current question
- `play()` lets you experiment with R on your own; swirl will ignore what you do...
- `nxt()` which will regain swirl's attention
- `bye()` causes swirl to exit. Your progress will be saved
- `main()` returns you to swirl's main menu
- `info()` displays these options again
- `help.start()` will open a menu of resources
- `abs()`absolute value
- `sqrt()`square root
- the up arrow will cycle through previous commands
- `getwd()`determines the directory your current R session is using
- `ls()` lists all the objects in your local workspace
- `dir()` lists all the files in your working directory


### Install and load a package
```R
> install.packages("packageName")
> library("packageName")
> packageName()
```

### Basic Building Blocks
Assign a value to a variable: `var <- val` </br>

Create a vector: use the `c` function, or `concatenate`
```R
> z <- c(1.1, 4, 3.9)
> z * 2 + 100

102.20 118.00 106.28
```
When given two vectors of the same length, R performs the specified arithmetic operation **element-by-element**. If the vectors are of different lengths, R 'recycles' the shorter vector until it is the same length as the longer vector. When we did z * 2 + 100, z was a vector of length 3, but technically 2 and 100 are each vectors of length 1. Behind the scenes, R is 'recycling' the 2 to make a vector of 2s and the 100 to make a vector of 100s.
```R
> c(1, 2, 3, 4) + c(0, 10)
> Result: 1 12 3 14
```

### File manipulation
- `file.create(...)`
- `file.exists(...)`
- `file.remove(...)`
- `file.rename(from, to)`
- `file.append(file1, file2)`
- `file.copy(from, to)`

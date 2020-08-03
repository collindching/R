
# Debugging (from _Advanced R_)

## Overall approach

1. Google the error message
2. Reproduce the problem, then make a minimum reproducible example
3. Locate the problem
4. Utilize scientific method
5. Fix and test

## Locating errors

Leverage `traceback()` to find out where the error occurs. 

## Interactive debugging

To get more information, use interactive debugger to pause execution of function and interactively explore its state.

Can insert a call to `browser()` at location where you'd want to pause and re-run function. This puts you into an interactive environment inside the function. RStudio will show you objects in current environment in Environment pane. 


### browser() commands

- `n` (next) executes next step in function
- `s` (step into) steps into function
- `f` (finish) finishes execution of current loop/function
- `c` (continue) leaves interactive debugging, and continues regular execution
- `q` (stop) stops debugigng, terminates function, and returns to globa lworkspace

## Print debugging

Insert print statements to precisely locate problem. Slow and primitive, but always works. 
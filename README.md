# Silent Failure in read.csv() when File Not Found

This repository demonstrates a common, yet subtle, error in R when using `read.csv()` to read a CSV file that might not exist. The issue is that the function fails silently, not providing any indication that the file was not found. This can lead to unexpected results and difficult-to-debug errors later in the code.

The `bug.R` file contains the problematic code.  `bugSolution.R` shows how to properly handle this situation using `tryCatch()` to gracefully manage the potential error.
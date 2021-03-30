# DS Teams - ACCRE FAQ/Troubleshooting


# Logging on to ACCRE

## Method 1: Visualization Portal

1. Go to portal.accre.vanderbilt.edu
2. Log on using your VUNetID as the Username and your ACCRE password (this is likely different from your VUNetID password)
3. Use an Interactive session (RStudio or Jupyter Notebook)

## Method 2: Using Command Line

1. ssh vunetid@login.accre.vanderbilt.edu
2. Enter ACCRE password (this is likely different from your VUNetID password)
3. You should now be in your home directory

# Working with Large Datasets

Consider using a sample of the data instead of joining all the datasets. For example, you could sample by customer ID, perhaps which will help increase your computation time significantly and free up resources for other users.

# Selecting Resources

When setting up an interactive session in RStudio or Jupyter Notebooks avoid using more resources than you need. **Unless you are using parallelization, your code is almost always running on a single core**. Do not ask for multiple cores unless you are using parallization. At most, ask for 2-3 cores. Instead, ask for more memory. In the scenario where you are using all the data combined, you will likely need at least 64GB of memory. 

**Use the GPU only if required!!**

# Reading and writing data

All original data provided to you by the client is stored under the following directory: /data/p_dsi/client_name/data/
The original data should ideally stay in this directory

The teams folders under /data/p_dsi/client_name/teams/ are not for storing the client data, but instead for storing any aggregates or additional data sources required for your project. 

**Do not write any files to your home directory.** There is also a file size limit on your home folder, so you will be unable to store any files larger than that size in your home directory. 

# Diagnosing crashed sessions

# Frequently asked questions

Please refer to the ACCRE FAQ for solutions to most issues: https://www.vanderbilt.edu/accre/support/faq/


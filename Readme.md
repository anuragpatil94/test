# Testing Submodules

> Understanding the basics of how Submodules works  

1. updating a submodule from project repository

2. updating a submodule from its own repository(In this case submodule is its own project)
   
   - This won't change the code in the project repository since the submodule is pointed to a specific commit.
   - A change made (commited and pushed) in submodule from project repository is supposed to pull and resolve any conflicts before pushing it to submodule repository. (WHICH SHOULDN'T BE THE CASE AS THE SUBMODULE IS SUPPOSED TO BE HANDLED BY A SEPARATE TEAM)

3. Submodule Status

```
    1) modified:   submodule (modified content)
    -   This status means that the submodule has modified contents in when the contents is changed through project repository
    - The Project cannot be commited unless the submodule is commmited. 
    2) modified:   submodule (new commits)
    - Once the commits are resolved then the project can be commited with the submodule else the submodule won't be in the staging area
```

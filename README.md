# SMAIAX

This repository contains all the other repositories and brings the whole project together.

## How to clone the repository
To clone the repository you need to use the following commands otherwise the git submodule folders will be empty:
```
git clone https://github.com/SMAIA-X/smaiax --recursive
```

If you clone the repository without `--recursive` you have to use the following command:
```
git submodule update --init --recursive
```

## How to update the submodules
To update the submodules you need to run the following command
```
git submodule update --remote --merge 
```

After updating the submodules you need to commit the changes:
```
git add .
git commit -m "Updated submodules"
git push
```
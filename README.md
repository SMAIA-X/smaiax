# SMAIAX

This repository contains all the other repositories and brings the whole project together.

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
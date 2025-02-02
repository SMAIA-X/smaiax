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

## How to pull from the repository
After you cloned the repository and there are new changes you can pull the repository with the following command:
```
git pull --recurse-submodules
```

## How to run the project
With the following commands you can start the whole project:
```
docker compose build
docker compose up -d
```
Once all Docker containers are up and running, you can access the frontend at: `http://localhost:8080`.
The application comes with three predefined users:
| Name           | Username       | Email                      | Password  |
|-------------- |--------------|---------------------------|----------|
| John Doe      | johndoe       | john.doe@example.com      | P@ssw0rd |
| Jane Doe      | janedoe       | jane.doe@example.com      | P@ssw0rd |
| Max Mustermann | maxmustermann | max.mustermann@example.com | P@ssw0rd |

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
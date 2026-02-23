# Coding challenge

## Bash

You are tasked with creating a bash script which takes three input parameters. A unique name, a region and a path to a `.json` file. The file should be used as a template, it contains a json object which must contain at least the three attributes, `name`, `region` and `instances`. `name` has to be a string, `region` has to be a string and `instances` has to be a number greater than zero. The json template can have placeholder variables in it which should be replaced by the script. `$ENV` should be replaced by the unique name parameter and `$REGION` should be replaced by the region parameter. The script should validate the json files and exit with a non-zero error code, if not all parameters were provided, the provided json file is not valid or the created json is not valid. If valid the created json should be written to a new file.

### parameter examples

| unique name | region |
| - | - |
| tiger | westus2 |
| panda | westeurope |
| lion | eastus2 |

All string parameters should work correctly with all provided example `.json` files.

This script should be executable as part of a CI/CD pipeline, what do you think is important in this scenario?
What documentation would you create to explain this script to your colleagues?
You are expected to use standard Linux utilities including jq.

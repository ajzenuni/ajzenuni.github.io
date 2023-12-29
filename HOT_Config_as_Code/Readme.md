# delete manifest
monaco delete --manifest manifest.yaml --file delete.yaml

# deploy a single project
monaco deploy manifest.yaml -e PROD -p ownership 

# delete all configurations in the environment - BE CAREFUL
export MONACO_ENABLE_DANGEROUS_COMMANDS=1
monaco purge manifest.yaml -e ENV_NAME

# deploy tag project
monaco deploy _manifest.yaml -e ENV_NAME -p tag

# deploy ownership project
monaco deploy _manifest.yaml -e ENV_NAME -p ownership

# deploy managementZones project
monaco deploy _manifest.yaml -e ENV_NAME -p managementZones

# delete projects
monaco delete --manifest _manifest.yaml -e kale_managed --file delete.yaml


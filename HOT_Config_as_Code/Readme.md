# delete manifest
monaco delete --manifest manifest.yaml --file delete.yaml

# deploy a single project
monaco deploy manifest.yaml -e PROD -p ownership 
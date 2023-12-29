## DOC
- https://docs.dynatrace.com/docs/shortlink/configuration-as-code-commands

## Configuration as Code - Monaco - terminal commands
### get help for monaco
`monaco -h`

### deploy tag project
`monaco deploy manifest.yaml -e ENV_NAME -p tag`

### deploy ownership project
`monaco deploy manifest.yaml -e ENV_NAME -p ownership`

### deploy managementZones project
`monaco deploy manifest.yaml -e ENV_NAME -p managementZones`

### delete configurations as specified in delete.yaml
`monaco delete --manifest manifest.yaml -e ENV_NAME --file delete.yaml`

### download environment configurations
`monaco download --manifest manifest.yaml -e ENV_NAME`

#vscode-yaml-validation

## Description

This is a work in progress/early release version, of a VSCode extension for YAML validation against a JSON schema.

This extension uses schemas defined in VSCode settings.

**.vscode/settings.json**

    "json.schemas": [
      {
        "fileMatch": [ "**/default.json" ],
        "url": "./src/specs/schema/sources/JsonSchema.d4.json"
      },
      {
        "fileMatch": [ "/.babelrc" ],
        "url": "http://json.schemastore.org/babelrc
      },
      {
        "fileMatch": [ "**/swagger.yaml" ],
        "url": "http://json.schemastore.org/swagger-2.0"
      }
    ]

## Contributions

Contents of the /server/src/yaml folder are from the following repos, with modifications:

- https://github.com/mulesoft-labs/yaml-ast-parser
- https://github.com/nodeca/js-yaml

They are included here, because I intend to take major liberties and make further strides towards
conversion to TypeScript, if this effort proves viable.

Contents of the /server/src/json and /client folder are from the following repos, with modifications:

- https://github.com/Microsoft/vscode/tree/master/extensions/json
- https://github.com/Microsoft/vscode-languageserver-node-example

PetStore schemas were from the following repo:

- https://raw.githubusercontent.com/OAI/OpenAPI-Specification/master/examples/v2.0/json/petstore-expanded.json


## License
[MIT](LICENSE.txt)

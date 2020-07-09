# Typescript-Proto

With this library you can generate type-safe interfaces for Typescript based on your protobuf definitions.

## Usage

A cli named `typescript-proto` is exposed and can be used to generate Typescript interfaces.

`typescript-proto -o ${OUTPUT_FILENAME}.ts ${INPUT_FILE}.proto`

Basic usage would be like:

`typescript-proto -o 'output.ts' 'input.proto'`

You can also have several proto files as input parameter:

`typescript-proto -o 'output.ts' 'input1.proto' 'input2.proto'`

When this is combined with the `find`-command, you can simply have all of your proto-files as input parameter:

`` typescript-proto -o 'src/_generated/proto_namespaces.ts' `find '../../../protobuf-definitions' -name '*.proto' -not -path '*/google/*'` ``

### Options

-   --out (-o): pass the output directory.

#### Side Notes

This is actively used and maintained by @Salamantex.

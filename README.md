# ambar-openapi-spec
Official repo for Ambar.cloud OpenAPI Specification. Use this spec to generate a client in your language of choice to get started using Ambar today!

For more information about Ambar resources and general usage, refer to the [Official Ambar docs](https://docs.ambar.cloud)

## Prerequisites:
* [OpenApi-Generator](https://github.com/OpenAPITools/openapi-generator)
* `bash` or shell compatible with running the generator

## Directions:
To use the OpenAPI spec to generate an API client in an arbitrary language:
1. Download the provided `api.yaml` from this repository to the directory where you want the generated client.
2. Refer to details for required and optional flags for your language of choice, and execute the generator. E.G. for `golang` the command would look something like `openapi-generator generate -i api.yaml -g go -o ./go`
3. The generated folder will contain the source files necessary to use the client, as well as documentation and examples.
4. Ensure to instantiate the client such that it will pass your API key via an http header with the key `x-api-key`
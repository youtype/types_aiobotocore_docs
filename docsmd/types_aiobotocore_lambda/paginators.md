# Paginators

> [Index](../README.md) > [Lambda](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListAliases.html#Lambda.Paginator.ListAliases)

```python
# ListAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FunctionName: str,
    FunctionVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAliasesRequestPaginateTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestPaginateTypeDef](./type_defs.md#listaliasesrequestpaginatetypedef) 
## ListCodeSigningConfigsPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_code_signing_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListCodeSigningConfigs.html#Lambda.Paginator.ListCodeSigningConfigs)

```python
# ListCodeSigningConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListCodeSigningConfigsPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListCodeSigningConfigsPaginator = client.get_paginator("list_code_signing_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListCodeSigningConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListCodeSigningConfigsPaginator](./paginators.md#listcodesigningconfigspaginator)
3. item: [:material-code-braces: ListCodeSigningConfigsResponseTypeDef](./type_defs.md#listcodesigningconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCodeSigningConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCodeSigningConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCodeSigningConfigsResponseTypeDef](./type_defs.md#listcodesigningconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCodeSigningConfigsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCodeSigningConfigsRequestPaginateTypeDef](./type_defs.md#listcodesigningconfigsrequestpaginatetypedef) 
## ListEventSourceMappingsPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_event_source_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListEventSourceMappings.html#Lambda.Paginator.ListEventSourceMappings)

```python
# ListEventSourceMappingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListEventSourceMappingsPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListEventSourceMappingsPaginator = client.get_paginator("list_event_source_mappings")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventSourceMappingsResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListEventSourceMappingsPaginator](./paginators.md#listeventsourcemappingspaginator)
3. item: [:material-code-braces: ListEventSourceMappingsResponseTypeDef](./type_defs.md#listeventsourcemappingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventSourceMappingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EventSourceArn: str = ...,
    FunctionName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventSourceMappingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventSourceMappingsResponseTypeDef](./type_defs.md#listeventsourcemappingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventSourceMappingsRequestPaginateTypeDef = {  # (1)
    "EventSourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventSourceMappingsRequestPaginateTypeDef](./type_defs.md#listeventsourcemappingsrequestpaginatetypedef) 
## ListFunctionEventInvokeConfigsPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_function_event_invoke_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListFunctionEventInvokeConfigs.html#Lambda.Paginator.ListFunctionEventInvokeConfigs)

```python
# ListFunctionEventInvokeConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListFunctionEventInvokeConfigsPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListFunctionEventInvokeConfigsPaginator = client.get_paginator("list_function_event_invoke_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionEventInvokeConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListFunctionEventInvokeConfigsPaginator](./paginators.md#listfunctioneventinvokeconfigspaginator)
3. item: [:material-code-braces: ListFunctionEventInvokeConfigsResponseTypeDef](./type_defs.md#listfunctioneventinvokeconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionEventInvokeConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FunctionName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFunctionEventInvokeConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionEventInvokeConfigsResponseTypeDef](./type_defs.md#listfunctioneventinvokeconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFunctionEventInvokeConfigsRequestPaginateTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionEventInvokeConfigsRequestPaginateTypeDef](./type_defs.md#listfunctioneventinvokeconfigsrequestpaginatetypedef) 
## ListFunctionUrlConfigsPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_function_url_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListFunctionUrlConfigs.html#Lambda.Paginator.ListFunctionUrlConfigs)

```python
# ListFunctionUrlConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListFunctionUrlConfigsPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListFunctionUrlConfigsPaginator = client.get_paginator("list_function_url_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionUrlConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListFunctionUrlConfigsPaginator](./paginators.md#listfunctionurlconfigspaginator)
3. item: [:material-code-braces: ListFunctionUrlConfigsResponseTypeDef](./type_defs.md#listfunctionurlconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionUrlConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FunctionName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFunctionUrlConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionUrlConfigsResponseTypeDef](./type_defs.md#listfunctionurlconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFunctionUrlConfigsRequestPaginateTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionUrlConfigsRequestPaginateTypeDef](./type_defs.md#listfunctionurlconfigsrequestpaginatetypedef) 
## ListFunctionsByCodeSigningConfigPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_functions_by_code_signing_config")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListFunctionsByCodeSigningConfig.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig)

```python
# ListFunctionsByCodeSigningConfigPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListFunctionsByCodeSigningConfigPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListFunctionsByCodeSigningConfigPaginator = client.get_paginator("list_functions_by_code_signing_config")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionsByCodeSigningConfigResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListFunctionsByCodeSigningConfigPaginator](./paginators.md#listfunctionsbycodesigningconfigpaginator)
3. item: [:material-code-braces: ListFunctionsByCodeSigningConfigResponseTypeDef](./type_defs.md#listfunctionsbycodesigningconfigresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionsByCodeSigningConfigPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CodeSigningConfigArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFunctionsByCodeSigningConfigResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionsByCodeSigningConfigResponseTypeDef](./type_defs.md#listfunctionsbycodesigningconfigresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFunctionsByCodeSigningConfigRequestPaginateTypeDef = {  # (1)
    "CodeSigningConfigArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionsByCodeSigningConfigRequestPaginateTypeDef](./type_defs.md#listfunctionsbycodesigningconfigrequestpaginatetypedef) 
## ListFunctionsPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_functions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListFunctions.html#Lambda.Paginator.ListFunctions)

```python
# ListFunctionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListFunctionsPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListFunctionsPaginator = client.get_paginator("list_functions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListFunctionsPaginator](./paginators.md#listfunctionspaginator)
3. item: [:material-code-braces: ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MasterRegion: str = ...,
    FunctionVersion: FunctionVersionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListFunctionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FunctionVersionType](./literals.md#functionversiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFunctionsRequestPaginateTypeDef = {  # (1)
    "MasterRegion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionsRequestPaginateTypeDef](./type_defs.md#listfunctionsrequestpaginatetypedef) 
## ListLayerVersionsPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_layer_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListLayerVersions.html#Lambda.Paginator.ListLayerVersions)

```python
# ListLayerVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListLayerVersionsPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListLayerVersionsPaginator = client.get_paginator("list_layer_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLayerVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListLayerVersionsPaginator](./paginators.md#listlayerversionspaginator)
3. item: [:material-code-braces: ListLayerVersionsResponseTypeDef](./type_defs.md#listlayerversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLayerVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LayerName: str,
    CompatibleRuntime: RuntimeType = ...,  # (1)
    CompatibleArchitecture: ArchitectureType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListLayerVersionsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListLayerVersionsResponseTypeDef](./type_defs.md#listlayerversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLayerVersionsRequestPaginateTypeDef = {  # (1)
    "LayerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLayerVersionsRequestPaginateTypeDef](./type_defs.md#listlayerversionsrequestpaginatetypedef) 
## ListLayersPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_layers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListLayers.html#Lambda.Paginator.ListLayers)

```python
# ListLayersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListLayersPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListLayersPaginator = client.get_paginator("list_layers")  # (2)
    async for item in paginator.paginate(...):
        item: ListLayersResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListLayersPaginator](./paginators.md#listlayerspaginator)
3. item: [:material-code-braces: ListLayersResponseTypeDef](./type_defs.md#listlayersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLayersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CompatibleRuntime: RuntimeType = ...,  # (1)
    CompatibleArchitecture: ArchitectureType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListLayersResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListLayersResponseTypeDef](./type_defs.md#listlayersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLayersRequestPaginateTypeDef = {  # (1)
    "CompatibleRuntime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLayersRequestPaginateTypeDef](./type_defs.md#listlayersrequestpaginatetypedef) 
## ListProvisionedConcurrencyConfigsPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_provisioned_concurrency_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListProvisionedConcurrencyConfigs.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs)

```python
# ListProvisionedConcurrencyConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListProvisionedConcurrencyConfigsPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListProvisionedConcurrencyConfigsPaginator = client.get_paginator("list_provisioned_concurrency_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListProvisionedConcurrencyConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListProvisionedConcurrencyConfigsPaginator](./paginators.md#listprovisionedconcurrencyconfigspaginator)
3. item: [:material-code-braces: ListProvisionedConcurrencyConfigsResponseTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProvisionedConcurrencyConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FunctionName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProvisionedConcurrencyConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProvisionedConcurrencyConfigsResponseTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProvisionedConcurrencyConfigsRequestPaginateTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisionedConcurrencyConfigsRequestPaginateTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsrequestpaginatetypedef) 
## ListVersionsByFunctionPaginator

Type annotations and code completion for `#!python session.create_client("lambda").get_paginator("list_versions_by_function")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/paginator/ListVersionsByFunction.html#Lambda.Paginator.ListVersionsByFunction)

```python
# ListVersionsByFunctionPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lambda.paginator import ListVersionsByFunctionPaginator

session = get_session()
async with session.create_client("lambda") as client:  # (1)
    paginator: ListVersionsByFunctionPaginator = client.get_paginator("list_versions_by_function")  # (2)
    async for item in paginator.paginate(...):
        item: ListVersionsByFunctionResponseTypeDef
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListVersionsByFunctionPaginator](./paginators.md#listversionsbyfunctionpaginator)
3. item: [:material-code-braces: ListVersionsByFunctionResponseTypeDef](./type_defs.md#listversionsbyfunctionresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVersionsByFunctionPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FunctionName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListVersionsByFunctionResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVersionsByFunctionResponseTypeDef](./type_defs.md#listversionsbyfunctionresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVersionsByFunctionRequestPaginateTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVersionsByFunctionRequestPaginateTypeDef](./type_defs.md#listversionsbyfunctionrequestpaginatetypedef) 

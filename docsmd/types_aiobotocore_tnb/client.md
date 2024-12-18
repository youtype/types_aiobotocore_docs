# TelcoNetworkBuilderClient

> [Index](../README.md) > [TelcoNetworkBuilder](./README.md) > TelcoNetworkBuilderClient

!!! note ""

    Auto-generated documentation for [TelcoNetworkBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#telconetworkbuilder)
    type annotations stubs module [types-aiobotocore-tnb](https://pypi.org/project/types-aiobotocore-tnb/).

## TelcoNetworkBuilderClient

Type annotations and code completion for `#!python session.create_client("tnb")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client)

```python
# TelcoNetworkBuilderClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_tnb.client import TelcoNetworkBuilderClient

session = get_session()
async with session.create_client("tnb") as client:
    client: TelcoNetworkBuilderClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("tnb").exceptions` structure.

```python
# TelcoNetworkBuilderClient.exceptions usage example

async with session.create_client("tnb") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# TelcoNetworkBuilderClient usage type checking example

from types_aiobotocore_tnb.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("tnb").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("tnb").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("tnb").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### cancel\_sol\_network\_operation

Cancels a network operation.

Type annotations and code completion for `#!python session.create_client("tnb").cancel_sol_network_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/cancel_sol_network_operation.html)

```python
# cancel_sol_network_operation method definition

await def cancel_sol_network_operation(
    self,
    *,
    nsLcmOpOccId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_sol_network_operation method usage example with argument unpacking

kwargs: CancelSolNetworkOperationInputRequestTypeDef = {  # (1)
    "nsLcmOpOccId": ...,
}

parent.cancel_sol_network_operation(**kwargs)
```

1. See [:material-code-braces: CancelSolNetworkOperationInputRequestTypeDef](./type_defs.md#cancelsolnetworkoperationinputrequesttypedef) 

### create\_sol\_function\_package

Creates a function package.

Type annotations and code completion for `#!python session.create_client("tnb").create_sol_function_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/create_sol_function_package.html)

```python
# create_sol_function_package method definition

await def create_sol_function_package(
    self,
    *,
    tags: Mapping[str, str] = ...,
) -> CreateSolFunctionPackageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSolFunctionPackageOutputTypeDef](./type_defs.md#createsolfunctionpackageoutputtypedef) 


```python
# create_sol_function_package method usage example with argument unpacking

kwargs: CreateSolFunctionPackageInputRequestTypeDef = {  # (1)
    "tags": ...,
}

parent.create_sol_function_package(**kwargs)
```

1. See [:material-code-braces: CreateSolFunctionPackageInputRequestTypeDef](./type_defs.md#createsolfunctionpackageinputrequesttypedef) 

### create\_sol\_network\_instance

Creates a network instance.

Type annotations and code completion for `#!python session.create_client("tnb").create_sol_network_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/create_sol_network_instance.html)

```python
# create_sol_network_instance method definition

await def create_sol_network_instance(
    self,
    *,
    nsName: str,
    nsdInfoId: str,
    nsDescription: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateSolNetworkInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSolNetworkInstanceOutputTypeDef](./type_defs.md#createsolnetworkinstanceoutputtypedef) 


```python
# create_sol_network_instance method usage example with argument unpacking

kwargs: CreateSolNetworkInstanceInputRequestTypeDef = {  # (1)
    "nsName": ...,
    "nsdInfoId": ...,
}

parent.create_sol_network_instance(**kwargs)
```

1. See [:material-code-braces: CreateSolNetworkInstanceInputRequestTypeDef](./type_defs.md#createsolnetworkinstanceinputrequesttypedef) 

### create\_sol\_network\_package

Creates a network package.

Type annotations and code completion for `#!python session.create_client("tnb").create_sol_network_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/create_sol_network_package.html)

```python
# create_sol_network_package method definition

await def create_sol_network_package(
    self,
    *,
    tags: Mapping[str, str] = ...,
) -> CreateSolNetworkPackageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSolNetworkPackageOutputTypeDef](./type_defs.md#createsolnetworkpackageoutputtypedef) 


```python
# create_sol_network_package method usage example with argument unpacking

kwargs: CreateSolNetworkPackageInputRequestTypeDef = {  # (1)
    "tags": ...,
}

parent.create_sol_network_package(**kwargs)
```

1. See [:material-code-braces: CreateSolNetworkPackageInputRequestTypeDef](./type_defs.md#createsolnetworkpackageinputrequesttypedef) 

### delete\_sol\_function\_package

Deletes a function package.

Type annotations and code completion for `#!python session.create_client("tnb").delete_sol_function_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/delete_sol_function_package.html)

```python
# delete_sol_function_package method definition

await def delete_sol_function_package(
    self,
    *,
    vnfPkgId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_sol_function_package method usage example with argument unpacking

kwargs: DeleteSolFunctionPackageInputRequestTypeDef = {  # (1)
    "vnfPkgId": ...,
}

parent.delete_sol_function_package(**kwargs)
```

1. See [:material-code-braces: DeleteSolFunctionPackageInputRequestTypeDef](./type_defs.md#deletesolfunctionpackageinputrequesttypedef) 

### delete\_sol\_network\_instance

Deletes a network instance.

Type annotations and code completion for `#!python session.create_client("tnb").delete_sol_network_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/delete_sol_network_instance.html)

```python
# delete_sol_network_instance method definition

await def delete_sol_network_instance(
    self,
    *,
    nsInstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_sol_network_instance method usage example with argument unpacking

kwargs: DeleteSolNetworkInstanceInputRequestTypeDef = {  # (1)
    "nsInstanceId": ...,
}

parent.delete_sol_network_instance(**kwargs)
```

1. See [:material-code-braces: DeleteSolNetworkInstanceInputRequestTypeDef](./type_defs.md#deletesolnetworkinstanceinputrequesttypedef) 

### delete\_sol\_network\_package

Deletes network package.

Type annotations and code completion for `#!python session.create_client("tnb").delete_sol_network_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/delete_sol_network_package.html)

```python
# delete_sol_network_package method definition

await def delete_sol_network_package(
    self,
    *,
    nsdInfoId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_sol_network_package method usage example with argument unpacking

kwargs: DeleteSolNetworkPackageInputRequestTypeDef = {  # (1)
    "nsdInfoId": ...,
}

parent.delete_sol_network_package(**kwargs)
```

1. See [:material-code-braces: DeleteSolNetworkPackageInputRequestTypeDef](./type_defs.md#deletesolnetworkpackageinputrequesttypedef) 

### get\_sol\_function\_instance

Gets the details of a network function instance, including the instantiation
state and metadata from the function package descriptor in the network function
package.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_function_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_function_instance.html)

```python
# get_sol_function_instance method definition

await def get_sol_function_instance(
    self,
    *,
    vnfInstanceId: str,
) -> GetSolFunctionInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSolFunctionInstanceOutputTypeDef](./type_defs.md#getsolfunctioninstanceoutputtypedef) 


```python
# get_sol_function_instance method usage example with argument unpacking

kwargs: GetSolFunctionInstanceInputRequestTypeDef = {  # (1)
    "vnfInstanceId": ...,
}

parent.get_sol_function_instance(**kwargs)
```

1. See [:material-code-braces: GetSolFunctionInstanceInputRequestTypeDef](./type_defs.md#getsolfunctioninstanceinputrequesttypedef) 

### get\_sol\_function\_package

Gets the details of an individual function package, such as the operational
state and whether the package is in use.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_function_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_function_package.html)

```python
# get_sol_function_package method definition

await def get_sol_function_package(
    self,
    *,
    vnfPkgId: str,
) -> GetSolFunctionPackageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSolFunctionPackageOutputTypeDef](./type_defs.md#getsolfunctionpackageoutputtypedef) 


```python
# get_sol_function_package method usage example with argument unpacking

kwargs: GetSolFunctionPackageInputRequestTypeDef = {  # (1)
    "vnfPkgId": ...,
}

parent.get_sol_function_package(**kwargs)
```

1. See [:material-code-braces: GetSolFunctionPackageInputRequestTypeDef](./type_defs.md#getsolfunctionpackageinputrequesttypedef) 

### get\_sol\_function\_package\_content

Gets the contents of a function package.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_function_package_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_function_package_content.html)

```python
# get_sol_function_package_content method definition

await def get_sol_function_package_content(
    self,
    *,
    accept: PackageContentTypeType,  # (1)
    vnfPkgId: str,
) -> GetSolFunctionPackageContentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PackageContentTypeType](./literals.md#packagecontenttypetype) 
2. See [:material-code-braces: GetSolFunctionPackageContentOutputTypeDef](./type_defs.md#getsolfunctionpackagecontentoutputtypedef) 


```python
# get_sol_function_package_content method usage example with argument unpacking

kwargs: GetSolFunctionPackageContentInputRequestTypeDef = {  # (1)
    "accept": ...,
    "vnfPkgId": ...,
}

parent.get_sol_function_package_content(**kwargs)
```

1. See [:material-code-braces: GetSolFunctionPackageContentInputRequestTypeDef](./type_defs.md#getsolfunctionpackagecontentinputrequesttypedef) 

### get\_sol\_function\_package\_descriptor

Gets a function package descriptor in a function package.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_function_package_descriptor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_function_package_descriptor.html)

```python
# get_sol_function_package_descriptor method definition

await def get_sol_function_package_descriptor(
    self,
    *,
    accept: DescriptorContentTypeType,  # (1)
    vnfPkgId: str,
) -> GetSolFunctionPackageDescriptorOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DescriptorContentTypeType](./literals.md#descriptorcontenttypetype) 
2. See [:material-code-braces: GetSolFunctionPackageDescriptorOutputTypeDef](./type_defs.md#getsolfunctionpackagedescriptoroutputtypedef) 


```python
# get_sol_function_package_descriptor method usage example with argument unpacking

kwargs: GetSolFunctionPackageDescriptorInputRequestTypeDef = {  # (1)
    "accept": ...,
    "vnfPkgId": ...,
}

parent.get_sol_function_package_descriptor(**kwargs)
```

1. See [:material-code-braces: GetSolFunctionPackageDescriptorInputRequestTypeDef](./type_defs.md#getsolfunctionpackagedescriptorinputrequesttypedef) 

### get\_sol\_network\_instance

Gets the details of the network instance.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_network_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_network_instance.html)

```python
# get_sol_network_instance method definition

await def get_sol_network_instance(
    self,
    *,
    nsInstanceId: str,
) -> GetSolNetworkInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSolNetworkInstanceOutputTypeDef](./type_defs.md#getsolnetworkinstanceoutputtypedef) 


```python
# get_sol_network_instance method usage example with argument unpacking

kwargs: GetSolNetworkInstanceInputRequestTypeDef = {  # (1)
    "nsInstanceId": ...,
}

parent.get_sol_network_instance(**kwargs)
```

1. See [:material-code-braces: GetSolNetworkInstanceInputRequestTypeDef](./type_defs.md#getsolnetworkinstanceinputrequesttypedef) 

### get\_sol\_network\_operation

Gets the details of a network operation, including the tasks involved in the
network operation and the status of the tasks.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_network_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_network_operation.html)

```python
# get_sol_network_operation method definition

await def get_sol_network_operation(
    self,
    *,
    nsLcmOpOccId: str,
) -> GetSolNetworkOperationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSolNetworkOperationOutputTypeDef](./type_defs.md#getsolnetworkoperationoutputtypedef) 


```python
# get_sol_network_operation method usage example with argument unpacking

kwargs: GetSolNetworkOperationInputRequestTypeDef = {  # (1)
    "nsLcmOpOccId": ...,
}

parent.get_sol_network_operation(**kwargs)
```

1. See [:material-code-braces: GetSolNetworkOperationInputRequestTypeDef](./type_defs.md#getsolnetworkoperationinputrequesttypedef) 

### get\_sol\_network\_package

Gets the details of a network package.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_network_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_network_package.html)

```python
# get_sol_network_package method definition

await def get_sol_network_package(
    self,
    *,
    nsdInfoId: str,
) -> GetSolNetworkPackageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSolNetworkPackageOutputTypeDef](./type_defs.md#getsolnetworkpackageoutputtypedef) 


```python
# get_sol_network_package method usage example with argument unpacking

kwargs: GetSolNetworkPackageInputRequestTypeDef = {  # (1)
    "nsdInfoId": ...,
}

parent.get_sol_network_package(**kwargs)
```

1. See [:material-code-braces: GetSolNetworkPackageInputRequestTypeDef](./type_defs.md#getsolnetworkpackageinputrequesttypedef) 

### get\_sol\_network\_package\_content

Gets the contents of a network package.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_network_package_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_network_package_content.html)

```python
# get_sol_network_package_content method definition

await def get_sol_network_package_content(
    self,
    *,
    accept: PackageContentTypeType,  # (1)
    nsdInfoId: str,
) -> GetSolNetworkPackageContentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PackageContentTypeType](./literals.md#packagecontenttypetype) 
2. See [:material-code-braces: GetSolNetworkPackageContentOutputTypeDef](./type_defs.md#getsolnetworkpackagecontentoutputtypedef) 


```python
# get_sol_network_package_content method usage example with argument unpacking

kwargs: GetSolNetworkPackageContentInputRequestTypeDef = {  # (1)
    "accept": ...,
    "nsdInfoId": ...,
}

parent.get_sol_network_package_content(**kwargs)
```

1. See [:material-code-braces: GetSolNetworkPackageContentInputRequestTypeDef](./type_defs.md#getsolnetworkpackagecontentinputrequesttypedef) 

### get\_sol\_network\_package\_descriptor

Gets the content of the network service descriptor.

Type annotations and code completion for `#!python session.create_client("tnb").get_sol_network_package_descriptor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/get_sol_network_package_descriptor.html)

```python
# get_sol_network_package_descriptor method definition

await def get_sol_network_package_descriptor(
    self,
    *,
    nsdInfoId: str,
) -> GetSolNetworkPackageDescriptorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSolNetworkPackageDescriptorOutputTypeDef](./type_defs.md#getsolnetworkpackagedescriptoroutputtypedef) 


```python
# get_sol_network_package_descriptor method usage example with argument unpacking

kwargs: GetSolNetworkPackageDescriptorInputRequestTypeDef = {  # (1)
    "nsdInfoId": ...,
}

parent.get_sol_network_package_descriptor(**kwargs)
```

1. See [:material-code-braces: GetSolNetworkPackageDescriptorInputRequestTypeDef](./type_defs.md#getsolnetworkpackagedescriptorinputrequesttypedef) 

### instantiate\_sol\_network\_instance

Instantiates a network instance.

Type annotations and code completion for `#!python session.create_client("tnb").instantiate_sol_network_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/instantiate_sol_network_instance.html)

```python
# instantiate_sol_network_instance method definition

await def instantiate_sol_network_instance(
    self,
    *,
    nsInstanceId: str,
    additionalParamsForNs: Mapping[str, Any] = ...,
    dryRun: bool = ...,
    tags: Mapping[str, str] = ...,
) -> InstantiateSolNetworkInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InstantiateSolNetworkInstanceOutputTypeDef](./type_defs.md#instantiatesolnetworkinstanceoutputtypedef) 


```python
# instantiate_sol_network_instance method usage example with argument unpacking

kwargs: InstantiateSolNetworkInstanceInputRequestTypeDef = {  # (1)
    "nsInstanceId": ...,
}

parent.instantiate_sol_network_instance(**kwargs)
```

1. See [:material-code-braces: InstantiateSolNetworkInstanceInputRequestTypeDef](./type_defs.md#instantiatesolnetworkinstanceinputrequesttypedef) 

### list\_sol\_function\_instances

Lists network function instances.

Type annotations and code completion for `#!python session.create_client("tnb").list_sol_function_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/list_sol_function_instances.html)

```python
# list_sol_function_instances method definition

await def list_sol_function_instances(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSolFunctionInstancesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSolFunctionInstancesOutputTypeDef](./type_defs.md#listsolfunctioninstancesoutputtypedef) 


```python
# list_sol_function_instances method usage example with argument unpacking

kwargs: ListSolFunctionInstancesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_sol_function_instances(**kwargs)
```

1. See [:material-code-braces: ListSolFunctionInstancesInputRequestTypeDef](./type_defs.md#listsolfunctioninstancesinputrequesttypedef) 

### list\_sol\_function\_packages

Lists information about function packages.

Type annotations and code completion for `#!python session.create_client("tnb").list_sol_function_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/list_sol_function_packages.html)

```python
# list_sol_function_packages method definition

await def list_sol_function_packages(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSolFunctionPackagesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSolFunctionPackagesOutputTypeDef](./type_defs.md#listsolfunctionpackagesoutputtypedef) 


```python
# list_sol_function_packages method usage example with argument unpacking

kwargs: ListSolFunctionPackagesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_sol_function_packages(**kwargs)
```

1. See [:material-code-braces: ListSolFunctionPackagesInputRequestTypeDef](./type_defs.md#listsolfunctionpackagesinputrequesttypedef) 

### list\_sol\_network\_instances

Lists your network instances.

Type annotations and code completion for `#!python session.create_client("tnb").list_sol_network_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/list_sol_network_instances.html)

```python
# list_sol_network_instances method definition

await def list_sol_network_instances(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSolNetworkInstancesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSolNetworkInstancesOutputTypeDef](./type_defs.md#listsolnetworkinstancesoutputtypedef) 


```python
# list_sol_network_instances method usage example with argument unpacking

kwargs: ListSolNetworkInstancesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_sol_network_instances(**kwargs)
```

1. See [:material-code-braces: ListSolNetworkInstancesInputRequestTypeDef](./type_defs.md#listsolnetworkinstancesinputrequesttypedef) 

### list\_sol\_network\_operations

Lists details for a network operation, including when the operation started and
the status of the operation.

Type annotations and code completion for `#!python session.create_client("tnb").list_sol_network_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/list_sol_network_operations.html)

```python
# list_sol_network_operations method definition

await def list_sol_network_operations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    nsInstanceId: str = ...,
) -> ListSolNetworkOperationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSolNetworkOperationsOutputTypeDef](./type_defs.md#listsolnetworkoperationsoutputtypedef) 


```python
# list_sol_network_operations method usage example with argument unpacking

kwargs: ListSolNetworkOperationsInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_sol_network_operations(**kwargs)
```

1. See [:material-code-braces: ListSolNetworkOperationsInputRequestTypeDef](./type_defs.md#listsolnetworkoperationsinputrequesttypedef) 

### list\_sol\_network\_packages

Lists network packages.

Type annotations and code completion for `#!python session.create_client("tnb").list_sol_network_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/list_sol_network_packages.html)

```python
# list_sol_network_packages method definition

await def list_sol_network_packages(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSolNetworkPackagesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSolNetworkPackagesOutputTypeDef](./type_defs.md#listsolnetworkpackagesoutputtypedef) 


```python
# list_sol_network_packages method usage example with argument unpacking

kwargs: ListSolNetworkPackagesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_sol_network_packages(**kwargs)
```

1. See [:material-code-braces: ListSolNetworkPackagesInputRequestTypeDef](./type_defs.md#listsolnetworkpackagesinputrequesttypedef) 

### list\_tags\_for\_resource

Lists tags for AWS TNB resources.

Type annotations and code completion for `#!python session.create_client("tnb").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### put\_sol\_function\_package\_content

Uploads the contents of a function package.

Type annotations and code completion for `#!python session.create_client("tnb").put_sol_function_package_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/put_sol_function_package_content.html)

```python
# put_sol_function_package_content method definition

await def put_sol_function_package_content(
    self,
    *,
    file: BlobTypeDef,
    vnfPkgId: str,
    contentType: PackageContentTypeType = ...,  # (1)
) -> PutSolFunctionPackageContentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PackageContentTypeType](./literals.md#packagecontenttypetype) 
2. See [:material-code-braces: PutSolFunctionPackageContentOutputTypeDef](./type_defs.md#putsolfunctionpackagecontentoutputtypedef) 


```python
# put_sol_function_package_content method usage example with argument unpacking

kwargs: PutSolFunctionPackageContentInputRequestTypeDef = {  # (1)
    "file": ...,
    "vnfPkgId": ...,
}

parent.put_sol_function_package_content(**kwargs)
```

1. See [:material-code-braces: PutSolFunctionPackageContentInputRequestTypeDef](./type_defs.md#putsolfunctionpackagecontentinputrequesttypedef) 

### put\_sol\_network\_package\_content

Uploads the contents of a network package.

Type annotations and code completion for `#!python session.create_client("tnb").put_sol_network_package_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/put_sol_network_package_content.html)

```python
# put_sol_network_package_content method definition

await def put_sol_network_package_content(
    self,
    *,
    file: BlobTypeDef,
    nsdInfoId: str,
    contentType: PackageContentTypeType = ...,  # (1)
) -> PutSolNetworkPackageContentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PackageContentTypeType](./literals.md#packagecontenttypetype) 
2. See [:material-code-braces: PutSolNetworkPackageContentOutputTypeDef](./type_defs.md#putsolnetworkpackagecontentoutputtypedef) 


```python
# put_sol_network_package_content method usage example with argument unpacking

kwargs: PutSolNetworkPackageContentInputRequestTypeDef = {  # (1)
    "file": ...,
    "nsdInfoId": ...,
}

parent.put_sol_network_package_content(**kwargs)
```

1. See [:material-code-braces: PutSolNetworkPackageContentInputRequestTypeDef](./type_defs.md#putsolnetworkpackagecontentinputrequesttypedef) 

### tag\_resource

Tags an AWS TNB resource.

Type annotations and code completion for `#!python session.create_client("tnb").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### terminate\_sol\_network\_instance

Terminates a network instance.

Type annotations and code completion for `#!python session.create_client("tnb").terminate_sol_network_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/terminate_sol_network_instance.html)

```python
# terminate_sol_network_instance method definition

await def terminate_sol_network_instance(
    self,
    *,
    nsInstanceId: str,
    tags: Mapping[str, str] = ...,
) -> TerminateSolNetworkInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TerminateSolNetworkInstanceOutputTypeDef](./type_defs.md#terminatesolnetworkinstanceoutputtypedef) 


```python
# terminate_sol_network_instance method usage example with argument unpacking

kwargs: TerminateSolNetworkInstanceInputRequestTypeDef = {  # (1)
    "nsInstanceId": ...,
}

parent.terminate_sol_network_instance(**kwargs)
```

1. See [:material-code-braces: TerminateSolNetworkInstanceInputRequestTypeDef](./type_defs.md#terminatesolnetworkinstanceinputrequesttypedef) 

### untag\_resource

Untags an AWS TNB resource.

Type annotations and code completion for `#!python session.create_client("tnb").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_sol\_function\_package

Updates the operational state of function package.

Type annotations and code completion for `#!python session.create_client("tnb").update_sol_function_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/update_sol_function_package.html)

```python
# update_sol_function_package method definition

await def update_sol_function_package(
    self,
    *,
    operationalState: OperationalStateType,  # (1)
    vnfPkgId: str,
) -> UpdateSolFunctionPackageOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OperationalStateType](./literals.md#operationalstatetype) 
2. See [:material-code-braces: UpdateSolFunctionPackageOutputTypeDef](./type_defs.md#updatesolfunctionpackageoutputtypedef) 


```python
# update_sol_function_package method usage example with argument unpacking

kwargs: UpdateSolFunctionPackageInputRequestTypeDef = {  # (1)
    "operationalState": ...,
    "vnfPkgId": ...,
}

parent.update_sol_function_package(**kwargs)
```

1. See [:material-code-braces: UpdateSolFunctionPackageInputRequestTypeDef](./type_defs.md#updatesolfunctionpackageinputrequesttypedef) 

### update\_sol\_network\_instance

Update a network instance.

Type annotations and code completion for `#!python session.create_client("tnb").update_sol_network_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/update_sol_network_instance.html)

```python
# update_sol_network_instance method definition

await def update_sol_network_instance(
    self,
    *,
    nsInstanceId: str,
    updateType: UpdateSolNetworkTypeType,  # (1)
    modifyVnfInfoData: UpdateSolNetworkModifyTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    updateNs: UpdateSolNetworkServiceDataTypeDef = ...,  # (3)
) -> UpdateSolNetworkInstanceOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: UpdateSolNetworkTypeType](./literals.md#updatesolnetworktypetype) 
2. See [:material-code-braces: UpdateSolNetworkModifyTypeDef](./type_defs.md#updatesolnetworkmodifytypedef) 
3. See [:material-code-braces: UpdateSolNetworkServiceDataTypeDef](./type_defs.md#updatesolnetworkservicedatatypedef) 
4. See [:material-code-braces: UpdateSolNetworkInstanceOutputTypeDef](./type_defs.md#updatesolnetworkinstanceoutputtypedef) 


```python
# update_sol_network_instance method usage example with argument unpacking

kwargs: UpdateSolNetworkInstanceInputRequestTypeDef = {  # (1)
    "nsInstanceId": ...,
    "updateType": ...,
}

parent.update_sol_network_instance(**kwargs)
```

1. See [:material-code-braces: UpdateSolNetworkInstanceInputRequestTypeDef](./type_defs.md#updatesolnetworkinstanceinputrequesttypedef) 

### update\_sol\_network\_package

Updates the operational state of a network package.

Type annotations and code completion for `#!python session.create_client("tnb").update_sol_network_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/update_sol_network_package.html)

```python
# update_sol_network_package method definition

await def update_sol_network_package(
    self,
    *,
    nsdInfoId: str,
    nsdOperationalState: NsdOperationalStateType,  # (1)
) -> UpdateSolNetworkPackageOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NsdOperationalStateType](./literals.md#nsdoperationalstatetype) 
2. See [:material-code-braces: UpdateSolNetworkPackageOutputTypeDef](./type_defs.md#updatesolnetworkpackageoutputtypedef) 


```python
# update_sol_network_package method usage example with argument unpacking

kwargs: UpdateSolNetworkPackageInputRequestTypeDef = {  # (1)
    "nsdInfoId": ...,
    "nsdOperationalState": ...,
}

parent.update_sol_network_package(**kwargs)
```

1. See [:material-code-braces: UpdateSolNetworkPackageInputRequestTypeDef](./type_defs.md#updatesolnetworkpackageinputrequesttypedef) 

### validate\_sol\_function\_package\_content

Validates function package content.

Type annotations and code completion for `#!python session.create_client("tnb").validate_sol_function_package_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/validate_sol_function_package_content.html)

```python
# validate_sol_function_package_content method definition

await def validate_sol_function_package_content(
    self,
    *,
    file: BlobTypeDef,
    vnfPkgId: str,
    contentType: PackageContentTypeType = ...,  # (1)
) -> ValidateSolFunctionPackageContentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PackageContentTypeType](./literals.md#packagecontenttypetype) 
2. See [:material-code-braces: ValidateSolFunctionPackageContentOutputTypeDef](./type_defs.md#validatesolfunctionpackagecontentoutputtypedef) 


```python
# validate_sol_function_package_content method usage example with argument unpacking

kwargs: ValidateSolFunctionPackageContentInputRequestTypeDef = {  # (1)
    "file": ...,
    "vnfPkgId": ...,
}

parent.validate_sol_function_package_content(**kwargs)
```

1. See [:material-code-braces: ValidateSolFunctionPackageContentInputRequestTypeDef](./type_defs.md#validatesolfunctionpackagecontentinputrequesttypedef) 

### validate\_sol\_network\_package\_content

Validates network package content.

Type annotations and code completion for `#!python session.create_client("tnb").validate_sol_network_package_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb/client/validate_sol_network_package_content.html)

```python
# validate_sol_network_package_content method definition

await def validate_sol_network_package_content(
    self,
    *,
    file: BlobTypeDef,
    nsdInfoId: str,
    contentType: PackageContentTypeType = ...,  # (1)
) -> ValidateSolNetworkPackageContentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PackageContentTypeType](./literals.md#packagecontenttypetype) 
2. See [:material-code-braces: ValidateSolNetworkPackageContentOutputTypeDef](./type_defs.md#validatesolnetworkpackagecontentoutputtypedef) 


```python
# validate_sol_network_package_content method usage example with argument unpacking

kwargs: ValidateSolNetworkPackageContentInputRequestTypeDef = {  # (1)
    "file": ...,
    "nsdInfoId": ...,
}

parent.validate_sol_network_package_content(**kwargs)
```

1. See [:material-code-braces: ValidateSolNetworkPackageContentInputRequestTypeDef](./type_defs.md#validatesolnetworkpackagecontentinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("tnb").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "TelcoNetworkBuilderClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("tnb").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("tnb").get_paginator` method with overloads.

- `client.get_paginator("list_sol_function_instances")` -> [ListSolFunctionInstancesPaginator](./paginators.md#listsolfunctioninstancespaginator)
- `client.get_paginator("list_sol_function_packages")` -> [ListSolFunctionPackagesPaginator](./paginators.md#listsolfunctionpackagespaginator)
- `client.get_paginator("list_sol_network_instances")` -> [ListSolNetworkInstancesPaginator](./paginators.md#listsolnetworkinstancespaginator)
- `client.get_paginator("list_sol_network_operations")` -> [ListSolNetworkOperationsPaginator](./paginators.md#listsolnetworkoperationspaginator)
- `client.get_paginator("list_sol_network_packages")` -> [ListSolNetworkPackagesPaginator](./paginators.md#listsolnetworkpackagespaginator)




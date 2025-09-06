# CloudControlApi module

> [Index](../README.md) > CloudControlApi


!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#cloudcontrolapi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudControlApi` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudControlApi` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudcontrol]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudcontrol]'

# standalone installation
python -m pip install types-aiobotocore-cloudcontrol
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudcontrol
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudControlApiClient

Type annotations and code completion for  `#!python session.create_client("cloudcontrol")` as [CloudControlApiClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client)

```python
# CloudControlApiClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudcontrol.client import CloudControlApiClient


session = get_session()
async with session.create_client("cloudcontrol") as client:
    client: CloudControlApiClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloudcontrol").get_paginator("...")`.

```python
# ListResourceRequestsPaginator usage example

from types_aiobotocore_cloudcontrol.paginator import ListResourceRequestsPaginator

def get_list_resource_requests_paginator() -> ListResourceRequestsPaginator:
    return client.get_paginator("list_resource_requests"))
```

- [ListResourceRequestsPaginator](./paginators.md#listresourcerequestspaginator)
- [ListResourcesPaginator](./paginators.md#listresourcespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("cloudcontrol").get_waiter("...")`.

```python
# ResourceRequestSuccessWaiter usage example

from types_aiobotocore_cloudcontrol.waiter import ResourceRequestSuccessWaiter

def get_resource_request_success_waiter() -> ResourceRequestSuccessWaiter:
    return Session().client("cloudcontrol").get_waiter("resource_request_success")
```

- [ResourceRequestSuccessWaiter](./waiters.md#resourcerequestsuccesswaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# HandlerErrorCodeType usage example

from types_aiobotocore_cloudcontrol.literals import HandlerErrorCodeType

def get_value() -> HandlerErrorCodeType:
    return "AccessDenied"
```

- [HandlerErrorCodeType](./literals.md#handlererrorcodetype)
- [ListResourceRequestsPaginatorName](./literals.md#listresourcerequestspaginatorname)
- [ListResourcesPaginatorName](./literals.md#listresourcespaginatorname)
- [OperationStatusType](./literals.md#operationstatustype)
- [OperationType](./literals.md#operationtype)
- [ResourceRequestSuccessWaiterName](./literals.md#resourcerequestsuccesswaitername)
- [CloudControlApiServiceName](./literals.md#cloudcontrolapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CancelResourceRequestInputTypeDef](./type_defs.md#cancelresourcerequestinputtypedef)
- [ProgressEventTypeDef](./type_defs.md#progresseventtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateResourceInputTypeDef](./type_defs.md#createresourceinputtypedef)
- [DeleteResourceInputTypeDef](./type_defs.md#deleteresourceinputtypedef)
- [GetResourceInputTypeDef](./type_defs.md#getresourceinputtypedef)
- [ResourceDescriptionTypeDef](./type_defs.md#resourcedescriptiontypedef)
- [GetResourceRequestStatusInputTypeDef](./type_defs.md#getresourcerequeststatusinputtypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [HookProgressEventTypeDef](./type_defs.md#hookprogresseventtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef)
- [ListResourcesInputTypeDef](./type_defs.md#listresourcesinputtypedef)
- [UpdateResourceInputTypeDef](./type_defs.md#updateresourceinputtypedef)
- [CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef)
- [CreateResourceOutputTypeDef](./type_defs.md#createresourceoutputtypedef)
- [DeleteResourceOutputTypeDef](./type_defs.md#deleteresourceoutputtypedef)
- [ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef)
- [UpdateResourceOutputTypeDef](./type_defs.md#updateresourceoutputtypedef)
- [GetResourceOutputTypeDef](./type_defs.md#getresourceoutputtypedef)
- [ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef)
- [GetResourceRequestStatusInputWaitTypeDef](./type_defs.md#getresourcerequeststatusinputwaittypedef)
- [GetResourceRequestStatusOutputTypeDef](./type_defs.md#getresourcerequeststatusoutputtypedef)
- [ListResourcesInputPaginateTypeDef](./type_defs.md#listresourcesinputpaginatetypedef)
- [ListResourceRequestsInputPaginateTypeDef](./type_defs.md#listresourcerequestsinputpaginatetypedef)
- [ListResourceRequestsInputTypeDef](./type_defs.md#listresourcerequestsinputtypedef)


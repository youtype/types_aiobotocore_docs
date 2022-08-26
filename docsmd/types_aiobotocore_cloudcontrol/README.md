# CloudControlApi module

> [Index](../README.md) > CloudControlApi


!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

## How to install



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

```python title="Usage example"
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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_cloudcontrol.waiter import ResourceRequestSuccessWaiter

def get_resource_request_success_waiter() -> ResourceRequestSuccessWaiter:
    return Session().client("cloudcontrol").get_waiter("resource_request_success")
```

- [ResourceRequestSuccessWaiter](./waiters.md#resourcerequestsuccesswaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
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




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputRequestTypeDef

def get_value() -> CancelResourceRequestInputRequestTypeDef:
    return {
        "RequestToken": ...,
    }
```

- [CancelResourceRequestInputRequestTypeDef](./type_defs.md#cancelresourcerequestinputrequesttypedef)
- [ProgressEventTypeDef](./type_defs.md#progresseventtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateResourceInputRequestTypeDef](./type_defs.md#createresourceinputrequesttypedef)
- [DeleteResourceInputRequestTypeDef](./type_defs.md#deleteresourceinputrequesttypedef)
- [GetResourceInputRequestTypeDef](./type_defs.md#getresourceinputrequesttypedef)
- [ResourceDescriptionTypeDef](./type_defs.md#resourcedescriptiontypedef)
- [GetResourceRequestStatusInputRequestTypeDef](./type_defs.md#getresourcerequeststatusinputrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef)
- [ListResourcesInputRequestTypeDef](./type_defs.md#listresourcesinputrequesttypedef)
- [UpdateResourceInputRequestTypeDef](./type_defs.md#updateresourceinputrequesttypedef)
- [CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef)
- [CreateResourceOutputTypeDef](./type_defs.md#createresourceoutputtypedef)
- [DeleteResourceOutputTypeDef](./type_defs.md#deleteresourceoutputtypedef)
- [GetResourceRequestStatusOutputTypeDef](./type_defs.md#getresourcerequeststatusoutputtypedef)
- [ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef)
- [UpdateResourceOutputTypeDef](./type_defs.md#updateresourceoutputtypedef)
- [GetResourceOutputTypeDef](./type_defs.md#getresourceoutputtypedef)
- [ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef)
- [GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef](./type_defs.md#getresourcerequeststatusinputresourcerequestsuccesswaittypedef)
- [ListResourcesInputListResourcesPaginateTypeDef](./type_defs.md#listresourcesinputlistresourcespaginatetypedef)
- [ListResourceRequestsInputListResourceRequestsPaginateTypeDef](./type_defs.md#listresourcerequestsinputlistresourcerequestspaginatetypedef)
- [ListResourceRequestsInputRequestTypeDef](./type_defs.md#listresourcerequestsinputrequesttypedef)


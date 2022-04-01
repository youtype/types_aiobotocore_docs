# CloudControlApi module

> [Index](../README.md) > CloudControlApi


!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `CloudControlApi`.

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
- [OperationStatusType](./literals.md#operationstatustype)
- [OperationType](./literals.md#operationtype)
- [ResourceRequestSuccessWaiterName](./literals.md#resourcerequestsuccesswaitername)
- [CloudControlApiServiceName](./literals.md#cloudcontrolapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
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
- [CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef)
- [CreateResourceInputRequestTypeDef](./type_defs.md#createresourceinputrequesttypedef)
- [CreateResourceOutputTypeDef](./type_defs.md#createresourceoutputtypedef)
- [DeleteResourceInputRequestTypeDef](./type_defs.md#deleteresourceinputrequesttypedef)
- [DeleteResourceOutputTypeDef](./type_defs.md#deleteresourceoutputtypedef)
- [GetResourceInputRequestTypeDef](./type_defs.md#getresourceinputrequesttypedef)
- [GetResourceOutputTypeDef](./type_defs.md#getresourceoutputtypedef)
- [GetResourceRequestStatusInputRequestTypeDef](./type_defs.md#getresourcerequeststatusinputrequesttypedef)
- [GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef](./type_defs.md#getresourcerequeststatusinputresourcerequestsuccesswaittypedef)
- [GetResourceRequestStatusOutputTypeDef](./type_defs.md#getresourcerequeststatusoutputtypedef)
- [ListResourceRequestsInputRequestTypeDef](./type_defs.md#listresourcerequestsinputrequesttypedef)
- [ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef)
- [ListResourcesInputRequestTypeDef](./type_defs.md#listresourcesinputrequesttypedef)
- [ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef)
- [ProgressEventTypeDef](./type_defs.md#progresseventtypedef)
- [ResourceDescriptionTypeDef](./type_defs.md#resourcedescriptiontypedef)
- [ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UpdateResourceInputRequestTypeDef](./type_defs.md#updateresourceinputrequesttypedef)
- [UpdateResourceOutputTypeDef](./type_defs.md#updateresourceoutputtypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


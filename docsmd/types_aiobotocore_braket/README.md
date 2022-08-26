# Braket module

> [Index](../README.md) > Braket


!!! note ""

    Auto-generated documentation for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
    type annotations stubs module [types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Braket` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[braket]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[braket]'


# standalone installation
python -m pip install types-aiobotocore-braket
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-braket
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BraketClient

Type annotations and code completion for  `#!python session.create_client("braket")` as [BraketClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_braket.client import BraketClient


session = get_session()
async with session.create_client("braket") as client:
    client: BraketClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("braket").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_braket.paginator import SearchDevicesPaginator

def get_search_devices_paginator() -> SearchDevicesPaginator:
    return client.get_paginator("search_devices"))
```

- [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
- [SearchJobsPaginator](./paginators.md#searchjobspaginator)
- [SearchQuantumTasksPaginator](./paginators.md#searchquantumtaskspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_braket.literals import CancellationStatusType

def get_value() -> CancellationStatusType:
    return "CANCELLED"
```

- [CancellationStatusType](./literals.md#cancellationstatustype)
- [CompressionTypeType](./literals.md#compressiontypetype)
- [DeviceStatusType](./literals.md#devicestatustype)
- [DeviceTypeType](./literals.md#devicetypetype)
- [InstanceTypeType](./literals.md#instancetypetype)
- [JobEventTypeType](./literals.md#jobeventtypetype)
- [JobPrimaryStatusType](./literals.md#jobprimarystatustype)
- [QuantumTaskStatusType](./literals.md#quantumtaskstatustype)
- [SearchDevicesPaginatorName](./literals.md#searchdevicespaginatorname)
- [SearchJobsFilterOperatorType](./literals.md#searchjobsfilteroperatortype)
- [SearchJobsPaginatorName](./literals.md#searchjobspaginatorname)
- [SearchQuantumTasksFilterOperatorType](./literals.md#searchquantumtasksfilteroperatortype)
- [SearchQuantumTasksPaginatorName](./literals.md#searchquantumtaskspaginatorname)
- [BraketServiceName](./literals.md#braketservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_braket.type_defs import ContainerImageTypeDef

def get_value() -> ContainerImageTypeDef:
    return {
        "uri": ...,
    }
```

- [ContainerImageTypeDef](./type_defs.md#containerimagetypedef)
- [ScriptModeConfigTypeDef](./type_defs.md#scriptmodeconfigtypedef)
- [CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelQuantumTaskRequestRequestTypeDef](./type_defs.md#cancelquantumtaskrequestrequesttypedef)
- [DeviceConfigTypeDef](./type_defs.md#deviceconfigtypedef)
- [InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef)
- [JobCheckpointConfigTypeDef](./type_defs.md#jobcheckpointconfigtypedef)
- [JobOutputDataConfigTypeDef](./type_defs.md#joboutputdataconfigtypedef)
- [JobStoppingConditionTypeDef](./type_defs.md#jobstoppingconditiontypedef)
- [CreateQuantumTaskRequestRequestTypeDef](./type_defs.md#createquantumtaskrequestrequesttypedef)
- [S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef)
- [DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef)
- [GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef)
- [GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef)
- [JobEventDetailsTypeDef](./type_defs.md#jobeventdetailstypedef)
- [GetQuantumTaskRequestRequestTypeDef](./type_defs.md#getquantumtaskrequestrequesttypedef)
- [JobSummaryTypeDef](./type_defs.md#jobsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [QuantumTaskSummaryTypeDef](./type_defs.md#quantumtasksummarytypedef)
- [SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef)
- [SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef)
- [SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef)
- [CancelJobResponseTypeDef](./type_defs.md#canceljobresponsetypedef)
- [CancelQuantumTaskResponseTypeDef](./type_defs.md#cancelquantumtaskresponsetypedef)
- [CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef)
- [CreateQuantumTaskResponseTypeDef](./type_defs.md#createquantumtaskresponsetypedef)
- [GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef)
- [GetQuantumTaskResponseTypeDef](./type_defs.md#getquantumtaskresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef)
- [SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef)
- [SearchQuantumTasksResponseTypeDef](./type_defs.md#searchquantumtasksresponsetypedef)
- [SearchDevicesRequestRequestTypeDef](./type_defs.md#searchdevicesrequestrequesttypedef)
- [SearchDevicesRequestSearchDevicesPaginateTypeDef](./type_defs.md#searchdevicesrequestsearchdevicespaginatetypedef)
- [SearchJobsRequestRequestTypeDef](./type_defs.md#searchjobsrequestrequesttypedef)
- [SearchJobsRequestSearchJobsPaginateTypeDef](./type_defs.md#searchjobsrequestsearchjobspaginatetypedef)
- [SearchQuantumTasksRequestRequestTypeDef](./type_defs.md#searchquantumtasksrequestrequesttypedef)
- [SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef](./type_defs.md#searchquantumtasksrequestsearchquantumtaskspaginatetypedef)
- [InputFileConfigTypeDef](./type_defs.md#inputfileconfigtypedef)
- [CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef)
- [GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef)


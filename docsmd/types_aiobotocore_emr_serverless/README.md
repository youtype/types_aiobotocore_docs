# EMRServerless module

> [Index](../README.md) > EMRServerless


!!! note ""

    Auto-generated documentation for [EMRServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
    type annotations stubs module [types-aiobotocore-emr-serverless](https://pypi.org/project/types-aiobotocore-emr-serverless/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `EMRServerless` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[emr-serverless]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[emr-serverless]'


# standalone installation
python -m pip install types-aiobotocore-emr-serverless
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-emr-serverless
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EMRServerlessClient

Type annotations and code completion for  `#!python session.create_client("emr-serverless")` as [EMRServerlessClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_emr_serverless.client import EMRServerlessClient


session = get_session()
async with session.create_client("emr-serverless") as client:
    client: EMRServerlessClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("emr-serverless").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_emr_serverless.paginator import ListApplicationsPaginator

def get_list_applications_paginator() -> ListApplicationsPaginator:
    return client.get_paginator("list_applications"))
```

- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_emr_serverless.literals import ApplicationStateType

def get_value() -> ApplicationStateType:
    return "CREATED"
```

- [ApplicationStateType](./literals.md#applicationstatetype)
- [JobRunStateType](./literals.md#jobrunstatetype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListJobRunsPaginatorName](./literals.md#listjobrunspaginatorname)
- [EMRServerlessServiceName](./literals.md#emrserverlessservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_emr_serverless.type_defs import ApplicationSummaryTypeDef

def get_value() -> ApplicationSummaryTypeDef:
    return {
        "id": ...,
        "arn": ...,
        "releaseLabel": ...,
        "type": ...,
        "state": ...,
        "createdAt": ...,
        "updatedAt": ...,
    }
```

- [ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef)
- [AutoStartConfigTypeDef](./type_defs.md#autostartconfigtypedef)
- [AutoStopConfigTypeDef](./type_defs.md#autostopconfigtypedef)
- [MaximumAllowedResourcesTypeDef](./type_defs.md#maximumallowedresourcestypedef)
- [NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
- [CancelJobRunRequestRequestTypeDef](./type_defs.md#canceljobrunrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef)
- [GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef)
- [GetJobRunRequestRequestTypeDef](./type_defs.md#getjobrunrequestrequesttypedef)
- [HiveTypeDef](./type_defs.md#hivetypedef)
- [WorkerResourceConfigTypeDef](./type_defs.md#workerresourceconfigtypedef)
- [SparkSubmitTypeDef](./type_defs.md#sparksubmittypedef)
- [JobRunSummaryTypeDef](./type_defs.md#jobrunsummarytypedef)
- [TotalResourceUtilizationTypeDef](./type_defs.md#totalresourceutilizationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef)
- [ListJobRunsRequestRequestTypeDef](./type_defs.md#listjobrunsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ManagedPersistenceMonitoringConfigurationTypeDef](./type_defs.md#managedpersistencemonitoringconfigurationtypedef)
- [S3MonitoringConfigurationTypeDef](./type_defs.md#s3monitoringconfigurationtypedef)
- [StartApplicationRequestRequestTypeDef](./type_defs.md#startapplicationrequestrequesttypedef)
- [StopApplicationRequestRequestTypeDef](./type_defs.md#stopapplicationrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartJobRunResponseTypeDef](./type_defs.md#startjobrunresponsetypedef)
- [InitialCapacityConfigTypeDef](./type_defs.md#initialcapacityconfigtypedef)
- [JobDriverTypeDef](./type_defs.md#jobdrivertypedef)
- [ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef)
- [ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef)
- [ListJobRunsRequestListJobRunsPaginateTypeDef](./type_defs.md#listjobrunsrequestlistjobrunspaginatetypedef)
- [MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef)
- [GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)
- [UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef)
- [JobRunTypeDef](./type_defs.md#jobruntypedef)
- [StartJobRunRequestRequestTypeDef](./type_defs.md#startjobrunrequestrequesttypedef)
- [GetJobRunResponseTypeDef](./type_defs.md#getjobrunresponsetypedef)


# LookoutforVision module

> [Index](../README.md) > LookoutforVision


!!! note ""

    Auto-generated documentation for [LookoutforVision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#lookoutforvision)
    type annotations stubs module [types-aiobotocore-lookoutvision](https://pypi.org/project/types-aiobotocore-lookoutvision/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LookoutforVision` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LookoutforVision` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[lookoutvision]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[lookoutvision]'

# standalone installation
python -m pip install types-aiobotocore-lookoutvision
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lookoutvision
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LookoutforVisionClient

Type annotations and code completion for  `#!python session.create_client("lookoutvision")` as [LookoutforVisionClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# LookoutforVisionClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_lookoutvision.client import LookoutforVisionClient


session = get_session()
async with session.create_client("lookoutvision") as client:
    client: LookoutforVisionClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("lookoutvision").get_paginator("...")`.

```python
# ListDatasetEntriesPaginator usage example

from types_aiobotocore_lookoutvision.paginator import ListDatasetEntriesPaginator

def get_list_dataset_entries_paginator() -> ListDatasetEntriesPaginator:
    return client.get_paginator("list_dataset_entries"))
```

- [ListDatasetEntriesPaginator](./paginators.md#listdatasetentriespaginator)
- [ListModelPackagingJobsPaginator](./paginators.md#listmodelpackagingjobspaginator)
- [ListModelsPaginator](./paginators.md#listmodelspaginator)
- [ListProjectsPaginator](./paginators.md#listprojectspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DatasetStatusType usage example

from types_aiobotocore_lookoutvision.literals import DatasetStatusType

def get_value() -> DatasetStatusType:
    return "CREATE_COMPLETE"
```

- [DatasetStatusType](./literals.md#datasetstatustype)
- [ListDatasetEntriesPaginatorName](./literals.md#listdatasetentriespaginatorname)
- [ListModelPackagingJobsPaginatorName](./literals.md#listmodelpackagingjobspaginatorname)
- [ListModelsPaginatorName](./literals.md#listmodelspaginatorname)
- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [ModelHostingStatusType](./literals.md#modelhostingstatustype)
- [ModelPackagingJobStatusType](./literals.md#modelpackagingjobstatustype)
- [ModelStatusType](./literals.md#modelstatustype)
- [TargetDeviceType](./literals.md#targetdevicetype)
- [TargetPlatformAcceleratorType](./literals.md#targetplatformacceleratortype)
- [TargetPlatformArchType](./literals.md#targetplatformarchtype)
- [TargetPlatformOsType](./literals.md#targetplatformostype)
- [LookoutforVisionServiceName](./literals.md#lookoutforvisionservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [PixelAnomalyTypeDef](./type_defs.md#pixelanomalytypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [DatasetMetadataTypeDef](./type_defs.md#datasetmetadatatypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateProjectRequestTypeDef](./type_defs.md#createprojectrequesttypedef)
- [ProjectMetadataTypeDef](./type_defs.md#projectmetadatatypedef)
- [DatasetImageStatsTypeDef](./type_defs.md#datasetimagestatstypedef)
- [InputS3ObjectTypeDef](./type_defs.md#inputs3objecttypedef)
- [DeleteDatasetRequestTypeDef](./type_defs.md#deletedatasetrequesttypedef)
- [DeleteModelRequestTypeDef](./type_defs.md#deletemodelrequesttypedef)
- [DeleteProjectRequestTypeDef](./type_defs.md#deleteprojectrequesttypedef)
- [DescribeDatasetRequestTypeDef](./type_defs.md#describedatasetrequesttypedef)
- [DescribeModelPackagingJobRequestTypeDef](./type_defs.md#describemodelpackagingjobrequesttypedef)
- [DescribeModelRequestTypeDef](./type_defs.md#describemodelrequesttypedef)
- [DescribeProjectRequestTypeDef](./type_defs.md#describeprojectrequesttypedef)
- [ImageSourceTypeDef](./type_defs.md#imagesourcetypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [TargetPlatformTypeDef](./type_defs.md#targetplatformtypedef)
- [GreengrassOutputDetailsTypeDef](./type_defs.md#greengrassoutputdetailstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListModelPackagingJobsRequestTypeDef](./type_defs.md#listmodelpackagingjobsrequesttypedef)
- [ModelPackagingJobMetadataTypeDef](./type_defs.md#modelpackagingjobmetadatatypedef)
- [ListModelsRequestTypeDef](./type_defs.md#listmodelsrequesttypedef)
- [ListProjectsRequestTypeDef](./type_defs.md#listprojectsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ModelPerformanceTypeDef](./type_defs.md#modelperformancetypedef)
- [OutputS3ObjectTypeDef](./type_defs.md#outputs3objecttypedef)
- [StartModelRequestTypeDef](./type_defs.md#startmodelrequesttypedef)
- [StopModelRequestTypeDef](./type_defs.md#stopmodelrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [AnomalyTypeDef](./type_defs.md#anomalytypedef)
- [DetectAnomaliesRequestTypeDef](./type_defs.md#detectanomaliesrequesttypedef)
- [UpdateDatasetEntriesRequestTypeDef](./type_defs.md#updatedatasetentriesrequesttypedef)
- [ProjectDescriptionTypeDef](./type_defs.md#projectdescriptiontypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [DeleteModelResponseTypeDef](./type_defs.md#deletemodelresponsetypedef)
- [DeleteProjectResponseTypeDef](./type_defs.md#deleteprojectresponsetypedef)
- [ListDatasetEntriesResponseTypeDef](./type_defs.md#listdatasetentriesresponsetypedef)
- [StartModelPackagingJobResponseTypeDef](./type_defs.md#startmodelpackagingjobresponsetypedef)
- [StartModelResponseTypeDef](./type_defs.md#startmodelresponsetypedef)
- [StopModelResponseTypeDef](./type_defs.md#stopmodelresponsetypedef)
- [UpdateDatasetEntriesResponseTypeDef](./type_defs.md#updatedatasetentriesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef)
- [ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)
- [DatasetDescriptionTypeDef](./type_defs.md#datasetdescriptiontypedef)
- [DatasetGroundTruthManifestTypeDef](./type_defs.md#datasetgroundtruthmanifesttypedef)
- [OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
- [GreengrassConfigurationOutputTypeDef](./type_defs.md#greengrassconfigurationoutputtypedef)
- [GreengrassConfigurationTypeDef](./type_defs.md#greengrassconfigurationtypedef)
- [ModelPackagingOutputDetailsTypeDef](./type_defs.md#modelpackagingoutputdetailstypedef)
- [ListModelPackagingJobsRequestPaginateTypeDef](./type_defs.md#listmodelpackagingjobsrequestpaginatetypedef)
- [ListModelsRequestPaginateTypeDef](./type_defs.md#listmodelsrequestpaginatetypedef)
- [ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef)
- [ListDatasetEntriesRequestPaginateTypeDef](./type_defs.md#listdatasetentriesrequestpaginatetypedef)
- [ListDatasetEntriesRequestTypeDef](./type_defs.md#listdatasetentriesrequesttypedef)
- [ListModelPackagingJobsResponseTypeDef](./type_defs.md#listmodelpackagingjobsresponsetypedef)
- [ModelMetadataTypeDef](./type_defs.md#modelmetadatatypedef)
- [DetectAnomalyResultTypeDef](./type_defs.md#detectanomalyresulttypedef)
- [DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef)
- [CreateModelRequestTypeDef](./type_defs.md#createmodelrequesttypedef)
- [ModelDescriptionTypeDef](./type_defs.md#modeldescriptiontypedef)
- [ModelPackagingConfigurationOutputTypeDef](./type_defs.md#modelpackagingconfigurationoutputtypedef)
- [ModelPackagingConfigurationTypeDef](./type_defs.md#modelpackagingconfigurationtypedef)
- [CreateModelResponseTypeDef](./type_defs.md#createmodelresponsetypedef)
- [ListModelsResponseTypeDef](./type_defs.md#listmodelsresponsetypedef)
- [DetectAnomaliesResponseTypeDef](./type_defs.md#detectanomaliesresponsetypedef)
- [CreateDatasetRequestTypeDef](./type_defs.md#createdatasetrequesttypedef)
- [DescribeModelResponseTypeDef](./type_defs.md#describemodelresponsetypedef)
- [ModelPackagingDescriptionTypeDef](./type_defs.md#modelpackagingdescriptiontypedef)
- [ModelPackagingConfigurationUnionTypeDef](./type_defs.md#modelpackagingconfigurationuniontypedef)
- [DescribeModelPackagingJobResponseTypeDef](./type_defs.md#describemodelpackagingjobresponsetypedef)
- [StartModelPackagingJobRequestTypeDef](./type_defs.md#startmodelpackagingjobrequesttypedef)


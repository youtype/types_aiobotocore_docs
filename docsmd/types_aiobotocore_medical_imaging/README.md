# HealthImaging module

> [Index](../README.md) > HealthImaging


!!! note ""

    Auto-generated documentation for [HealthImaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#healthimaging)
    type annotations stubs module [types-aiobotocore-medical-imaging](https://pypi.org/project/types-aiobotocore-medical-imaging/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `HealthImaging` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `HealthImaging` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[medical-imaging]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[medical-imaging]'

# standalone installation
python -m pip install types-aiobotocore-medical-imaging
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-medical-imaging
```

## Usage

Code samples can be found in [Examples](./usage.md).

## HealthImagingClient

Type annotations and code completion for  `#!python session.create_client("medical-imaging")` as [HealthImagingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Client)

```python
# HealthImagingClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_medical_imaging.client import HealthImagingClient


session = get_session()
async with session.create_client("medical-imaging") as client:
    client: HealthImagingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("medical-imaging").get_paginator("...")`.

```python
# ListDICOMImportJobsPaginator usage example

from types_aiobotocore_medical_imaging.paginator import ListDICOMImportJobsPaginator

def get_list_dicom_import_jobs_paginator() -> ListDICOMImportJobsPaginator:
    return client.get_paginator("list_dicom_import_jobs"))
```

- [ListDICOMImportJobsPaginator](./paginators.md#listdicomimportjobspaginator)
- [ListDatastoresPaginator](./paginators.md#listdatastorespaginator)
- [ListImageSetVersionsPaginator](./paginators.md#listimagesetversionspaginator)
- [SearchImageSetsPaginator](./paginators.md#searchimagesetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DatastoreStatusType usage example

from types_aiobotocore_medical_imaging.literals import DatastoreStatusType

def get_value() -> DatastoreStatusType:
    return "ACTIVE"
```

- [DatastoreStatusType](./literals.md#datastorestatustype)
- [ImageSetStateType](./literals.md#imagesetstatetype)
- [ImageSetWorkflowStatusType](./literals.md#imagesetworkflowstatustype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListDICOMImportJobsPaginatorName](./literals.md#listdicomimportjobspaginatorname)
- [ListDatastoresPaginatorName](./literals.md#listdatastorespaginatorname)
- [ListImageSetVersionsPaginatorName](./literals.md#listimagesetversionspaginatorname)
- [OperatorType](./literals.md#operatortype)
- [SearchImageSetsPaginatorName](./literals.md#searchimagesetspaginatorname)
- [SortFieldType](./literals.md#sortfieldtype)
- [SortOrderType](./literals.md#sortordertype)
- [HealthImagingServiceName](./literals.md#healthimagingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CopyDestinationImageSetPropertiesTypeDef](./type_defs.md#copydestinationimagesetpropertiestypedef)
- [CopyDestinationImageSetTypeDef](./type_defs.md#copydestinationimagesettypedef)
- [CopySourceImageSetPropertiesTypeDef](./type_defs.md#copysourceimagesetpropertiestypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [MetadataCopiesTypeDef](./type_defs.md#metadatacopiestypedef)
- [CreateDatastoreRequestRequestTypeDef](./type_defs.md#createdatastorerequestrequesttypedef)
- [DICOMImportJobPropertiesTypeDef](./type_defs.md#dicomimportjobpropertiestypedef)
- [DICOMImportJobSummaryTypeDef](./type_defs.md#dicomimportjobsummarytypedef)
- [DICOMStudyDateAndTimeTypeDef](./type_defs.md#dicomstudydateandtimetypedef)
- [DICOMTagsTypeDef](./type_defs.md#dicomtagstypedef)
- [DatastorePropertiesTypeDef](./type_defs.md#datastorepropertiestypedef)
- [DatastoreSummaryTypeDef](./type_defs.md#datastoresummarytypedef)
- [DeleteDatastoreRequestRequestTypeDef](./type_defs.md#deletedatastorerequestrequesttypedef)
- [DeleteImageSetRequestRequestTypeDef](./type_defs.md#deleteimagesetrequestrequesttypedef)
- [GetDICOMImportJobRequestRequestTypeDef](./type_defs.md#getdicomimportjobrequestrequesttypedef)
- [GetDatastoreRequestRequestTypeDef](./type_defs.md#getdatastorerequestrequesttypedef)
- [ImageFrameInformationTypeDef](./type_defs.md#imageframeinformationtypedef)
- [GetImageSetMetadataRequestRequestTypeDef](./type_defs.md#getimagesetmetadatarequestrequesttypedef)
- [GetImageSetRequestRequestTypeDef](./type_defs.md#getimagesetrequestrequesttypedef)
- [OverridesTypeDef](./type_defs.md#overridestypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDICOMImportJobsRequestRequestTypeDef](./type_defs.md#listdicomimportjobsrequestrequesttypedef)
- [ListDatastoresRequestRequestTypeDef](./type_defs.md#listdatastoresrequestrequesttypedef)
- [ListImageSetVersionsRequestRequestTypeDef](./type_defs.md#listimagesetversionsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [SortTypeDef](./type_defs.md#sorttypedef)
- [StartDICOMImportJobRequestRequestTypeDef](./type_defs.md#startdicomimportjobrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [DICOMUpdatesTypeDef](./type_defs.md#dicomupdatestypedef)
- [CopyImageSetResponseTypeDef](./type_defs.md#copyimagesetresponsetypedef)
- [CreateDatastoreResponseTypeDef](./type_defs.md#createdatastoreresponsetypedef)
- [DeleteDatastoreResponseTypeDef](./type_defs.md#deletedatastoreresponsetypedef)
- [DeleteImageSetResponseTypeDef](./type_defs.md#deleteimagesetresponsetypedef)
- [GetImageFrameResponseTypeDef](./type_defs.md#getimageframeresponsetypedef)
- [GetImageSetMetadataResponseTypeDef](./type_defs.md#getimagesetmetadataresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartDICOMImportJobResponseTypeDef](./type_defs.md#startdicomimportjobresponsetypedef)
- [UpdateImageSetMetadataResponseTypeDef](./type_defs.md#updateimagesetmetadataresponsetypedef)
- [CopySourceImageSetInformationTypeDef](./type_defs.md#copysourceimagesetinformationtypedef)
- [GetDICOMImportJobResponseTypeDef](./type_defs.md#getdicomimportjobresponsetypedef)
- [ListDICOMImportJobsResponseTypeDef](./type_defs.md#listdicomimportjobsresponsetypedef)
- [ImageSetsMetadataSummaryTypeDef](./type_defs.md#imagesetsmetadatasummarytypedef)
- [GetDatastoreResponseTypeDef](./type_defs.md#getdatastoreresponsetypedef)
- [ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef)
- [GetImageFrameRequestRequestTypeDef](./type_defs.md#getimageframerequestrequesttypedef)
- [GetImageSetResponseTypeDef](./type_defs.md#getimagesetresponsetypedef)
- [ImageSetPropertiesTypeDef](./type_defs.md#imagesetpropertiestypedef)
- [ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef](./type_defs.md#listdicomimportjobsrequestlistdicomimportjobspaginatetypedef)
- [ListDatastoresRequestListDatastoresPaginateTypeDef](./type_defs.md#listdatastoresrequestlistdatastorespaginatetypedef)
- [ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef](./type_defs.md#listimagesetversionsrequestlistimagesetversionspaginatetypedef)
- [SearchByAttributeValueTypeDef](./type_defs.md#searchbyattributevaluetypedef)
- [MetadataUpdatesTypeDef](./type_defs.md#metadataupdatestypedef)
- [CopyImageSetInformationTypeDef](./type_defs.md#copyimagesetinformationtypedef)
- [SearchImageSetsResponseTypeDef](./type_defs.md#searchimagesetsresponsetypedef)
- [ListImageSetVersionsResponseTypeDef](./type_defs.md#listimagesetversionsresponsetypedef)
- [SearchFilterTypeDef](./type_defs.md#searchfiltertypedef)
- [UpdateImageSetMetadataRequestRequestTypeDef](./type_defs.md#updateimagesetmetadatarequestrequesttypedef)
- [CopyImageSetRequestRequestTypeDef](./type_defs.md#copyimagesetrequestrequesttypedef)
- [SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef)
- [SearchImageSetsRequestRequestTypeDef](./type_defs.md#searchimagesetsrequestrequesttypedef)
- [SearchImageSetsRequestSearchImageSetsPaginateTypeDef](./type_defs.md#searchimagesetsrequestsearchimagesetspaginatetypedef)


# ApplicationCostProfiler module

> [Index](../README.md) > ApplicationCostProfiler


!!! note ""

    Auto-generated documentation for [ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#applicationcostprofiler)
    type annotations stubs module [types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ApplicationCostProfiler` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ApplicationCostProfiler` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[applicationcostprofiler]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[applicationcostprofiler]'

# standalone installation
python -m pip install types-aiobotocore-applicationcostprofiler
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-applicationcostprofiler
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ApplicationCostProfilerClient

Type annotations and code completion for  `#!python session.create_client("applicationcostprofiler")` as [ApplicationCostProfilerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# ApplicationCostProfilerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_applicationcostprofiler.client import ApplicationCostProfilerClient


session = get_session()
async with session.create_client("applicationcostprofiler") as client:
    client: ApplicationCostProfilerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("applicationcostprofiler").get_paginator("...")`.

```python
# ListReportDefinitionsPaginator usage example

from types_aiobotocore_applicationcostprofiler.paginator import ListReportDefinitionsPaginator

def get_list_report_definitions_paginator() -> ListReportDefinitionsPaginator:
    return client.get_paginator("list_report_definitions"))
```

- [ListReportDefinitionsPaginator](./paginators.md#listreportdefinitionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# FormatType usage example

from types_aiobotocore_applicationcostprofiler.literals import FormatType

def get_value() -> FormatType:
    return "CSV"
```

- [FormatType](./literals.md#formattype)
- [ListReportDefinitionsPaginatorName](./literals.md#listreportdefinitionspaginatorname)
- [ReportFrequencyType](./literals.md#reportfrequencytype)
- [S3BucketRegionType](./literals.md#s3bucketregiontype)
- [ApplicationCostProfilerServiceName](./literals.md#applicationcostprofilerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeleteReportDefinitionRequestTypeDef](./type_defs.md#deletereportdefinitionrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetReportDefinitionRequestTypeDef](./type_defs.md#getreportdefinitionrequesttypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListReportDefinitionsRequestTypeDef](./type_defs.md#listreportdefinitionsrequesttypedef)
- [DeleteReportDefinitionResultTypeDef](./type_defs.md#deletereportdefinitionresulttypedef)
- [ImportApplicationUsageResultTypeDef](./type_defs.md#importapplicationusageresulttypedef)
- [PutReportDefinitionResultTypeDef](./type_defs.md#putreportdefinitionresulttypedef)
- [UpdateReportDefinitionResultTypeDef](./type_defs.md#updatereportdefinitionresulttypedef)
- [GetReportDefinitionResultTypeDef](./type_defs.md#getreportdefinitionresulttypedef)
- [PutReportDefinitionRequestTypeDef](./type_defs.md#putreportdefinitionrequesttypedef)
- [ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef)
- [UpdateReportDefinitionRequestTypeDef](./type_defs.md#updatereportdefinitionrequesttypedef)
- [ImportApplicationUsageRequestTypeDef](./type_defs.md#importapplicationusagerequesttypedef)
- [ListReportDefinitionsRequestPaginateTypeDef](./type_defs.md#listreportdefinitionsrequestpaginatetypedef)
- [ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef)


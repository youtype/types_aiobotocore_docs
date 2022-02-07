<a id="type-annotations-for-aiobotocore-applicationcostprofiler-module"></a>

# Type annotations for aiobotocore ApplicationCostProfiler module

> [Index](..) > ApplicationCostProfiler

Auto-generated documentation for
[ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
type annotations stubs module
[types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[applicationcostprofiler]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[applicationcostprofiler]'

# standalone installation
pip install types-aiobotocore-applicationcostprofiler
```

- [Type annotations for aiobotocore ApplicationCostProfiler module](#type-annotations-for-aiobotocore-applicationcostprofiler-module)
  - [ApplicationCostProfilerClient](#applicationcostprofilerclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="applicationcostprofilerclient"></a>

## ApplicationCostProfilerClient

Type annotations for `session.create_client("applicationcostprofiler")` as
[ApplicationCostProfilerClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_applicationcostprofiler.client import ApplicationCostProfilerClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [delete_report_definition](./client.md#delete_report_definition)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_paginator](./client.md#get_paginator)
- [get_report_definition](./client.md#get_report_definition)
- [import_application_usage](./client.md#import_application_usage)
- [list_report_definitions](./client.md#list_report_definitions)
- [put_report_definition](./client.md#put_report_definition)
- [update_report_definition](./client.md#update_report_definition)

<a id="exceptions"></a>

### Exceptions

ApplicationCostProfilerClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- InternalServerException
- ServiceQuotaExceededException
- ThrottlingException
- ValidationException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("applicationcostprofiler").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_applicationcostprofiler.paginator import ListReportDefinitionsPaginator, ...
```

- [ListReportDefinitionsPaginator](./paginators.md#listreportdefinitionspaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_applicationcostprofiler.literals import FormatType, ...
```

- [FormatType](./literals.md#formattype)
- [ListReportDefinitionsPaginatorName](./literals.md#listreportdefinitionspaginatorname)
- [ReportFrequencyType](./literals.md#reportfrequencytype)
- [S3BucketRegionType](./literals.md#s3bucketregiontype)
- [ServiceName](./literals.md#servicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_applicationcostprofiler.type_defs import DeleteReportDefinitionRequestRequestTypeDef, ...
```

- [DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef)
- [DeleteReportDefinitionResultTypeDef](./type_defs.md#deletereportdefinitionresulttypedef)
- [GetReportDefinitionRequestRequestTypeDef](./type_defs.md#getreportdefinitionrequestrequesttypedef)
- [GetReportDefinitionResultTypeDef](./type_defs.md#getreportdefinitionresulttypedef)
- [ImportApplicationUsageRequestRequestTypeDef](./type_defs.md#importapplicationusagerequestrequesttypedef)
- [ImportApplicationUsageResultTypeDef](./type_defs.md#importapplicationusageresulttypedef)
- [ListReportDefinitionsRequestRequestTypeDef](./type_defs.md#listreportdefinitionsrequestrequesttypedef)
- [ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef)
- [PutReportDefinitionResultTypeDef](./type_defs.md#putreportdefinitionresulttypedef)
- [ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef)
- [UpdateReportDefinitionRequestRequestTypeDef](./type_defs.md#updatereportdefinitionrequestrequesttypedef)
- [UpdateReportDefinitionResultTypeDef](./type_defs.md#updatereportdefinitionresulttypedef)

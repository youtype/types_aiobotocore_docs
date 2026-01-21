# ImportExport module

> [Index](../README.md) > ImportExport


!!! note ""

    Auto-generated documentation for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#importexport)
    type annotations stubs module [types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ImportExport` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ImportExport` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[importexport]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[importexport]'

# standalone installation
python -m pip install types-aiobotocore-importexport
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-importexport
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ImportExportClient

Type annotations and code completion for  `#!python session.create_client("importexport")` as [ImportExportClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# ImportExportClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_importexport.client import ImportExportClient


session = get_session()
async with session.create_client("importexport") as client:
    client: ImportExportClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("importexport").get_paginator("...")`.

```python
# ListJobsPaginator usage example

from types_aiobotocore_importexport.paginator import ListJobsPaginator

def get_list_jobs_paginator() -> ListJobsPaginator:
    return client.get_paginator("list_jobs"))
```

- [ListJobsPaginator](./paginators.md#listjobspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# JobTypeType usage example

from types_aiobotocore_importexport.literals import JobTypeType

def get_value() -> JobTypeType:
    return "Export"
```

- [JobTypeType](./literals.md#jobtypetype)
- [ListJobsPaginatorName](./literals.md#listjobspaginatorname)
- [ImportExportServiceName](./literals.md#importexportservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ArtifactTypeDef](./type_defs.md#artifacttypedef)
- [CancelJobInputTypeDef](./type_defs.md#canceljobinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateJobInputTypeDef](./type_defs.md#createjobinputtypedef)
- [GetShippingLabelInputTypeDef](./type_defs.md#getshippinglabelinputtypedef)
- [GetStatusInputTypeDef](./type_defs.md#getstatusinputtypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListJobsInputTypeDef](./type_defs.md#listjobsinputtypedef)
- [UpdateJobInputTypeDef](./type_defs.md#updatejobinputtypedef)
- [CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef)
- [CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef)
- [GetShippingLabelOutputTypeDef](./type_defs.md#getshippinglabeloutputtypedef)
- [GetStatusOutputTypeDef](./type_defs.md#getstatusoutputtypedef)
- [UpdateJobOutputTypeDef](./type_defs.md#updatejoboutputtypedef)
- [ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef)
- [ListJobsInputPaginateTypeDef](./type_defs.md#listjobsinputpaginatetypedef)


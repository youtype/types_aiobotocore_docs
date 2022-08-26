# ImportExport module

> [Index](../README.md) > ImportExport


!!! note ""

    Auto-generated documentation for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
    type annotations stubs module [types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

## How to install



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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_importexport.paginator import ListJobsPaginator

def get_list_jobs_paginator() -> ListJobsPaginator:
    return client.get_paginator("list_jobs"))
```

- [ListJobsPaginator](./paginators.md#listjobspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
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




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_importexport.type_defs import ArtifactTypeDef

def get_value() -> ArtifactTypeDef:
    return {
        "Description": ...,
    }
```

- [ArtifactTypeDef](./type_defs.md#artifacttypedef)
- [CancelJobInputRequestTypeDef](./type_defs.md#canceljobinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateJobInputRequestTypeDef](./type_defs.md#createjobinputrequesttypedef)
- [GetShippingLabelInputRequestTypeDef](./type_defs.md#getshippinglabelinputrequesttypedef)
- [GetStatusInputRequestTypeDef](./type_defs.md#getstatusinputrequesttypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListJobsInputRequestTypeDef](./type_defs.md#listjobsinputrequesttypedef)
- [UpdateJobInputRequestTypeDef](./type_defs.md#updatejobinputrequesttypedef)
- [CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef)
- [CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef)
- [GetShippingLabelOutputTypeDef](./type_defs.md#getshippinglabeloutputtypedef)
- [GetStatusOutputTypeDef](./type_defs.md#getstatusoutputtypedef)
- [UpdateJobOutputTypeDef](./type_defs.md#updatejoboutputtypedef)
- [ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef)
- [ListJobsInputListJobsPaginateTypeDef](./type_defs.md#listjobsinputlistjobspaginatetypedef)


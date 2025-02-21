# Examples

> [Index](../README.md) > [HealthImaging](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [HealthImaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#healthimaging)
    type annotations stubs module [types-aiobotocore-medical-imaging](https://pypi.org/project/types-aiobotocore-medical-imaging/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[medical-imaging]` package installed.

Write your `HealthImaging` code as usual,
type checking and code completion should work out of the box.



```python
# HealthImagingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("medical-imaging") as client:  # (1)
    result = await client.copy_image_set()  # (2)
```

1. client: [HealthImagingClient](./client.md)
2. result: [:material-code-braces: CopyImageSetResponseTypeDef](./type_defs.md#copyimagesetresponsetypedef) 



```python
# ListDICOMImportJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("medical-imaging") as client:  # (1)
    paginator = client.get_paginator("list_dicom_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. paginator: [ListDICOMImportJobsPaginator](./paginators.md#listdicomimportjobspaginator)
3. item: [:material-code-braces: ListDICOMImportJobsResponseTypeDef](./type_defs.md#listdicomimportjobsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[medical-imaging]`
or a standalone `types_aiobotocore_medical_imaging` package, you have to explicitly specify
`client: HealthImagingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# HealthImagingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_medical_imaging.client import HealthImagingClient
from types_aiobotocore_medical_imaging.type_defs import CopyImageSetResponseTypeDef
from types_aiobotocore_medical_imaging.type_defs import CopyImageSetRequestTypeDef


session = get_session()

async with session.create_client("medical-imaging") as client:
    client: HealthImagingClient
    kwargs: CopyImageSetRequestTypeDef = {...}
    result: CopyImageSetResponseTypeDef = await client.copy_image_set(**kwargs)
```



```python
# ListDICOMImportJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_medical_imaging.client import HealthImagingClient
from types_aiobotocore_medical_imaging.paginator import ListDICOMImportJobsPaginator
from types_aiobotocore_medical_imaging.type_defs import ListDICOMImportJobsResponseTypeDef


session = get_session()

async with session.create_client("medical-imaging") as client:
    client: HealthImagingClient
    paginator: ListDICOMImportJobsPaginator = client.get_paginator("list_dicom_import_jobs")
    async for item in paginator.paginate(...):
        item: ListDICOMImportJobsResponseTypeDef
        print(item)
```



# Honeycode module

> [Index](../README.md) > Honeycode


!!! note ""

    Auto-generated documentation for [Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
    type annotations stubs module [types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Honeycode` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[honeycode]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[honeycode]'


# standalone installation
python -m pip install types-aiobotocore-honeycode
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-honeycode
```

## Usage

Code samples can be found in [Examples](./usage.md).

## HoneycodeClient

Type annotations and code completion for  `#!python session.create_client("honeycode")` as [HoneycodeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_honeycode.client import HoneycodeClient


session = get_session()
async with session.create_client("honeycode") as client:
    client: HoneycodeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("honeycode").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_honeycode.paginator import ListTableColumnsPaginator

def get_list_table_columns_paginator() -> ListTableColumnsPaginator:
    return client.get_paginator("list_table_columns"))
```

- [ListTableColumnsPaginator](./paginators.md#listtablecolumnspaginator)
- [ListTableRowsPaginator](./paginators.md#listtablerowspaginator)
- [ListTablesPaginator](./paginators.md#listtablespaginator)
- [QueryTableRowsPaginator](./paginators.md#querytablerowspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_honeycode.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "ACCESS_DENIED"
```

- [ErrorCodeType](./literals.md#errorcodetype)
- [FormatType](./literals.md#formattype)
- [ImportDataCharacterEncodingType](./literals.md#importdatacharacterencodingtype)
- [ImportSourceDataFormatType](./literals.md#importsourcedataformattype)
- [ListTableColumnsPaginatorName](./literals.md#listtablecolumnspaginatorname)
- [ListTableRowsPaginatorName](./literals.md#listtablerowspaginatorname)
- [ListTablesPaginatorName](./literals.md#listtablespaginatorname)
- [QueryTableRowsPaginatorName](./literals.md#querytablerowspaginatorname)
- [TableDataImportJobStatusType](./literals.md#tabledataimportjobstatustype)
- [UpsertActionType](./literals.md#upsertactiontype)
- [HoneycodeServiceName](./literals.md#honeycodeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_honeycode.type_defs import FailedBatchItemTypeDef

def get_value() -> FailedBatchItemTypeDef:
    return {
        "id": ...,
        "errorMessage": ...,
    }
```

- [FailedBatchItemTypeDef](./type_defs.md#failedbatchitemtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDeleteTableRowsRequestRequestTypeDef](./type_defs.md#batchdeletetablerowsrequestrequesttypedef)
- [UpsertRowsResultTypeDef](./type_defs.md#upsertrowsresulttypedef)
- [CellInputTypeDef](./type_defs.md#cellinputtypedef)
- [CellTypeDef](./type_defs.md#celltypedef)
- [ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef)
- [DataItemTypeDef](./type_defs.md#dataitemtypedef)
- [DelimitedTextImportOptionsTypeDef](./type_defs.md#delimitedtextimportoptionstypedef)
- [DescribeTableDataImportJobRequestRequestTypeDef](./type_defs.md#describetabledataimportjobrequestrequesttypedef)
- [SourceDataColumnPropertiesTypeDef](./type_defs.md#sourcedatacolumnpropertiestypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [VariableValueTypeDef](./type_defs.md#variablevaluetypedef)
- [ImportDataSourceConfigTypeDef](./type_defs.md#importdatasourceconfigtypedef)
- [ImportJobSubmitterTypeDef](./type_defs.md#importjobsubmittertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTableColumnsRequestRequestTypeDef](./type_defs.md#listtablecolumnsrequestrequesttypedef)
- [TableColumnTypeDef](./type_defs.md#tablecolumntypedef)
- [ListTableRowsRequestRequestTypeDef](./type_defs.md#listtablerowsrequestrequesttypedef)
- [ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef)
- [TableTypeDef](./type_defs.md#tabletypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [BatchCreateTableRowsResultTypeDef](./type_defs.md#batchcreatetablerowsresulttypedef)
- [BatchDeleteTableRowsResultTypeDef](./type_defs.md#batchdeletetablerowsresulttypedef)
- [BatchUpdateTableRowsResultTypeDef](./type_defs.md#batchupdatetablerowsresulttypedef)
- [InvokeScreenAutomationResultTypeDef](./type_defs.md#invokescreenautomationresulttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [StartTableDataImportJobResultTypeDef](./type_defs.md#starttabledataimportjobresulttypedef)
- [BatchUpsertTableRowsResultTypeDef](./type_defs.md#batchupserttablerowsresulttypedef)
- [CreateRowDataTypeDef](./type_defs.md#createrowdatatypedef)
- [UpdateRowDataTypeDef](./type_defs.md#updaterowdatatypedef)
- [TableRowTypeDef](./type_defs.md#tablerowtypedef)
- [ResultRowTypeDef](./type_defs.md#resultrowtypedef)
- [DestinationOptionsTypeDef](./type_defs.md#destinationoptionstypedef)
- [QueryTableRowsRequestRequestTypeDef](./type_defs.md#querytablerowsrequestrequesttypedef)
- [UpsertRowDataTypeDef](./type_defs.md#upsertrowdatatypedef)
- [GetScreenDataRequestRequestTypeDef](./type_defs.md#getscreendatarequestrequesttypedef)
- [InvokeScreenAutomationRequestRequestTypeDef](./type_defs.md#invokescreenautomationrequestrequesttypedef)
- [ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef)
- [ListTableColumnsRequestListTableColumnsPaginateTypeDef](./type_defs.md#listtablecolumnsrequestlisttablecolumnspaginatetypedef)
- [ListTableRowsRequestListTableRowsPaginateTypeDef](./type_defs.md#listtablerowsrequestlisttablerowspaginatetypedef)
- [ListTablesRequestListTablesPaginateTypeDef](./type_defs.md#listtablesrequestlisttablespaginatetypedef)
- [QueryTableRowsRequestQueryTableRowsPaginateTypeDef](./type_defs.md#querytablerowsrequestquerytablerowspaginatetypedef)
- [ListTableColumnsResultTypeDef](./type_defs.md#listtablecolumnsresulttypedef)
- [ListTablesResultTypeDef](./type_defs.md#listtablesresulttypedef)
- [BatchCreateTableRowsRequestRequestTypeDef](./type_defs.md#batchcreatetablerowsrequestrequesttypedef)
- [BatchUpdateTableRowsRequestRequestTypeDef](./type_defs.md#batchupdatetablerowsrequestrequesttypedef)
- [ListTableRowsResultTypeDef](./type_defs.md#listtablerowsresulttypedef)
- [QueryTableRowsResultTypeDef](./type_defs.md#querytablerowsresulttypedef)
- [ResultSetTypeDef](./type_defs.md#resultsettypedef)
- [ImportOptionsTypeDef](./type_defs.md#importoptionstypedef)
- [BatchUpsertTableRowsRequestRequestTypeDef](./type_defs.md#batchupserttablerowsrequestrequesttypedef)
- [GetScreenDataResultTypeDef](./type_defs.md#getscreendataresulttypedef)
- [StartTableDataImportJobRequestRequestTypeDef](./type_defs.md#starttabledataimportjobrequestrequesttypedef)
- [TableDataImportJobMetadataTypeDef](./type_defs.md#tabledataimportjobmetadatatypedef)
- [DescribeTableDataImportJobResultTypeDef](./type_defs.md#describetabledataimportjobresulttypedef)


# CloudSearchDomain module

> [Index](../README.md) > CloudSearchDomain


!!! note ""

    Auto-generated documentation for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
    type annotations stubs module [types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `CloudSearchDomain`.

### From PyPI with pip

Install `types-aiobotocore` for `CloudSearchDomain` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudsearchdomain]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudsearchdomain]'


# standalone installation
python -m pip install types-aiobotocore-cloudsearchdomain
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudsearchdomain
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudSearchDomainClient

Type annotations and code completion for  `#!python session.create_client("cloudsearchdomain")` as [CloudSearchDomainClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient


session = get_session()
async with session.create_client("cloudsearchdomain") as client:
    client: CloudSearchDomainClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_cloudsearchdomain.literals import ContentTypeType

def get_value() -> ContentTypeType:
    return "application/json"
```

- [ContentTypeType](./literals.md#contenttypetype)
- [QueryParserType](./literals.md#queryparsertype)
- [CloudSearchDomainServiceName](./literals.md#cloudsearchdomainservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_cloudsearchdomain.type_defs import BucketInfoTypeDef

def get_value() -> BucketInfoTypeDef:
    return {
        "buckets": ...,
    }
```

- [BucketInfoTypeDef](./type_defs.md#bucketinfotypedef)
- [BucketTypeDef](./type_defs.md#buckettypedef)
- [DocumentServiceWarningTypeDef](./type_defs.md#documentservicewarningtypedef)
- [FieldStatsTypeDef](./type_defs.md#fieldstatstypedef)
- [HitTypeDef](./type_defs.md#hittypedef)
- [HitsTypeDef](./type_defs.md#hitstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SearchRequestRequestTypeDef](./type_defs.md#searchrequestrequesttypedef)
- [SearchResponseTypeDef](./type_defs.md#searchresponsetypedef)
- [SearchStatusTypeDef](./type_defs.md#searchstatustypedef)
- [SuggestModelTypeDef](./type_defs.md#suggestmodeltypedef)
- [SuggestRequestRequestTypeDef](./type_defs.md#suggestrequestrequesttypedef)
- [SuggestResponseTypeDef](./type_defs.md#suggestresponsetypedef)
- [SuggestStatusTypeDef](./type_defs.md#suggeststatustypedef)
- [SuggestionMatchTypeDef](./type_defs.md#suggestionmatchtypedef)
- [UploadDocumentsRequestRequestTypeDef](./type_defs.md#uploaddocumentsrequestrequesttypedef)
- [UploadDocumentsResponseTypeDef](./type_defs.md#uploaddocumentsresponsetypedef)


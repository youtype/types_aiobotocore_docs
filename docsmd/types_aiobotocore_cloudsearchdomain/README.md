# CloudSearchDomain module

> [Index](../README.md) > CloudSearchDomain


!!! note ""

    Auto-generated documentation for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#cloudsearchdomain)
    type annotations stubs module [types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudSearchDomain` service.
1. Use provided commands to install generated packages.



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

```python
# CloudSearchDomainClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient


session = get_session()
async with session.create_client("cloudsearchdomain") as client:
    client: CloudSearchDomainClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ContentTypeType usage example

from types_aiobotocore_cloudsearchdomain.literals import ContentTypeType

def get_value() -> ContentTypeType:
    return "application/json"
```

- [ContentTypeType](./literals.md#contenttypetype)
- [QueryParserType](./literals.md#queryparsertype)
- [CloudSearchDomainServiceName](./literals.md#cloudsearchdomainservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BucketTypeDef](./type_defs.md#buckettypedef)
- [DocumentServiceWarningTypeDef](./type_defs.md#documentservicewarningtypedef)
- [FieldStatsTypeDef](./type_defs.md#fieldstatstypedef)
- [HitTypeDef](./type_defs.md#hittypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SearchRequestTypeDef](./type_defs.md#searchrequesttypedef)
- [SearchStatusTypeDef](./type_defs.md#searchstatustypedef)
- [SuggestionMatchTypeDef](./type_defs.md#suggestionmatchtypedef)
- [SuggestRequestTypeDef](./type_defs.md#suggestrequesttypedef)
- [SuggestStatusTypeDef](./type_defs.md#suggeststatustypedef)
- [UploadDocumentsRequestTypeDef](./type_defs.md#uploaddocumentsrequesttypedef)
- [BucketInfoTypeDef](./type_defs.md#bucketinfotypedef)
- [HitsTypeDef](./type_defs.md#hitstypedef)
- [UploadDocumentsResponseTypeDef](./type_defs.md#uploaddocumentsresponsetypedef)
- [SuggestModelTypeDef](./type_defs.md#suggestmodeltypedef)
- [SearchResponseTypeDef](./type_defs.md#searchresponsetypedef)
- [SuggestResponseTypeDef](./type_defs.md#suggestresponsetypedef)


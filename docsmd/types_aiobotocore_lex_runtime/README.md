# LexRuntimeService module

> [Index](../README.md) > LexRuntimeService


!!! note ""

    Auto-generated documentation for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#lexruntimeservice)
    type annotations stubs module [types-aiobotocore-lex-runtime](https://pypi.org/project/types-aiobotocore-lex-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LexRuntimeService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LexRuntimeService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[lex-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[lex-runtime]'

# standalone installation
python -m pip install types-aiobotocore-lex-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lex-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LexRuntimeServiceClient

Type annotations and code completion for  `#!python session.create_client("lex-runtime")` as [LexRuntimeServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# LexRuntimeServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient


session = get_session()
async with session.create_client("lex-runtime") as client:
    client: LexRuntimeServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConfirmationStatusType usage example

from types_aiobotocore_lex_runtime.literals import ConfirmationStatusType

def get_value() -> ConfirmationStatusType:
    return "Confirmed"
```

- [ConfirmationStatusType](./literals.md#confirmationstatustype)
- [ContentTypeType](./literals.md#contenttypetype)
- [DialogActionTypeType](./literals.md#dialogactiontypetype)
- [DialogStateType](./literals.md#dialogstatetype)
- [FulfillmentStateType](./literals.md#fulfillmentstatetype)
- [MessageFormatTypeType](./literals.md#messageformattypetype)
- [LexRuntimeServiceServiceName](./literals.md#lexruntimeserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ButtonTypeDef](./type_defs.md#buttontypedef)
- [DeleteSessionRequestTypeDef](./type_defs.md#deletesessionrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DialogActionOutputTypeDef](./type_defs.md#dialogactionoutputtypedef)
- [DialogActionTypeDef](./type_defs.md#dialogactiontypedef)
- [GetSessionRequestTypeDef](./type_defs.md#getsessionrequesttypedef)
- [IntentSummaryOutputTypeDef](./type_defs.md#intentsummaryoutputtypedef)
- [IntentConfidenceTypeDef](./type_defs.md#intentconfidencetypedef)
- [IntentSummaryTypeDef](./type_defs.md#intentsummarytypedef)
- [SentimentResponseTypeDef](./type_defs.md#sentimentresponsetypedef)
- [ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef)
- [ActiveContextTypeDef](./type_defs.md#activecontexttypedef)
- [PostContentRequestTypeDef](./type_defs.md#postcontentrequesttypedef)
- [GenericAttachmentTypeDef](./type_defs.md#genericattachmenttypedef)
- [DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef)
- [PostContentResponseTypeDef](./type_defs.md#postcontentresponsetypedef)
- [PutSessionResponseTypeDef](./type_defs.md#putsessionresponsetypedef)
- [DialogActionUnionTypeDef](./type_defs.md#dialogactionuniontypedef)
- [PredictedIntentTypeDef](./type_defs.md#predictedintenttypedef)
- [IntentSummaryUnionTypeDef](./type_defs.md#intentsummaryuniontypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [ActiveContextUnionTypeDef](./type_defs.md#activecontextuniontypedef)
- [ResponseCardTypeDef](./type_defs.md#responsecardtypedef)
- [PostTextRequestTypeDef](./type_defs.md#posttextrequesttypedef)
- [PutSessionRequestTypeDef](./type_defs.md#putsessionrequesttypedef)
- [PostTextResponseTypeDef](./type_defs.md#posttextresponsetypedef)


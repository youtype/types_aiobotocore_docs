# Polly module

> [Index](../README.md) > Polly


!!! note ""

    Auto-generated documentation for [Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#polly)
    type annotations stubs module [types-aiobotocore-polly](https://pypi.org/project/types-aiobotocore-polly/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Polly` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Polly` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[polly]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[polly]'

# standalone installation
python -m pip install types-aiobotocore-polly
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-polly
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PollyClient

Type annotations and code completion for  `#!python session.create_client("polly")` as [PollyClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# PollyClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_polly.client import PollyClient


session = get_session()
async with session.create_client("polly") as client:
    client: PollyClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("polly").get_paginator("...")`.

```python
# DescribeVoicesPaginator usage example

from types_aiobotocore_polly.paginator import DescribeVoicesPaginator

def get_describe_voices_paginator() -> DescribeVoicesPaginator:
    return client.get_paginator("describe_voices"))
```

- [DescribeVoicesPaginator](./paginators.md#describevoicespaginator)
- [ListLexiconsPaginator](./paginators.md#listlexiconspaginator)
- [ListSpeechSynthesisTasksPaginator](./paginators.md#listspeechsynthesistaskspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DescribeVoicesPaginatorName usage example

from types_aiobotocore_polly.literals import DescribeVoicesPaginatorName

def get_value() -> DescribeVoicesPaginatorName:
    return "describe_voices"
```

- [DescribeVoicesPaginatorName](./literals.md#describevoicespaginatorname)
- [EngineType](./literals.md#enginetype)
- [GenderType](./literals.md#gendertype)
- [LanguageCodeType](./literals.md#languagecodetype)
- [ListLexiconsPaginatorName](./literals.md#listlexiconspaginatorname)
- [ListSpeechSynthesisTasksPaginatorName](./literals.md#listspeechsynthesistaskspaginatorname)
- [OutputFormatType](./literals.md#outputformattype)
- [SpeechMarkTypeType](./literals.md#speechmarktypetype)
- [TaskStatusType](./literals.md#taskstatustype)
- [TextTypeType](./literals.md#texttypetype)
- [VoiceIdType](./literals.md#voiceidtype)
- [PollyServiceName](./literals.md#pollyservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeleteLexiconInputTypeDef](./type_defs.md#deletelexiconinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeVoicesInputTypeDef](./type_defs.md#describevoicesinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [VoiceTypeDef](./type_defs.md#voicetypedef)
- [GetLexiconInputTypeDef](./type_defs.md#getlexiconinputtypedef)
- [LexiconAttributesTypeDef](./type_defs.md#lexiconattributestypedef)
- [LexiconTypeDef](./type_defs.md#lexicontypedef)
- [GetSpeechSynthesisTaskInputTypeDef](./type_defs.md#getspeechsynthesistaskinputtypedef)
- [SynthesisTaskTypeDef](./type_defs.md#synthesistasktypedef)
- [ListLexiconsInputTypeDef](./type_defs.md#listlexiconsinputtypedef)
- [ListSpeechSynthesisTasksInputTypeDef](./type_defs.md#listspeechsynthesistasksinputtypedef)
- [PutLexiconInputTypeDef](./type_defs.md#putlexiconinputtypedef)
- [StartSpeechSynthesisTaskInputTypeDef](./type_defs.md#startspeechsynthesistaskinputtypedef)
- [SynthesizeSpeechInputTypeDef](./type_defs.md#synthesizespeechinputtypedef)
- [DescribeVoicesInputPaginateTypeDef](./type_defs.md#describevoicesinputpaginatetypedef)
- [ListLexiconsInputPaginateTypeDef](./type_defs.md#listlexiconsinputpaginatetypedef)
- [ListSpeechSynthesisTasksInputPaginateTypeDef](./type_defs.md#listspeechsynthesistasksinputpaginatetypedef)
- [SynthesizeSpeechOutputTypeDef](./type_defs.md#synthesizespeechoutputtypedef)
- [DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef)
- [LexiconDescriptionTypeDef](./type_defs.md#lexicondescriptiontypedef)
- [GetLexiconOutputTypeDef](./type_defs.md#getlexiconoutputtypedef)
- [GetSpeechSynthesisTaskOutputTypeDef](./type_defs.md#getspeechsynthesistaskoutputtypedef)
- [ListSpeechSynthesisTasksOutputTypeDef](./type_defs.md#listspeechsynthesistasksoutputtypedef)
- [StartSpeechSynthesisTaskOutputTypeDef](./type_defs.md#startspeechsynthesistaskoutputtypedef)
- [ListLexiconsOutputTypeDef](./type_defs.md#listlexiconsoutputtypedef)


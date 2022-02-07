<a id="paginators-for-aiobotocore-polly-module"></a>

# Paginators for aiobotocore Polly module

> [Index](..) > [Polly](.) > Paginators

Auto-generated documentation for
[Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
type annotations stubs module
[types-aiobotocore-polly](https://pypi.org/project/types-aiobotocore-polly/).

- [Paginators for aiobotocore Polly module](#paginators-for-aiobotocore-polly-module)
  - [DescribeVoicesPaginator](#describevoicespaginator)
  - [ListLexiconsPaginator](#listlexiconspaginator)
  - [ListSpeechSynthesisTasksPaginator](#listspeechsynthesistaskspaginator)

<a id="describevoicespaginator"></a>

## DescribeVoicesPaginator

Type annotations for
`session.create_client("polly").get_paginator("describe_voices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_polly.paginator import DescribeVoicesPaginator

session = get_session()
async with session.create_client("polly") as client:
    client: PollyClient
    paginator: DescribeVoicesPaginator = client.get_paginator("describe_voices")
```

Boto3 documentation:
[Polly.Paginator.DescribeVoices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices)

Arguments for `DescribeVoicesPaginator.paginate` method:

- `Engine`: [EngineType](./literals.md#enginetype)
- `LanguageCode`: [LanguageCodeType](./literals.md#languagecodetype)
- `IncludeAdditionalLanguageCodes`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeVoicesPaginator.paginate` returns
`_PageIterator`\[[DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef)\].

<a id="listlexiconspaginator"></a>

## ListLexiconsPaginator

Type annotations for
`session.create_client("polly").get_paginator("list_lexicons")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_polly.paginator import ListLexiconsPaginator

session = get_session()
async with session.create_client("polly") as client:
    client: PollyClient
    paginator: ListLexiconsPaginator = client.get_paginator("list_lexicons")
```

Boto3 documentation:
[Polly.Paginator.ListLexicons](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons)

Arguments for `ListLexiconsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLexiconsPaginator.paginate` returns
`_PageIterator`\[[ListLexiconsOutputTypeDef](./type_defs.md#listlexiconsoutputtypedef)\].

<a id="listspeechsynthesistaskspaginator"></a>

## ListSpeechSynthesisTasksPaginator

Type annotations for
`session.create_client("polly").get_paginator("list_speech_synthesis_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_polly.paginator import ListSpeechSynthesisTasksPaginator

session = get_session()
async with session.create_client("polly") as client:
    client: PollyClient
    paginator: ListSpeechSynthesisTasksPaginator = client.get_paginator("list_speech_synthesis_tasks")
```

Boto3 documentation:
[Polly.Paginator.ListSpeechSynthesisTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks)

Arguments for `ListSpeechSynthesisTasksPaginator.paginate` method:

- `Status`: [TaskStatusType](./literals.md#taskstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSpeechSynthesisTasksPaginator.paginate` returns
`_PageIterator`\[[ListSpeechSynthesisTasksOutputTypeDef](./type_defs.md#listspeechsynthesistasksoutputtypedef)\].

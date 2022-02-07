<a id="translateclient-for-aiobotocore-translate-module"></a>

# TranslateClient for aiobotocore Translate module

> [Index](..) > [Translate](.) > TranslateClient

Auto-generated documentation for
[Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
type annotations stubs module
[types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

- [TranslateClient for aiobotocore Translate module](#translateclient-for-aiobotocore-translate-module)
  - [TranslateClient](#translateclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_parallel_data](#create_parallel_data)
    - [delete_parallel_data](#delete_parallel_data)
    - [delete_terminology](#delete_terminology)
    - [describe_text_translation_job](#describe_text_translation_job)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_parallel_data](#get_parallel_data)
    - [get_terminology](#get_terminology)
    - [import_terminology](#import_terminology)
    - [list_parallel_data](#list_parallel_data)
    - [list_terminologies](#list_terminologies)
    - [list_text_translation_jobs](#list_text_translation_jobs)
    - [start_text_translation_job](#start_text_translation_job)
    - [stop_text_translation_job](#stop_text_translation_job)
    - [translate_text](#translate_text)
    - [update_parallel_data](#update_parallel_data)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="translateclient"></a>

## TranslateClient

Type annotations for `session.create_client("translate")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_translate.client import TranslateClient

session = get_session()
async with session.create_client("translate") as client:
    client: TranslateClient
```

Boto3 documentation:
[Translate.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_translate.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.ConflictException`
- `Exceptions.DetectedLanguageLowConfidenceException`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidFilterException`
- `Exceptions.InvalidParameterValueException`
- `Exceptions.InvalidRequestException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.TextSizeLimitExceededException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.UnsupportedLanguagePairException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

TranslateClient exceptions.

Type annotations for `session.create_client("translate").exceptions` method.

Boto3 documentation:
[Translate.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("translate").can_paginate` method.

Boto3 documentation:
[Translate.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_parallel_data"></a>

### create_parallel_data

Creates a parallel data resource in Amazon Translate by importing an input file
from Amazon S3.

Type annotations for `session.create_client("translate").create_parallel_data`
method.

Boto3 documentation:
[Translate.Client.create_parallel_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.create_parallel_data)

Asynchronous method. Use `await create_parallel_data(...)` for a synchronous
call.

Arguments mapping described in
[CreateParallelDataRequestRequestTypeDef](./type_defs.md#createparalleldatarequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ParallelDataConfig`:
  [ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef)
  *(required)*
- `ClientToken`: `str` *(required)*
- `Description`: `str`
- `EncryptionKey`: [EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef)

Returns a `Coroutine` for
[CreateParallelDataResponseTypeDef](./type_defs.md#createparalleldataresponsetypedef).

<a id="delete_parallel_data"></a>

### delete_parallel_data

Deletes a parallel data resource in Amazon Translate.

Type annotations for `session.create_client("translate").delete_parallel_data`
method.

Boto3 documentation:
[Translate.Client.delete_parallel_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.delete_parallel_data)

Asynchronous method. Use `await delete_parallel_data(...)` for a synchronous
call.

Arguments mapping described in
[DeleteParallelDataRequestRequestTypeDef](./type_defs.md#deleteparalleldatarequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DeleteParallelDataResponseTypeDef](./type_defs.md#deleteparalleldataresponsetypedef).

<a id="delete_terminology"></a>

### delete_terminology

A synchronous action that deletes a custom terminology.

Type annotations for `session.create_client("translate").delete_terminology`
method.

Boto3 documentation:
[Translate.Client.delete_terminology](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.delete_terminology)

Asynchronous method. Use `await delete_terminology(...)` for a synchronous
call.

Arguments mapping described in
[DeleteTerminologyRequestRequestTypeDef](./type_defs.md#deleteterminologyrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

<a id="describe_text_translation_job"></a>

### describe_text_translation_job

Gets the properties associated with an asynchronous batch translation job
including name, ID, status, source and target languages, input/output S3
buckets, and so on.

Type annotations for
`session.create_client("translate").describe_text_translation_job` method.

Boto3 documentation:
[Translate.Client.describe_text_translation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.describe_text_translation_job)

Asynchronous method. Use `await describe_text_translation_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeTextTranslationJobRequestRequestTypeDef](./type_defs.md#describetexttranslationjobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTextTranslationJobResponseTypeDef](./type_defs.md#describetexttranslationjobresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("translate").generate_presigned_url` method.

Boto3 documentation:
[Translate.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_parallel_data"></a>

### get_parallel_data

Provides information about a parallel data resource.

Type annotations for `session.create_client("translate").get_parallel_data`
method.

Boto3 documentation:
[Translate.Client.get_parallel_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.get_parallel_data)

Asynchronous method. Use `await get_parallel_data(...)` for a synchronous call.

Arguments mapping described in
[GetParallelDataRequestRequestTypeDef](./type_defs.md#getparalleldatarequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetParallelDataResponseTypeDef](./type_defs.md#getparalleldataresponsetypedef).

<a id="get_terminology"></a>

### get_terminology

Retrieves a custom terminology.

Type annotations for `session.create_client("translate").get_terminology`
method.

Boto3 documentation:
[Translate.Client.get_terminology](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.get_terminology)

Asynchronous method. Use `await get_terminology(...)` for a synchronous call.

Arguments mapping described in
[GetTerminologyRequestRequestTypeDef](./type_defs.md#getterminologyrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `TerminologyDataFormat`:
  [TerminologyDataFormatType](./literals.md#terminologydataformattype)

Returns a `Coroutine` for
[GetTerminologyResponseTypeDef](./type_defs.md#getterminologyresponsetypedef).

<a id="import_terminology"></a>

### import_terminology

Creates or updates a custom terminology, depending on whether or not one
already exists for the given terminology name.

Type annotations for `session.create_client("translate").import_terminology`
method.

Boto3 documentation:
[Translate.Client.import_terminology](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.import_terminology)

Asynchronous method. Use `await import_terminology(...)` for a synchronous
call.

Arguments mapping described in
[ImportTerminologyRequestRequestTypeDef](./type_defs.md#importterminologyrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `MergeStrategy`: `Literal['OVERWRITE']` (see
  [MergeStrategyType](./literals.md#mergestrategytype)) *(required)*
- `TerminologyData`:
  [TerminologyDataTypeDef](./type_defs.md#terminologydatatypedef) *(required)*
- `Description`: `str`
- `EncryptionKey`: [EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef)

Returns a `Coroutine` for
[ImportTerminologyResponseTypeDef](./type_defs.md#importterminologyresponsetypedef).

<a id="list_parallel_data"></a>

### list_parallel_data

Provides a list of your parallel data resources in Amazon Translate.

Type annotations for `session.create_client("translate").list_parallel_data`
method.

Boto3 documentation:
[Translate.Client.list_parallel_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.list_parallel_data)

Asynchronous method. Use `await list_parallel_data(...)` for a synchronous
call.

Arguments mapping described in
[ListParallelDataRequestRequestTypeDef](./type_defs.md#listparalleldatarequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListParallelDataResponseTypeDef](./type_defs.md#listparalleldataresponsetypedef).

<a id="list_terminologies"></a>

### list_terminologies

Provides a list of custom terminologies associated with your account.

Type annotations for `session.create_client("translate").list_terminologies`
method.

Boto3 documentation:
[Translate.Client.list_terminologies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.list_terminologies)

Asynchronous method. Use `await list_terminologies(...)` for a synchronous
call.

Arguments mapping described in
[ListTerminologiesRequestRequestTypeDef](./type_defs.md#listterminologiesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef).

<a id="list_text_translation_jobs"></a>

### list_text_translation_jobs

Gets a list of the batch translation jobs that you have submitted.

Type annotations for
`session.create_client("translate").list_text_translation_jobs` method.

Boto3 documentation:
[Translate.Client.list_text_translation_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.list_text_translation_jobs)

Asynchronous method. Use `await list_text_translation_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListTextTranslationJobsRequestRequestTypeDef](./type_defs.md#listtexttranslationjobsrequestrequesttypedef).

Keyword-only arguments:

- `Filter`:
  [TextTranslationJobFilterTypeDef](./type_defs.md#texttranslationjobfiltertypedef)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListTextTranslationJobsResponseTypeDef](./type_defs.md#listtexttranslationjobsresponsetypedef).

<a id="start_text_translation_job"></a>

### start_text_translation_job

Starts an asynchronous batch translation job.

Type annotations for
`session.create_client("translate").start_text_translation_job` method.

Boto3 documentation:
[Translate.Client.start_text_translation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.start_text_translation_job)

Asynchronous method. Use `await start_text_translation_job(...)` for a
synchronous call.

Arguments mapping described in
[StartTextTranslationJobRequestRequestTypeDef](./type_defs.md#starttexttranslationjobrequestrequesttypedef).

Keyword-only arguments:

- `InputDataConfig`:
  [InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) *(required)*
- `OutputDataConfig`:
  [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
  *(required)*
- `DataAccessRoleArn`: `str` *(required)*
- `SourceLanguageCode`: `str` *(required)*
- `TargetLanguageCodes`: `Sequence`\[`str`\] *(required)*
- `ClientToken`: `str` *(required)*
- `JobName`: `str`
- `TerminologyNames`: `Sequence`\[`str`\]
- `ParallelDataNames`: `Sequence`\[`str`\]
- `Settings`:
  [TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef)

Returns a `Coroutine` for
[StartTextTranslationJobResponseTypeDef](./type_defs.md#starttexttranslationjobresponsetypedef).

<a id="stop_text_translation_job"></a>

### stop_text_translation_job

Stops an asynchronous batch translation job that is in progress.

Type annotations for
`session.create_client("translate").stop_text_translation_job` method.

Boto3 documentation:
[Translate.Client.stop_text_translation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.stop_text_translation_job)

Asynchronous method. Use `await stop_text_translation_job(...)` for a
synchronous call.

Arguments mapping described in
[StopTextTranslationJobRequestRequestTypeDef](./type_defs.md#stoptexttranslationjobrequestrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[StopTextTranslationJobResponseTypeDef](./type_defs.md#stoptexttranslationjobresponsetypedef).

<a id="translate_text"></a>

### translate_text

Translates input text from the source language to the target language.

Type annotations for `session.create_client("translate").translate_text`
method.

Boto3 documentation:
[Translate.Client.translate_text](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_text)

Asynchronous method. Use `await translate_text(...)` for a synchronous call.

Arguments mapping described in
[TranslateTextRequestRequestTypeDef](./type_defs.md#translatetextrequestrequesttypedef).

Keyword-only arguments:

- `Text`: `str` *(required)*
- `SourceLanguageCode`: `str` *(required)*
- `TargetLanguageCode`: `str` *(required)*
- `TerminologyNames`: `Sequence`\[`str`\]
- `Settings`:
  [TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef)

Returns a `Coroutine` for
[TranslateTextResponseTypeDef](./type_defs.md#translatetextresponsetypedef).

<a id="update_parallel_data"></a>

### update_parallel_data

Updates a previously created parallel data resource by importing a new input
file from Amazon S3.

Type annotations for `session.create_client("translate").update_parallel_data`
method.

Boto3 documentation:
[Translate.Client.update_parallel_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.update_parallel_data)

Asynchronous method. Use `await update_parallel_data(...)` for a synchronous
call.

Arguments mapping described in
[UpdateParallelDataRequestRequestTypeDef](./type_defs.md#updateparalleldatarequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ParallelDataConfig`:
  [ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef)
  *(required)*
- `ClientToken`: `str` *(required)*
- `Description`: `str`

Returns a `Coroutine` for
[UpdateParallelDataResponseTypeDef](./type_defs.md#updateparalleldataresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("translate").__aenter__` method.

Boto3 documentation:
[Translate.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [TranslateClient](#translateclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("translate").__aexit__` method.

Boto3 documentation:
[Translate.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("translate").get_paginator` method
with overloads.

- `client.get_paginator("list_terminologies")` ->
  [ListTerminologiesPaginator](./paginators.md#listterminologiespaginator)

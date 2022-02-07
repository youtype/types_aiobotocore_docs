<a id="pollyclient-for-aiobotocore-polly-module"></a>

# PollyClient for aiobotocore Polly module

> [Index](..) > [Polly](.) > PollyClient

Auto-generated documentation for
[Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
type annotations stubs module
[types-aiobotocore-polly](https://pypi.org/project/types-aiobotocore-polly/).

- [PollyClient for aiobotocore Polly module](#pollyclient-for-aiobotocore-polly-module)
  - [PollyClient](#pollyclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [delete_lexicon](#delete_lexicon)
    - [describe_voices](#describe_voices)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_lexicon](#get_lexicon)
    - [get_speech_synthesis_task](#get_speech_synthesis_task)
    - [list_lexicons](#list_lexicons)
    - [list_speech_synthesis_tasks](#list_speech_synthesis_tasks)
    - [put_lexicon](#put_lexicon)
    - [start_speech_synthesis_task](#start_speech_synthesis_task)
    - [synthesize_speech](#synthesize_speech)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="pollyclient"></a>

## PollyClient

Type annotations for `session.create_client("polly")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_polly.client import PollyClient

session = get_session()
async with session.create_client("polly") as client:
    client: PollyClient
```

Boto3 documentation:
[Polly.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_polly.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.EngineNotSupportedException`
- `Exceptions.InvalidLexiconException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidS3BucketException`
- `Exceptions.InvalidS3KeyException`
- `Exceptions.InvalidSampleRateException`
- `Exceptions.InvalidSnsTopicArnException`
- `Exceptions.InvalidSsmlException`
- `Exceptions.InvalidTaskIdException`
- `Exceptions.LanguageNotSupportedException`
- `Exceptions.LexiconNotFoundException`
- `Exceptions.LexiconSizeExceededException`
- `Exceptions.MarksNotSupportedForFormatException`
- `Exceptions.MaxLexemeLengthExceededException`
- `Exceptions.MaxLexiconsNumberExceededException`
- `Exceptions.ServiceFailureException`
- `Exceptions.SsmlMarksNotSupportedForTextTypeException`
- `Exceptions.SynthesisTaskNotFoundException`
- `Exceptions.TextLengthExceededException`
- `Exceptions.UnsupportedPlsAlphabetException`
- `Exceptions.UnsupportedPlsLanguageException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

PollyClient exceptions.

Type annotations for `session.create_client("polly").exceptions` method.

Boto3 documentation:
[Polly.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("polly").can_paginate` method.

Boto3 documentation:
[Polly.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="delete_lexicon"></a>

### delete_lexicon

Deletes the specified pronunciation lexicon stored in an Amazon Web Services
Region.

Type annotations for `session.create_client("polly").delete_lexicon` method.

Boto3 documentation:
[Polly.Client.delete_lexicon](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.delete_lexicon)

Asynchronous method. Use `await delete_lexicon(...)` for a synchronous call.

Arguments mapping described in
[DeleteLexiconInputRequestTypeDef](./type_defs.md#deletelexiconinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_voices"></a>

### describe_voices

Returns the list of voices that are available for use when requesting speech
synthesis.

Type annotations for `session.create_client("polly").describe_voices` method.

Boto3 documentation:
[Polly.Client.describe_voices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.describe_voices)

Asynchronous method. Use `await describe_voices(...)` for a synchronous call.

Arguments mapping described in
[DescribeVoicesInputRequestTypeDef](./type_defs.md#describevoicesinputrequesttypedef).

Keyword-only arguments:

- `Engine`: [EngineType](./literals.md#enginetype)
- `LanguageCode`: [LanguageCodeType](./literals.md#languagecodetype)
- `IncludeAdditionalLanguageCodes`: `bool`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("polly").generate_presigned_url`
method.

Boto3 documentation:
[Polly.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_lexicon"></a>

### get_lexicon

Returns the content of the specified pronunciation lexicon stored in an Amazon
Web Services Region.

Type annotations for `session.create_client("polly").get_lexicon` method.

Boto3 documentation:
[Polly.Client.get_lexicon](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.get_lexicon)

Asynchronous method. Use `await get_lexicon(...)` for a synchronous call.

Arguments mapping described in
[GetLexiconInputRequestTypeDef](./type_defs.md#getlexiconinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetLexiconOutputTypeDef](./type_defs.md#getlexiconoutputtypedef).

<a id="get_speech_synthesis_task"></a>

### get_speech_synthesis_task

Retrieves a specific SpeechSynthesisTask object based on its TaskID.

Type annotations for `session.create_client("polly").get_speech_synthesis_task`
method.

Boto3 documentation:
[Polly.Client.get_speech_synthesis_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.get_speech_synthesis_task)

Asynchronous method. Use `await get_speech_synthesis_task(...)` for a
synchronous call.

Arguments mapping described in
[GetSpeechSynthesisTaskInputRequestTypeDef](./type_defs.md#getspeechsynthesistaskinputrequesttypedef).

Keyword-only arguments:

- `TaskId`: `str` *(required)*

Returns a `Coroutine` for
[GetSpeechSynthesisTaskOutputTypeDef](./type_defs.md#getspeechsynthesistaskoutputtypedef).

<a id="list_lexicons"></a>

### list_lexicons

Returns a list of pronunciation lexicons stored in an Amazon Web Services
Region.

Type annotations for `session.create_client("polly").list_lexicons` method.

Boto3 documentation:
[Polly.Client.list_lexicons](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.list_lexicons)

Asynchronous method. Use `await list_lexicons(...)` for a synchronous call.

Arguments mapping described in
[ListLexiconsInputRequestTypeDef](./type_defs.md#listlexiconsinputrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`

Returns a `Coroutine` for
[ListLexiconsOutputTypeDef](./type_defs.md#listlexiconsoutputtypedef).

<a id="list_speech_synthesis_tasks"></a>

### list_speech_synthesis_tasks

Returns a list of SpeechSynthesisTask objects ordered by their creation date.

Type annotations for
`session.create_client("polly").list_speech_synthesis_tasks` method.

Boto3 documentation:
[Polly.Client.list_speech_synthesis_tasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.list_speech_synthesis_tasks)

Asynchronous method. Use `await list_speech_synthesis_tasks(...)` for a
synchronous call.

Arguments mapping described in
[ListSpeechSynthesisTasksInputRequestTypeDef](./type_defs.md#listspeechsynthesistasksinputrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `Status`: [TaskStatusType](./literals.md#taskstatustype)

Returns a `Coroutine` for
[ListSpeechSynthesisTasksOutputTypeDef](./type_defs.md#listspeechsynthesistasksoutputtypedef).

<a id="put_lexicon"></a>

### put_lexicon

Stores a pronunciation lexicon in an Amazon Web Services Region.

Type annotations for `session.create_client("polly").put_lexicon` method.

Boto3 documentation:
[Polly.Client.put_lexicon](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.put_lexicon)

Asynchronous method. Use `await put_lexicon(...)` for a synchronous call.

Arguments mapping described in
[PutLexiconInputRequestTypeDef](./type_defs.md#putlexiconinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Content`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start_speech_synthesis_task"></a>

### start_speech_synthesis_task

Allows the creation of an asynchronous synthesis task, by starting a new
`SpeechSynthesisTask`.

Type annotations for
`session.create_client("polly").start_speech_synthesis_task` method.

Boto3 documentation:
[Polly.Client.start_speech_synthesis_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.start_speech_synthesis_task)

Asynchronous method. Use `await start_speech_synthesis_task(...)` for a
synchronous call.

Arguments mapping described in
[StartSpeechSynthesisTaskInputRequestTypeDef](./type_defs.md#startspeechsynthesistaskinputrequesttypedef).

Keyword-only arguments:

- `OutputFormat`: [OutputFormatType](./literals.md#outputformattype)
  *(required)*
- `OutputS3BucketName`: `str` *(required)*
- `Text`: `str` *(required)*
- `VoiceId`: [VoiceIdType](./literals.md#voiceidtype) *(required)*
- `Engine`: [EngineType](./literals.md#enginetype)
- `LanguageCode`: [LanguageCodeType](./literals.md#languagecodetype)
- `LexiconNames`: `Sequence`\[`str`\]
- `OutputS3KeyPrefix`: `str`
- `SampleRate`: `str`
- `SnsTopicArn`: `str`
- `SpeechMarkTypes`:
  `Sequence`\[[SpeechMarkTypeType](./literals.md#speechmarktypetype)\]
- `TextType`: [TextTypeType](./literals.md#texttypetype)

Returns a `Coroutine` for
[StartSpeechSynthesisTaskOutputTypeDef](./type_defs.md#startspeechsynthesistaskoutputtypedef).

<a id="synthesize_speech"></a>

### synthesize_speech

Synthesizes UTF-8 input, plain text or SSML, to a stream of bytes.

Type annotations for `session.create_client("polly").synthesize_speech` method.

Boto3 documentation:
[Polly.Client.synthesize_speech](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.synthesize_speech)

Asynchronous method. Use `await synthesize_speech(...)` for a synchronous call.

Arguments mapping described in
[SynthesizeSpeechInputRequestTypeDef](./type_defs.md#synthesizespeechinputrequesttypedef).

Keyword-only arguments:

- `OutputFormat`: [OutputFormatType](./literals.md#outputformattype)
  *(required)*
- `Text`: `str` *(required)*
- `VoiceId`: [VoiceIdType](./literals.md#voiceidtype) *(required)*
- `Engine`: [EngineType](./literals.md#enginetype)
- `LanguageCode`: [LanguageCodeType](./literals.md#languagecodetype)
- `LexiconNames`: `Sequence`\[`str`\]
- `SampleRate`: `str`
- `SpeechMarkTypes`:
  `Sequence`\[[SpeechMarkTypeType](./literals.md#speechmarktypetype)\]
- `TextType`: [TextTypeType](./literals.md#texttypetype)

Returns a `Coroutine` for
[SynthesizeSpeechOutputTypeDef](./type_defs.md#synthesizespeechoutputtypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("polly").__aenter__` method.

Boto3 documentation:
[Polly.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [PollyClient](#pollyclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("polly").__aexit__` method.

Boto3 documentation:
[Polly.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("polly").get_paginator` method with
overloads.

- `client.get_paginator("describe_voices")` ->
  [DescribeVoicesPaginator](./paginators.md#describevoicespaginator)
- `client.get_paginator("list_lexicons")` ->
  [ListLexiconsPaginator](./paginators.md#listlexiconspaginator)
- `client.get_paginator("list_speech_synthesis_tasks")` ->
  [ListSpeechSynthesisTasksPaginator](./paginators.md#listspeechsynthesistaskspaginator)

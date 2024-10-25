# TranscribeServiceClient

> [Index](../README.md) > [TranscribeService](./README.md) > TranscribeServiceClient

!!! note ""

    Auto-generated documentation for [TranscribeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
    type annotations stubs module [types-aiobotocore-transcribe](https://pypi.org/project/types-aiobotocore-transcribe/).

## TranscribeServiceClient

Type annotations and code completion for `#!python session.create_client("transcribe")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client)

```python
# TranscribeServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_transcribe.client import TranscribeServiceClient

session = get_session()
async with session.create_client("transcribe") as client:
    client: TranscribeServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("transcribe").exceptions` structure.

```python
# TranscribeServiceClient.exceptions usage example

async with session.create_client("transcribe") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.InternalFailureException,
        client.LimitExceededException,
        client.NotFoundException,
    ) as e:
        print(e)
```

```python
# TranscribeServiceClient usage type checking example

from types_aiobotocore_transcribe.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("transcribe").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("transcribe").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_call\_analytics\_category

Creates a new Call Analytics category.

Type annotations and code completion for `#!python session.create_client("transcribe").create_call_analytics_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)

```python
# create_call_analytics_category method definition

await def create_call_analytics_category(
    self,
    *,
    CategoryName: str,
    Rules: Sequence[RuleUnionTypeDef],  # (1)
    InputType: InputTypeType = ...,  # (2)
) -> CreateCallAnalyticsCategoryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
2. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
3. See [:material-code-braces: CreateCallAnalyticsCategoryResponseTypeDef](./type_defs.md#createcallanalyticscategoryresponsetypedef) 


```python
# create_call_analytics_category method usage example with argument unpacking

kwargs: CreateCallAnalyticsCategoryRequestRequestTypeDef = {  # (1)
    "CategoryName": ...,
    "Rules": ...,
}

parent.create_call_analytics_category(**kwargs)
```

1. See [:material-code-braces: CreateCallAnalyticsCategoryRequestRequestTypeDef](./type_defs.md#createcallanalyticscategoryrequestrequesttypedef) 

### create\_language\_model

Creates a new custom language model.

Type annotations and code completion for `#!python session.create_client("transcribe").create_language_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_language_model)

```python
# create_language_model method definition

await def create_language_model(
    self,
    *,
    LanguageCode: CLMLanguageCodeType,  # (1)
    BaseModelName: BaseModelNameType,  # (2)
    ModelName: str,
    InputDataConfig: InputDataConfigTypeDef,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateLanguageModelResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CLMLanguageCodeType](./literals.md#clmlanguagecodetype) 
2. See [:material-code-brackets: BaseModelNameType](./literals.md#basemodelnametype) 
3. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateLanguageModelResponseTypeDef](./type_defs.md#createlanguagemodelresponsetypedef) 


```python
# create_language_model method usage example with argument unpacking

kwargs: CreateLanguageModelRequestRequestTypeDef = {  # (1)
    "LanguageCode": ...,
    "BaseModelName": ...,
    "ModelName": ...,
    "InputDataConfig": ...,
}

parent.create_language_model(**kwargs)
```

1. See [:material-code-braces: CreateLanguageModelRequestRequestTypeDef](./type_defs.md#createlanguagemodelrequestrequesttypedef) 

### create\_medical\_vocabulary

Creates a new custom medical vocabulary.

Type annotations and code completion for `#!python session.create_client("transcribe").create_medical_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_medical_vocabulary)

```python
# create_medical_vocabulary method definition

await def create_medical_vocabulary(
    self,
    *,
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyFileUri: str,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateMedicalVocabularyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateMedicalVocabularyResponseTypeDef](./type_defs.md#createmedicalvocabularyresponsetypedef) 


```python
# create_medical_vocabulary method usage example with argument unpacking

kwargs: CreateMedicalVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
    "LanguageCode": ...,
    "VocabularyFileUri": ...,
}

parent.create_medical_vocabulary(**kwargs)
```

1. See [:material-code-braces: CreateMedicalVocabularyRequestRequestTypeDef](./type_defs.md#createmedicalvocabularyrequestrequesttypedef) 

### create\_vocabulary

Creates a new custom vocabulary.

Type annotations and code completion for `#!python session.create_client("transcribe").create_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary)

```python
# create_vocabulary method definition

await def create_vocabulary(
    self,
    *,
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Phrases: Sequence[str] = ...,
    VocabularyFileUri: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    DataAccessRoleArn: str = ...,
) -> CreateVocabularyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateVocabularyResponseTypeDef](./type_defs.md#createvocabularyresponsetypedef) 


```python
# create_vocabulary method usage example with argument unpacking

kwargs: CreateVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
    "LanguageCode": ...,
}

parent.create_vocabulary(**kwargs)
```

1. See [:material-code-braces: CreateVocabularyRequestRequestTypeDef](./type_defs.md#createvocabularyrequestrequesttypedef) 

### create\_vocabulary\_filter

Creates a new custom vocabulary filter.

Type annotations and code completion for `#!python session.create_client("transcribe").create_vocabulary_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary_filter)

```python
# create_vocabulary_filter method definition

await def create_vocabulary_filter(
    self,
    *,
    VocabularyFilterName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Words: Sequence[str] = ...,
    VocabularyFilterFileUri: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    DataAccessRoleArn: str = ...,
) -> CreateVocabularyFilterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateVocabularyFilterResponseTypeDef](./type_defs.md#createvocabularyfilterresponsetypedef) 


```python
# create_vocabulary_filter method usage example with argument unpacking

kwargs: CreateVocabularyFilterRequestRequestTypeDef = {  # (1)
    "VocabularyFilterName": ...,
    "LanguageCode": ...,
}

parent.create_vocabulary_filter(**kwargs)
```

1. See [:material-code-braces: CreateVocabularyFilterRequestRequestTypeDef](./type_defs.md#createvocabularyfilterrequestrequesttypedef) 

### delete\_call\_analytics\_category

Deletes a Call Analytics category.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_call_analytics_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_call_analytics_category)

```python
# delete_call_analytics_category method definition

await def delete_call_analytics_category(
    self,
    *,
    CategoryName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_call_analytics_category method usage example with argument unpacking

kwargs: DeleteCallAnalyticsCategoryRequestRequestTypeDef = {  # (1)
    "CategoryName": ...,
}

parent.delete_call_analytics_category(**kwargs)
```

1. See [:material-code-braces: DeleteCallAnalyticsCategoryRequestRequestTypeDef](./type_defs.md#deletecallanalyticscategoryrequestrequesttypedef) 

### delete\_call\_analytics\_job

Deletes a Call Analytics job.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_call_analytics_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_call_analytics_job)

```python
# delete_call_analytics_job method definition

await def delete_call_analytics_job(
    self,
    *,
    CallAnalyticsJobName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_call_analytics_job method usage example with argument unpacking

kwargs: DeleteCallAnalyticsJobRequestRequestTypeDef = {  # (1)
    "CallAnalyticsJobName": ...,
}

parent.delete_call_analytics_job(**kwargs)
```

1. See [:material-code-braces: DeleteCallAnalyticsJobRequestRequestTypeDef](./type_defs.md#deletecallanalyticsjobrequestrequesttypedef) 

### delete\_language\_model

Deletes a custom language model.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_language_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_language_model)

```python
# delete_language_model method definition

await def delete_language_model(
    self,
    *,
    ModelName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_language_model method usage example with argument unpacking

kwargs: DeleteLanguageModelRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.delete_language_model(**kwargs)
```

1. See [:material-code-braces: DeleteLanguageModelRequestRequestTypeDef](./type_defs.md#deletelanguagemodelrequestrequesttypedef) 

### delete\_medical\_scribe\_job

Deletes a Medical Scribe job.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_medical_scribe_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_medical_scribe_job)

```python
# delete_medical_scribe_job method definition

await def delete_medical_scribe_job(
    self,
    *,
    MedicalScribeJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_medical_scribe_job method usage example with argument unpacking

kwargs: DeleteMedicalScribeJobRequestRequestTypeDef = {  # (1)
    "MedicalScribeJobName": ...,
}

parent.delete_medical_scribe_job(**kwargs)
```

1. See [:material-code-braces: DeleteMedicalScribeJobRequestRequestTypeDef](./type_defs.md#deletemedicalscribejobrequestrequesttypedef) 

### delete\_medical\_transcription\_job

Deletes a medical transcription job.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_medical_transcription_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_medical_transcription_job)

```python
# delete_medical_transcription_job method definition

await def delete_medical_transcription_job(
    self,
    *,
    MedicalTranscriptionJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_medical_transcription_job method usage example with argument unpacking

kwargs: DeleteMedicalTranscriptionJobRequestRequestTypeDef = {  # (1)
    "MedicalTranscriptionJobName": ...,
}

parent.delete_medical_transcription_job(**kwargs)
```

1. See [:material-code-braces: DeleteMedicalTranscriptionJobRequestRequestTypeDef](./type_defs.md#deletemedicaltranscriptionjobrequestrequesttypedef) 

### delete\_medical\_vocabulary

Deletes a custom medical vocabulary.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_medical_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_medical_vocabulary)

```python
# delete_medical_vocabulary method definition

await def delete_medical_vocabulary(
    self,
    *,
    VocabularyName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_medical_vocabulary method usage example with argument unpacking

kwargs: DeleteMedicalVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
}

parent.delete_medical_vocabulary(**kwargs)
```

1. See [:material-code-braces: DeleteMedicalVocabularyRequestRequestTypeDef](./type_defs.md#deletemedicalvocabularyrequestrequesttypedef) 

### delete\_transcription\_job

Deletes a transcription job.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_transcription_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_transcription_job)

```python
# delete_transcription_job method definition

await def delete_transcription_job(
    self,
    *,
    TranscriptionJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_transcription_job method usage example with argument unpacking

kwargs: DeleteTranscriptionJobRequestRequestTypeDef = {  # (1)
    "TranscriptionJobName": ...,
}

parent.delete_transcription_job(**kwargs)
```

1. See [:material-code-braces: DeleteTranscriptionJobRequestRequestTypeDef](./type_defs.md#deletetranscriptionjobrequestrequesttypedef) 

### delete\_vocabulary

Deletes a custom vocabulary.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_vocabulary)

```python
# delete_vocabulary method definition

await def delete_vocabulary(
    self,
    *,
    VocabularyName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_vocabulary method usage example with argument unpacking

kwargs: DeleteVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
}

parent.delete_vocabulary(**kwargs)
```

1. See [:material-code-braces: DeleteVocabularyRequestRequestTypeDef](./type_defs.md#deletevocabularyrequestrequesttypedef) 

### delete\_vocabulary\_filter

Deletes a custom vocabulary filter.

Type annotations and code completion for `#!python session.create_client("transcribe").delete_vocabulary_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_vocabulary_filter)

```python
# delete_vocabulary_filter method definition

await def delete_vocabulary_filter(
    self,
    *,
    VocabularyFilterName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_vocabulary_filter method usage example with argument unpacking

kwargs: DeleteVocabularyFilterRequestRequestTypeDef = {  # (1)
    "VocabularyFilterName": ...,
}

parent.delete_vocabulary_filter(**kwargs)
```

1. See [:material-code-braces: DeleteVocabularyFilterRequestRequestTypeDef](./type_defs.md#deletevocabularyfilterrequestrequesttypedef) 

### describe\_language\_model

Provides information about the specified custom language model.

Type annotations and code completion for `#!python session.create_client("transcribe").describe_language_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.describe_language_model)

```python
# describe_language_model method definition

await def describe_language_model(
    self,
    *,
    ModelName: str,
) -> DescribeLanguageModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLanguageModelResponseTypeDef](./type_defs.md#describelanguagemodelresponsetypedef) 


```python
# describe_language_model method usage example with argument unpacking

kwargs: DescribeLanguageModelRequestRequestTypeDef = {  # (1)
    "ModelName": ...,
}

parent.describe_language_model(**kwargs)
```

1. See [:material-code-braces: DescribeLanguageModelRequestRequestTypeDef](./type_defs.md#describelanguagemodelrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("transcribe").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_call\_analytics\_category

Provides information about the specified Call Analytics category.

Type annotations and code completion for `#!python session.create_client("transcribe").get_call_analytics_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_call_analytics_category)

```python
# get_call_analytics_category method definition

await def get_call_analytics_category(
    self,
    *,
    CategoryName: str,
) -> GetCallAnalyticsCategoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCallAnalyticsCategoryResponseTypeDef](./type_defs.md#getcallanalyticscategoryresponsetypedef) 


```python
# get_call_analytics_category method usage example with argument unpacking

kwargs: GetCallAnalyticsCategoryRequestRequestTypeDef = {  # (1)
    "CategoryName": ...,
}

parent.get_call_analytics_category(**kwargs)
```

1. See [:material-code-braces: GetCallAnalyticsCategoryRequestRequestTypeDef](./type_defs.md#getcallanalyticscategoryrequestrequesttypedef) 

### get\_call\_analytics\_job

Provides information about the specified Call Analytics job.

Type annotations and code completion for `#!python session.create_client("transcribe").get_call_analytics_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_call_analytics_job)

```python
# get_call_analytics_job method definition

await def get_call_analytics_job(
    self,
    *,
    CallAnalyticsJobName: str,
) -> GetCallAnalyticsJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCallAnalyticsJobResponseTypeDef](./type_defs.md#getcallanalyticsjobresponsetypedef) 


```python
# get_call_analytics_job method usage example with argument unpacking

kwargs: GetCallAnalyticsJobRequestRequestTypeDef = {  # (1)
    "CallAnalyticsJobName": ...,
}

parent.get_call_analytics_job(**kwargs)
```

1. See [:material-code-braces: GetCallAnalyticsJobRequestRequestTypeDef](./type_defs.md#getcallanalyticsjobrequestrequesttypedef) 

### get\_medical\_scribe\_job

Provides information about the specified Medical Scribe job.

Type annotations and code completion for `#!python session.create_client("transcribe").get_medical_scribe_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_medical_scribe_job)

```python
# get_medical_scribe_job method definition

await def get_medical_scribe_job(
    self,
    *,
    MedicalScribeJobName: str,
) -> GetMedicalScribeJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMedicalScribeJobResponseTypeDef](./type_defs.md#getmedicalscribejobresponsetypedef) 


```python
# get_medical_scribe_job method usage example with argument unpacking

kwargs: GetMedicalScribeJobRequestRequestTypeDef = {  # (1)
    "MedicalScribeJobName": ...,
}

parent.get_medical_scribe_job(**kwargs)
```

1. See [:material-code-braces: GetMedicalScribeJobRequestRequestTypeDef](./type_defs.md#getmedicalscribejobrequestrequesttypedef) 

### get\_medical\_transcription\_job

Provides information about the specified medical transcription job.

Type annotations and code completion for `#!python session.create_client("transcribe").get_medical_transcription_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_medical_transcription_job)

```python
# get_medical_transcription_job method definition

await def get_medical_transcription_job(
    self,
    *,
    MedicalTranscriptionJobName: str,
) -> GetMedicalTranscriptionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMedicalTranscriptionJobResponseTypeDef](./type_defs.md#getmedicaltranscriptionjobresponsetypedef) 


```python
# get_medical_transcription_job method usage example with argument unpacking

kwargs: GetMedicalTranscriptionJobRequestRequestTypeDef = {  # (1)
    "MedicalTranscriptionJobName": ...,
}

parent.get_medical_transcription_job(**kwargs)
```

1. See [:material-code-braces: GetMedicalTranscriptionJobRequestRequestTypeDef](./type_defs.md#getmedicaltranscriptionjobrequestrequesttypedef) 

### get\_medical\_vocabulary

Provides information about the specified custom medical vocabulary.

Type annotations and code completion for `#!python session.create_client("transcribe").get_medical_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_medical_vocabulary)

```python
# get_medical_vocabulary method definition

await def get_medical_vocabulary(
    self,
    *,
    VocabularyName: str,
) -> GetMedicalVocabularyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMedicalVocabularyResponseTypeDef](./type_defs.md#getmedicalvocabularyresponsetypedef) 


```python
# get_medical_vocabulary method usage example with argument unpacking

kwargs: GetMedicalVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
}

parent.get_medical_vocabulary(**kwargs)
```

1. See [:material-code-braces: GetMedicalVocabularyRequestRequestTypeDef](./type_defs.md#getmedicalvocabularyrequestrequesttypedef) 

### get\_transcription\_job

Provides information about the specified transcription job.

Type annotations and code completion for `#!python session.create_client("transcribe").get_transcription_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_transcription_job)

```python
# get_transcription_job method definition

await def get_transcription_job(
    self,
    *,
    TranscriptionJobName: str,
) -> GetTranscriptionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTranscriptionJobResponseTypeDef](./type_defs.md#gettranscriptionjobresponsetypedef) 


```python
# get_transcription_job method usage example with argument unpacking

kwargs: GetTranscriptionJobRequestRequestTypeDef = {  # (1)
    "TranscriptionJobName": ...,
}

parent.get_transcription_job(**kwargs)
```

1. See [:material-code-braces: GetTranscriptionJobRequestRequestTypeDef](./type_defs.md#gettranscriptionjobrequestrequesttypedef) 

### get\_vocabulary

Provides information about the specified custom vocabulary.

Type annotations and code completion for `#!python session.create_client("transcribe").get_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_vocabulary)

```python
# get_vocabulary method definition

await def get_vocabulary(
    self,
    *,
    VocabularyName: str,
) -> GetVocabularyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVocabularyResponseTypeDef](./type_defs.md#getvocabularyresponsetypedef) 


```python
# get_vocabulary method usage example with argument unpacking

kwargs: GetVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
}

parent.get_vocabulary(**kwargs)
```

1. See [:material-code-braces: GetVocabularyRequestRequestTypeDef](./type_defs.md#getvocabularyrequestrequesttypedef) 

### get\_vocabulary\_filter

Provides information about the specified custom vocabulary filter.

Type annotations and code completion for `#!python session.create_client("transcribe").get_vocabulary_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_vocabulary_filter)

```python
# get_vocabulary_filter method definition

await def get_vocabulary_filter(
    self,
    *,
    VocabularyFilterName: str,
) -> GetVocabularyFilterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVocabularyFilterResponseTypeDef](./type_defs.md#getvocabularyfilterresponsetypedef) 


```python
# get_vocabulary_filter method usage example with argument unpacking

kwargs: GetVocabularyFilterRequestRequestTypeDef = {  # (1)
    "VocabularyFilterName": ...,
}

parent.get_vocabulary_filter(**kwargs)
```

1. See [:material-code-braces: GetVocabularyFilterRequestRequestTypeDef](./type_defs.md#getvocabularyfilterrequestrequesttypedef) 

### list\_call\_analytics\_categories

Provides a list of Call Analytics categories, including all rules that make up
each
category.

Type annotations and code completion for `#!python session.create_client("transcribe").list_call_analytics_categories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_categories)

```python
# list_call_analytics_categories method definition

await def list_call_analytics_categories(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCallAnalyticsCategoriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCallAnalyticsCategoriesResponseTypeDef](./type_defs.md#listcallanalyticscategoriesresponsetypedef) 


```python
# list_call_analytics_categories method usage example with argument unpacking

kwargs: ListCallAnalyticsCategoriesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_call_analytics_categories(**kwargs)
```

1. See [:material-code-braces: ListCallAnalyticsCategoriesRequestRequestTypeDef](./type_defs.md#listcallanalyticscategoriesrequestrequesttypedef) 

### list\_call\_analytics\_jobs

Provides a list of Call Analytics jobs that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_call_analytics_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_jobs)

```python
# list_call_analytics_jobs method definition

await def list_call_analytics_jobs(
    self,
    *,
    Status: CallAnalyticsJobStatusType = ...,  # (1)
    JobNameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCallAnalyticsJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CallAnalyticsJobStatusType](./literals.md#callanalyticsjobstatustype) 
2. See [:material-code-braces: ListCallAnalyticsJobsResponseTypeDef](./type_defs.md#listcallanalyticsjobsresponsetypedef) 


```python
# list_call_analytics_jobs method usage example with argument unpacking

kwargs: ListCallAnalyticsJobsRequestRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_call_analytics_jobs(**kwargs)
```

1. See [:material-code-braces: ListCallAnalyticsJobsRequestRequestTypeDef](./type_defs.md#listcallanalyticsjobsrequestrequesttypedef) 

### list\_language\_models

Provides a list of custom language models that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_language_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_language_models)

```python
# list_language_models method definition

await def list_language_models(
    self,
    *,
    StatusEquals: ModelStatusType = ...,  # (1)
    NameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLanguageModelsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
2. See [:material-code-braces: ListLanguageModelsResponseTypeDef](./type_defs.md#listlanguagemodelsresponsetypedef) 


```python
# list_language_models method usage example with argument unpacking

kwargs: ListLanguageModelsRequestRequestTypeDef = {  # (1)
    "StatusEquals": ...,
}

parent.list_language_models(**kwargs)
```

1. See [:material-code-braces: ListLanguageModelsRequestRequestTypeDef](./type_defs.md#listlanguagemodelsrequestrequesttypedef) 

### list\_medical\_scribe\_jobs

Provides a list of Medical Scribe jobs that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_medical_scribe_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_scribe_jobs)

```python
# list_medical_scribe_jobs method definition

await def list_medical_scribe_jobs(
    self,
    *,
    Status: MedicalScribeJobStatusType = ...,  # (1)
    JobNameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMedicalScribeJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MedicalScribeJobStatusType](./literals.md#medicalscribejobstatustype) 
2. See [:material-code-braces: ListMedicalScribeJobsResponseTypeDef](./type_defs.md#listmedicalscribejobsresponsetypedef) 


```python
# list_medical_scribe_jobs method usage example with argument unpacking

kwargs: ListMedicalScribeJobsRequestRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_medical_scribe_jobs(**kwargs)
```

1. See [:material-code-braces: ListMedicalScribeJobsRequestRequestTypeDef](./type_defs.md#listmedicalscribejobsrequestrequesttypedef) 

### list\_medical\_transcription\_jobs

Provides a list of medical transcription jobs that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_medical_transcription_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_transcription_jobs)

```python
# list_medical_transcription_jobs method definition

await def list_medical_transcription_jobs(
    self,
    *,
    Status: TranscriptionJobStatusType = ...,  # (1)
    JobNameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMedicalTranscriptionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
2. See [:material-code-braces: ListMedicalTranscriptionJobsResponseTypeDef](./type_defs.md#listmedicaltranscriptionjobsresponsetypedef) 


```python
# list_medical_transcription_jobs method usage example with argument unpacking

kwargs: ListMedicalTranscriptionJobsRequestRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_medical_transcription_jobs(**kwargs)
```

1. See [:material-code-braces: ListMedicalTranscriptionJobsRequestRequestTypeDef](./type_defs.md#listmedicaltranscriptionjobsrequestrequesttypedef) 

### list\_medical\_vocabularies

Provides a list of custom medical vocabularies that match the specified
criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_medical_vocabularies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_vocabularies)

```python
# list_medical_vocabularies method definition

await def list_medical_vocabularies(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    StateEquals: VocabularyStateType = ...,  # (1)
    NameContains: str = ...,
) -> ListMedicalVocabulariesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: ListMedicalVocabulariesResponseTypeDef](./type_defs.md#listmedicalvocabulariesresponsetypedef) 


```python
# list_medical_vocabularies method usage example with argument unpacking

kwargs: ListMedicalVocabulariesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_medical_vocabularies(**kwargs)
```

1. See [:material-code-braces: ListMedicalVocabulariesRequestRequestTypeDef](./type_defs.md#listmedicalvocabulariesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags associated with the specified transcription job, vocabulary,
model, or
resource.

Type annotations and code completion for `#!python session.create_client("transcribe").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_transcription\_jobs

Provides a list of transcription jobs that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_transcription_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_transcription_jobs)

```python
# list_transcription_jobs method definition

await def list_transcription_jobs(
    self,
    *,
    Status: TranscriptionJobStatusType = ...,  # (1)
    JobNameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTranscriptionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
2. See [:material-code-braces: ListTranscriptionJobsResponseTypeDef](./type_defs.md#listtranscriptionjobsresponsetypedef) 


```python
# list_transcription_jobs method usage example with argument unpacking

kwargs: ListTranscriptionJobsRequestRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_transcription_jobs(**kwargs)
```

1. See [:material-code-braces: ListTranscriptionJobsRequestRequestTypeDef](./type_defs.md#listtranscriptionjobsrequestrequesttypedef) 

### list\_vocabularies

Provides a list of custom vocabularies that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_vocabularies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabularies)

```python
# list_vocabularies method definition

await def list_vocabularies(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    StateEquals: VocabularyStateType = ...,  # (1)
    NameContains: str = ...,
) -> ListVocabulariesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: ListVocabulariesResponseTypeDef](./type_defs.md#listvocabulariesresponsetypedef) 


```python
# list_vocabularies method usage example with argument unpacking

kwargs: ListVocabulariesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_vocabularies(**kwargs)
```

1. See [:material-code-braces: ListVocabulariesRequestRequestTypeDef](./type_defs.md#listvocabulariesrequestrequesttypedef) 

### list\_vocabulary\_filters

Provides a list of custom vocabulary filters that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("transcribe").list_vocabulary_filters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabulary_filters)

```python
# list_vocabulary_filters method definition

await def list_vocabulary_filters(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
) -> ListVocabularyFiltersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVocabularyFiltersResponseTypeDef](./type_defs.md#listvocabularyfiltersresponsetypedef) 


```python
# list_vocabulary_filters method usage example with argument unpacking

kwargs: ListVocabularyFiltersRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_vocabulary_filters(**kwargs)
```

1. See [:material-code-braces: ListVocabularyFiltersRequestRequestTypeDef](./type_defs.md#listvocabularyfiltersrequestrequesttypedef) 

### start\_call\_analytics\_job

Transcribes the audio from a customer service call and applies any additional
Request Parameters you choose to include in your
request.

Type annotations and code completion for `#!python session.create_client("transcribe").start_call_analytics_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)

```python
# start_call_analytics_job method definition

await def start_call_analytics_job(
    self,
    *,
    CallAnalyticsJobName: str,
    Media: MediaTypeDef,  # (1)
    OutputLocation: str = ...,
    OutputEncryptionKMSKeyId: str = ...,
    DataAccessRoleArn: str = ...,
    Settings: CallAnalyticsJobSettingsTypeDef = ...,  # (2)
    ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...,  # (3)
) -> StartCallAnalyticsJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
2. See [:material-code-braces: CallAnalyticsJobSettingsTypeDef](./type_defs.md#callanalyticsjobsettingstypedef) 
3. See [:material-code-braces: ChannelDefinitionTypeDef](./type_defs.md#channeldefinitiontypedef) 
4. See [:material-code-braces: StartCallAnalyticsJobResponseTypeDef](./type_defs.md#startcallanalyticsjobresponsetypedef) 


```python
# start_call_analytics_job method usage example with argument unpacking

kwargs: StartCallAnalyticsJobRequestRequestTypeDef = {  # (1)
    "CallAnalyticsJobName": ...,
    "Media": ...,
}

parent.start_call_analytics_job(**kwargs)
```

1. See [:material-code-braces: StartCallAnalyticsJobRequestRequestTypeDef](./type_defs.md#startcallanalyticsjobrequestrequesttypedef) 

### start\_medical\_scribe\_job

Transcribes patient-clinician conversations and generates clinical notes.

Type annotations and code completion for `#!python session.create_client("transcribe").start_medical_scribe_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_scribe_job)

```python
# start_medical_scribe_job method definition

await def start_medical_scribe_job(
    self,
    *,
    MedicalScribeJobName: str,
    Media: MediaTypeDef,  # (1)
    OutputBucketName: str,
    DataAccessRoleArn: str,
    Settings: MedicalScribeSettingsTypeDef,  # (2)
    OutputEncryptionKMSKeyId: str = ...,
    KMSEncryptionContext: Mapping[str, str] = ...,
    ChannelDefinitions: Sequence[MedicalScribeChannelDefinitionTypeDef] = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> StartMedicalScribeJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
2. See [:material-code-braces: MedicalScribeSettingsTypeDef](./type_defs.md#medicalscribesettingstypedef) 
3. See [:material-code-braces: MedicalScribeChannelDefinitionTypeDef](./type_defs.md#medicalscribechanneldefinitiontypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: StartMedicalScribeJobResponseTypeDef](./type_defs.md#startmedicalscribejobresponsetypedef) 


```python
# start_medical_scribe_job method usage example with argument unpacking

kwargs: StartMedicalScribeJobRequestRequestTypeDef = {  # (1)
    "MedicalScribeJobName": ...,
    "Media": ...,
    "OutputBucketName": ...,
    "DataAccessRoleArn": ...,
    "Settings": ...,
}

parent.start_medical_scribe_job(**kwargs)
```

1. See [:material-code-braces: StartMedicalScribeJobRequestRequestTypeDef](./type_defs.md#startmedicalscribejobrequestrequesttypedef) 

### start\_medical\_transcription\_job

Transcribes the audio from a medical dictation or conversation and applies any
additional Request Parameters you choose to include in your
request.

Type annotations and code completion for `#!python session.create_client("transcribe").start_medical_transcription_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_transcription_job)

```python
# start_medical_transcription_job method definition

await def start_medical_transcription_job(
    self,
    *,
    MedicalTranscriptionJobName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Media: MediaTypeDef,  # (2)
    OutputBucketName: str,
    Specialty: SpecialtyType,  # (3)
    Type: TypeType,  # (4)
    MediaSampleRateHertz: int = ...,
    MediaFormat: MediaFormatType = ...,  # (5)
    OutputKey: str = ...,
    OutputEncryptionKMSKeyId: str = ...,
    KMSEncryptionContext: Mapping[str, str] = ...,
    Settings: MedicalTranscriptionSettingTypeDef = ...,  # (6)
    ContentIdentificationType: MedicalContentIdentificationTypeType = ...,  # (7)
    Tags: Sequence[TagTypeDef] = ...,  # (8)
) -> StartMedicalTranscriptionJobResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
3. See [:material-code-brackets: SpecialtyType](./literals.md#specialtytype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
5. See [:material-code-brackets: MediaFormatType](./literals.md#mediaformattype) 
6. See [:material-code-braces: MedicalTranscriptionSettingTypeDef](./type_defs.md#medicaltranscriptionsettingtypedef) 
7. See [:material-code-brackets: MedicalContentIdentificationTypeType](./literals.md#medicalcontentidentificationtypetype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: StartMedicalTranscriptionJobResponseTypeDef](./type_defs.md#startmedicaltranscriptionjobresponsetypedef) 


```python
# start_medical_transcription_job method usage example with argument unpacking

kwargs: StartMedicalTranscriptionJobRequestRequestTypeDef = {  # (1)
    "MedicalTranscriptionJobName": ...,
    "LanguageCode": ...,
    "Media": ...,
    "OutputBucketName": ...,
    "Specialty": ...,
    "Type": ...,
}

parent.start_medical_transcription_job(**kwargs)
```

1. See [:material-code-braces: StartMedicalTranscriptionJobRequestRequestTypeDef](./type_defs.md#startmedicaltranscriptionjobrequestrequesttypedef) 

### start\_transcription\_job

Transcribes the audio from a media file and applies any additional Request
Parameters you choose to include in your
request.

Type annotations and code completion for `#!python session.create_client("transcribe").start_transcription_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)

```python
# start_transcription_job method definition

await def start_transcription_job(
    self,
    *,
    TranscriptionJobName: str,
    Media: MediaTypeDef,  # (1)
    LanguageCode: LanguageCodeType = ...,  # (2)
    MediaSampleRateHertz: int = ...,
    MediaFormat: MediaFormatType = ...,  # (3)
    OutputBucketName: str = ...,
    OutputKey: str = ...,
    OutputEncryptionKMSKeyId: str = ...,
    KMSEncryptionContext: Mapping[str, str] = ...,
    Settings: SettingsTypeDef = ...,  # (4)
    ModelSettings: ModelSettingsTypeDef = ...,  # (5)
    JobExecutionSettings: JobExecutionSettingsTypeDef = ...,  # (6)
    ContentRedaction: ContentRedactionTypeDef = ...,  # (7)
    IdentifyLanguage: bool = ...,
    IdentifyMultipleLanguages: bool = ...,
    LanguageOptions: Sequence[LanguageCodeType] = ...,  # (8)
    Subtitles: SubtitlesTypeDef = ...,  # (9)
    Tags: Sequence[TagTypeDef] = ...,  # (10)
    LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,  # (11)
    ToxicityDetection: Sequence[ToxicityDetectionSettingsUnionTypeDef] = ...,  # (12)
) -> StartTranscriptionJobResponseTypeDef:  # (13)
    ...
```

1. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-brackets: MediaFormatType](./literals.md#mediaformattype) 
4. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
5. See [:material-code-braces: ModelSettingsTypeDef](./type_defs.md#modelsettingstypedef) 
6. See [:material-code-braces: JobExecutionSettingsTypeDef](./type_defs.md#jobexecutionsettingstypedef) 
7. See [:material-code-braces: ContentRedactionTypeDef](./type_defs.md#contentredactiontypedef) 
8. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
9. See [:material-code-braces: SubtitlesTypeDef](./type_defs.md#subtitlestypedef) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) [:material-code-braces: LanguageIdSettingsTypeDef](./type_defs.md#languageidsettingstypedef) 
12. See [:material-code-braces: ToxicityDetectionSettingsTypeDef](./type_defs.md#toxicitydetectionsettingstypedef) [:material-code-braces: ToxicityDetectionSettingsOutputTypeDef](./type_defs.md#toxicitydetectionsettingsoutputtypedef) 
13. See [:material-code-braces: StartTranscriptionJobResponseTypeDef](./type_defs.md#starttranscriptionjobresponsetypedef) 


```python
# start_transcription_job method usage example with argument unpacking

kwargs: StartTranscriptionJobRequestRequestTypeDef = {  # (1)
    "TranscriptionJobName": ...,
    "Media": ...,
}

parent.start_transcription_job(**kwargs)
```

1. See [:material-code-braces: StartTranscriptionJobRequestRequestTypeDef](./type_defs.md#starttranscriptionjobrequestrequesttypedef) 

### tag\_resource

Adds one or more custom tags, each in the form of a key:value pair, to the
specified
resource.

Type annotations and code completion for `#!python session.create_client("transcribe").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified Amazon Transcribe resource.

Type annotations and code completion for `#!python session.create_client("transcribe").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_call\_analytics\_category

Updates the specified Call Analytics category with new rules.

Type annotations and code completion for `#!python session.create_client("transcribe").update_call_analytics_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)

```python
# update_call_analytics_category method definition

await def update_call_analytics_category(
    self,
    *,
    CategoryName: str,
    Rules: Sequence[RuleTypeDef],  # (1)
    InputType: InputTypeType = ...,  # (2)
) -> UpdateCallAnalyticsCategoryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
3. See [:material-code-braces: UpdateCallAnalyticsCategoryResponseTypeDef](./type_defs.md#updatecallanalyticscategoryresponsetypedef) 


```python
# update_call_analytics_category method usage example with argument unpacking

kwargs: UpdateCallAnalyticsCategoryRequestRequestTypeDef = {  # (1)
    "CategoryName": ...,
    "Rules": ...,
}

parent.update_call_analytics_category(**kwargs)
```

1. See [:material-code-braces: UpdateCallAnalyticsCategoryRequestRequestTypeDef](./type_defs.md#updatecallanalyticscategoryrequestrequesttypedef) 

### update\_medical\_vocabulary

Updates an existing custom medical vocabulary with new values.

Type annotations and code completion for `#!python session.create_client("transcribe").update_medical_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_medical_vocabulary)

```python
# update_medical_vocabulary method definition

await def update_medical_vocabulary(
    self,
    *,
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyFileUri: str,
) -> UpdateMedicalVocabularyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: UpdateMedicalVocabularyResponseTypeDef](./type_defs.md#updatemedicalvocabularyresponsetypedef) 


```python
# update_medical_vocabulary method usage example with argument unpacking

kwargs: UpdateMedicalVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
    "LanguageCode": ...,
    "VocabularyFileUri": ...,
}

parent.update_medical_vocabulary(**kwargs)
```

1. See [:material-code-braces: UpdateMedicalVocabularyRequestRequestTypeDef](./type_defs.md#updatemedicalvocabularyrequestrequesttypedef) 

### update\_vocabulary

Updates an existing custom vocabulary with new values.

Type annotations and code completion for `#!python session.create_client("transcribe").update_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary)

```python
# update_vocabulary method definition

await def update_vocabulary(
    self,
    *,
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Phrases: Sequence[str] = ...,
    VocabularyFileUri: str = ...,
    DataAccessRoleArn: str = ...,
) -> UpdateVocabularyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: UpdateVocabularyResponseTypeDef](./type_defs.md#updatevocabularyresponsetypedef) 


```python
# update_vocabulary method usage example with argument unpacking

kwargs: UpdateVocabularyRequestRequestTypeDef = {  # (1)
    "VocabularyName": ...,
    "LanguageCode": ...,
}

parent.update_vocabulary(**kwargs)
```

1. See [:material-code-braces: UpdateVocabularyRequestRequestTypeDef](./type_defs.md#updatevocabularyrequestrequesttypedef) 

### update\_vocabulary\_filter

Updates an existing custom vocabulary filter with a new list of words.

Type annotations and code completion for `#!python session.create_client("transcribe").update_vocabulary_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary_filter)

```python
# update_vocabulary_filter method definition

await def update_vocabulary_filter(
    self,
    *,
    VocabularyFilterName: str,
    Words: Sequence[str] = ...,
    VocabularyFilterFileUri: str = ...,
    DataAccessRoleArn: str = ...,
) -> UpdateVocabularyFilterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVocabularyFilterResponseTypeDef](./type_defs.md#updatevocabularyfilterresponsetypedef) 


```python
# update_vocabulary_filter method usage example with argument unpacking

kwargs: UpdateVocabularyFilterRequestRequestTypeDef = {  # (1)
    "VocabularyFilterName": ...,
}

parent.update_vocabulary_filter(**kwargs)
```

1. See [:material-code-braces: UpdateVocabularyFilterRequestRequestTypeDef](./type_defs.md#updatevocabularyfilterrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("transcribe").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "TranscribeServiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("transcribe").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```






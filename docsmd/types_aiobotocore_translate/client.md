# TranslateClient

> [Index](../README.md) > [Translate](./README.md) > TranslateClient

!!! note ""

    Auto-generated documentation for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#translate)
    type annotations stubs module [types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

## TranslateClient

Type annotations and code completion for `#!python session.create_client("translate")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client)

```python
# TranslateClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_translate.client import TranslateClient

session = get_session()
async with session.create_client("translate") as client:
    client: TranslateClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("translate").exceptions` structure.

```python
# TranslateClient.exceptions usage example

async with session.create_client("translate") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConcurrentModificationException,
        client.ConflictException,
        client.DetectedLanguageLowConfidenceException,
        client.InternalServerException,
        client.InvalidFilterException,
        client.InvalidParameterValueException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.TextSizeLimitExceededException,
        client.TooManyRequestsException,
        client.TooManyTagsException,
        client.UnsupportedDisplayLanguageCodeException,
        client.UnsupportedLanguagePairException,
    ) as e:
        print(e)
```

```python
# TranslateClient usage type checking example

from types_aiobotocore_translate.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("translate").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("translate").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("translate").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_parallel\_data

Creates a parallel data resource in Amazon Translate by importing an input file
from Amazon S3.

Type annotations and code completion for `#!python session.create_client("translate").create_parallel_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/create_parallel_data.html)

```python
# create_parallel_data method definition

await def create_parallel_data(
    self,
    *,
    Name: str,
    ParallelDataConfig: ParallelDataConfigTypeDef,  # (1)
    ClientToken: str,
    Description: str = ...,
    EncryptionKey: EncryptionKeyTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateParallelDataResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef) 
2. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateParallelDataResponseTypeDef](./type_defs.md#createparalleldataresponsetypedef) 


```python
# create_parallel_data method usage example with argument unpacking

kwargs: CreateParallelDataRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ParallelDataConfig": ...,
    "ClientToken": ...,
}

parent.create_parallel_data(**kwargs)
```

1. See [:material-code-braces: CreateParallelDataRequestRequestTypeDef](./type_defs.md#createparalleldatarequestrequesttypedef) 

### delete\_parallel\_data

Deletes a parallel data resource in Amazon Translate.

Type annotations and code completion for `#!python session.create_client("translate").delete_parallel_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/delete_parallel_data.html)

```python
# delete_parallel_data method definition

await def delete_parallel_data(
    self,
    *,
    Name: str,
) -> DeleteParallelDataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteParallelDataResponseTypeDef](./type_defs.md#deleteparalleldataresponsetypedef) 


```python
# delete_parallel_data method usage example with argument unpacking

kwargs: DeleteParallelDataRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_parallel_data(**kwargs)
```

1. See [:material-code-braces: DeleteParallelDataRequestRequestTypeDef](./type_defs.md#deleteparalleldatarequestrequesttypedef) 

### delete\_terminology

A synchronous action that deletes a custom terminology.

Type annotations and code completion for `#!python session.create_client("translate").delete_terminology` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/delete_terminology.html)

```python
# delete_terminology method definition

await def delete_terminology(
    self,
    *,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_terminology method usage example with argument unpacking

kwargs: DeleteTerminologyRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_terminology(**kwargs)
```

1. See [:material-code-braces: DeleteTerminologyRequestRequestTypeDef](./type_defs.md#deleteterminologyrequestrequesttypedef) 

### describe\_text\_translation\_job

Gets the properties associated with an asynchronous batch translation job
including name, ID, status, source and target languages, input/output S3
buckets, and so on.

Type annotations and code completion for `#!python session.create_client("translate").describe_text_translation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/describe_text_translation_job.html)

```python
# describe_text_translation_job method definition

await def describe_text_translation_job(
    self,
    *,
    JobId: str,
) -> DescribeTextTranslationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTextTranslationJobResponseTypeDef](./type_defs.md#describetexttranslationjobresponsetypedef) 


```python
# describe_text_translation_job method usage example with argument unpacking

kwargs: DescribeTextTranslationJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_text_translation_job(**kwargs)
```

1. See [:material-code-braces: DescribeTextTranslationJobRequestRequestTypeDef](./type_defs.md#describetexttranslationjobrequestrequesttypedef) 

### get\_parallel\_data

Provides information about a parallel data resource.

Type annotations and code completion for `#!python session.create_client("translate").get_parallel_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/get_parallel_data.html)

```python
# get_parallel_data method definition

await def get_parallel_data(
    self,
    *,
    Name: str,
) -> GetParallelDataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetParallelDataResponseTypeDef](./type_defs.md#getparalleldataresponsetypedef) 


```python
# get_parallel_data method usage example with argument unpacking

kwargs: GetParallelDataRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_parallel_data(**kwargs)
```

1. See [:material-code-braces: GetParallelDataRequestRequestTypeDef](./type_defs.md#getparalleldatarequestrequesttypedef) 

### get\_terminology

Retrieves a custom terminology.

Type annotations and code completion for `#!python session.create_client("translate").get_terminology` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/get_terminology.html)

```python
# get_terminology method definition

await def get_terminology(
    self,
    *,
    Name: str,
    TerminologyDataFormat: TerminologyDataFormatType = ...,  # (1)
) -> GetTerminologyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TerminologyDataFormatType](./literals.md#terminologydataformattype) 
2. See [:material-code-braces: GetTerminologyResponseTypeDef](./type_defs.md#getterminologyresponsetypedef) 


```python
# get_terminology method usage example with argument unpacking

kwargs: GetTerminologyRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_terminology(**kwargs)
```

1. See [:material-code-braces: GetTerminologyRequestRequestTypeDef](./type_defs.md#getterminologyrequestrequesttypedef) 

### import\_terminology

Creates or updates a custom terminology, depending on whether one already
exists for the given terminology name.

Type annotations and code completion for `#!python session.create_client("translate").import_terminology` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/import_terminology.html)

```python
# import_terminology method definition

await def import_terminology(
    self,
    *,
    Name: str,
    MergeStrategy: MergeStrategyType,  # (1)
    TerminologyData: TerminologyDataTypeDef,  # (2)
    Description: str = ...,
    EncryptionKey: EncryptionKeyTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> ImportTerminologyResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
2. See [:material-code-braces: TerminologyDataTypeDef](./type_defs.md#terminologydatatypedef) 
3. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ImportTerminologyResponseTypeDef](./type_defs.md#importterminologyresponsetypedef) 


```python
# import_terminology method usage example with argument unpacking

kwargs: ImportTerminologyRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "MergeStrategy": ...,
    "TerminologyData": ...,
}

parent.import_terminology(**kwargs)
```

1. See [:material-code-braces: ImportTerminologyRequestRequestTypeDef](./type_defs.md#importterminologyrequestrequesttypedef) 

### list\_languages

Provides a list of languages (RFC-5646 codes and names) that Amazon Translate
supports.

Type annotations and code completion for `#!python session.create_client("translate").list_languages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/list_languages.html)

```python
# list_languages method definition

await def list_languages(
    self,
    *,
    DisplayLanguageCode: DisplayLanguageCodeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLanguagesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DisplayLanguageCodeType](./literals.md#displaylanguagecodetype) 
2. See [:material-code-braces: ListLanguagesResponseTypeDef](./type_defs.md#listlanguagesresponsetypedef) 


```python
# list_languages method usage example with argument unpacking

kwargs: ListLanguagesRequestRequestTypeDef = {  # (1)
    "DisplayLanguageCode": ...,
}

parent.list_languages(**kwargs)
```

1. See [:material-code-braces: ListLanguagesRequestRequestTypeDef](./type_defs.md#listlanguagesrequestrequesttypedef) 

### list\_parallel\_data

Provides a list of your parallel data resources in Amazon Translate.

Type annotations and code completion for `#!python session.create_client("translate").list_parallel_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/list_parallel_data.html)

```python
# list_parallel_data method definition

await def list_parallel_data(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListParallelDataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListParallelDataResponseTypeDef](./type_defs.md#listparalleldataresponsetypedef) 


```python
# list_parallel_data method usage example with argument unpacking

kwargs: ListParallelDataRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_parallel_data(**kwargs)
```

1. See [:material-code-braces: ListParallelDataRequestRequestTypeDef](./type_defs.md#listparalleldatarequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags associated with a given Amazon Translate resource.

Type annotations and code completion for `#!python session.create_client("translate").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/list_tags_for_resource.html)

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

### list\_terminologies

Provides a list of custom terminologies associated with your account.

Type annotations and code completion for `#!python session.create_client("translate").list_terminologies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/list_terminologies.html)

```python
# list_terminologies method definition

await def list_terminologies(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTerminologiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef) 


```python
# list_terminologies method usage example with argument unpacking

kwargs: ListTerminologiesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_terminologies(**kwargs)
```

1. See [:material-code-braces: ListTerminologiesRequestRequestTypeDef](./type_defs.md#listterminologiesrequestrequesttypedef) 

### list\_text\_translation\_jobs

Gets a list of the batch translation jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("translate").list_text_translation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/list_text_translation_jobs.html)

```python
# list_text_translation_jobs method definition

await def list_text_translation_jobs(
    self,
    *,
    Filter: TextTranslationJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTextTranslationJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TextTranslationJobFilterTypeDef](./type_defs.md#texttranslationjobfiltertypedef) 
2. See [:material-code-braces: ListTextTranslationJobsResponseTypeDef](./type_defs.md#listtexttranslationjobsresponsetypedef) 


```python
# list_text_translation_jobs method usage example with argument unpacking

kwargs: ListTextTranslationJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_text_translation_jobs(**kwargs)
```

1. See [:material-code-braces: ListTextTranslationJobsRequestRequestTypeDef](./type_defs.md#listtexttranslationjobsrequestrequesttypedef) 

### start\_text\_translation\_job

Starts an asynchronous batch translation job.

Type annotations and code completion for `#!python session.create_client("translate").start_text_translation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/start_text_translation_job.html)

```python
# start_text_translation_job method definition

await def start_text_translation_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    SourceLanguageCode: str,
    TargetLanguageCodes: Sequence[str],
    ClientToken: str,
    JobName: str = ...,
    TerminologyNames: Sequence[str] = ...,
    ParallelDataNames: Sequence[str] = ...,
    Settings: TranslationSettingsTypeDef = ...,  # (3)
) -> StartTextTranslationJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
4. See [:material-code-braces: StartTextTranslationJobResponseTypeDef](./type_defs.md#starttexttranslationjobresponsetypedef) 


```python
# start_text_translation_job method usage example with argument unpacking

kwargs: StartTextTranslationJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
    "SourceLanguageCode": ...,
    "TargetLanguageCodes": ...,
    "ClientToken": ...,
}

parent.start_text_translation_job(**kwargs)
```

1. See [:material-code-braces: StartTextTranslationJobRequestRequestTypeDef](./type_defs.md#starttexttranslationjobrequestrequesttypedef) 

### stop\_text\_translation\_job

Stops an asynchronous batch translation job that is in progress.

Type annotations and code completion for `#!python session.create_client("translate").stop_text_translation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/stop_text_translation_job.html)

```python
# stop_text_translation_job method definition

await def stop_text_translation_job(
    self,
    *,
    JobId: str,
) -> StopTextTranslationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopTextTranslationJobResponseTypeDef](./type_defs.md#stoptexttranslationjobresponsetypedef) 


```python
# stop_text_translation_job method usage example with argument unpacking

kwargs: StopTextTranslationJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_text_translation_job(**kwargs)
```

1. See [:material-code-braces: StopTextTranslationJobRequestRequestTypeDef](./type_defs.md#stoptexttranslationjobrequestrequesttypedef) 

### tag\_resource

Associates a specific tag with a resource.

Type annotations and code completion for `#!python session.create_client("translate").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/tag_resource.html)

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

### translate\_document

Translates the input document from the source language to the target language.

Type annotations and code completion for `#!python session.create_client("translate").translate_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/translate_document.html)

```python
# translate_document method definition

await def translate_document(
    self,
    *,
    Document: DocumentTypeDef,  # (1)
    SourceLanguageCode: str,
    TargetLanguageCode: str,
    TerminologyNames: Sequence[str] = ...,
    Settings: TranslationSettingsTypeDef = ...,  # (2)
) -> TranslateDocumentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
3. See [:material-code-braces: TranslateDocumentResponseTypeDef](./type_defs.md#translatedocumentresponsetypedef) 


```python
# translate_document method usage example with argument unpacking

kwargs: TranslateDocumentRequestRequestTypeDef = {  # (1)
    "Document": ...,
    "SourceLanguageCode": ...,
    "TargetLanguageCode": ...,
}

parent.translate_document(**kwargs)
```

1. See [:material-code-braces: TranslateDocumentRequestRequestTypeDef](./type_defs.md#translatedocumentrequestrequesttypedef) 

### translate\_text

Translates input text from the source language to the target language.

Type annotations and code completion for `#!python session.create_client("translate").translate_text` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/translate_text.html)

```python
# translate_text method definition

await def translate_text(
    self,
    *,
    Text: str,
    SourceLanguageCode: str,
    TargetLanguageCode: str,
    TerminologyNames: Sequence[str] = ...,
    Settings: TranslationSettingsTypeDef = ...,  # (1)
) -> TranslateTextResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
2. See [:material-code-braces: TranslateTextResponseTypeDef](./type_defs.md#translatetextresponsetypedef) 


```python
# translate_text method usage example with argument unpacking

kwargs: TranslateTextRequestRequestTypeDef = {  # (1)
    "Text": ...,
    "SourceLanguageCode": ...,
    "TargetLanguageCode": ...,
}

parent.translate_text(**kwargs)
```

1. See [:material-code-braces: TranslateTextRequestRequestTypeDef](./type_defs.md#translatetextrequestrequesttypedef) 

### untag\_resource

Removes a specific tag associated with an Amazon Translate resource.

Type annotations and code completion for `#!python session.create_client("translate").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/untag_resource.html)

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

### update\_parallel\_data

Updates a previously created parallel data resource by importing a new input
file from Amazon S3.

Type annotations and code completion for `#!python session.create_client("translate").update_parallel_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/client/update_parallel_data.html)

```python
# update_parallel_data method definition

await def update_parallel_data(
    self,
    *,
    Name: str,
    ParallelDataConfig: ParallelDataConfigTypeDef,  # (1)
    ClientToken: str,
    Description: str = ...,
) -> UpdateParallelDataResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef) 
2. See [:material-code-braces: UpdateParallelDataResponseTypeDef](./type_defs.md#updateparalleldataresponsetypedef) 


```python
# update_parallel_data method usage example with argument unpacking

kwargs: UpdateParallelDataRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ParallelDataConfig": ...,
    "ClientToken": ...,
}

parent.update_parallel_data(**kwargs)
```

1. See [:material-code-braces: UpdateParallelDataRequestRequestTypeDef](./type_defs.md#updateparalleldatarequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("translate").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "TranslateClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("translate").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("translate").get_paginator` method with overloads.

- `client.get_paginator("list_terminologies")` -> [ListTerminologiesPaginator](./paginators.md#listterminologiespaginator)




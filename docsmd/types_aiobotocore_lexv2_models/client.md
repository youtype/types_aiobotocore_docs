# LexModelsV2Client

> [Index](../README.md) > [LexModelsV2](./README.md) > LexModelsV2Client

!!! note ""

    Auto-generated documentation for [LexModelsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
    type annotations stubs module [types-aiobotocore-lexv2-models](https://pypi.org/project/types-aiobotocore-lexv2-models/).

## LexModelsV2Client

Type annotations and code completion for `#!python session.create_client("lexv2-models")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client)

```python
# LexModelsV2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_lexv2_models.client import LexModelsV2Client

session = get_session()
async with session.create_client("lexv2-models") as client:
    client: LexModelsV2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("lexv2-models").exceptions` structure.

```python
# LexModelsV2Client.exceptions usage example

async with session.create_client("lexv2-models") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.PreconditionFailedException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# LexModelsV2Client usage type checking example

from types_aiobotocore_lexv2_models.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### batch\_create\_custom\_vocabulary\_item

Create a batch of custom vocabulary items for a given bot locale's custom
vocabulary.

Type annotations and code completion for `#!python session.create_client("lexv2-models").batch_create_custom_vocabulary_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_create_custom_vocabulary_item)

```python
# batch_create_custom_vocabulary_item method definition

await def batch_create_custom_vocabulary_item(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef],  # (1)
) -> BatchCreateCustomVocabularyItemResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NewCustomVocabularyItemTypeDef](./type_defs.md#newcustomvocabularyitemtypedef) 
2. See [:material-code-braces: BatchCreateCustomVocabularyItemResponseTypeDef](./type_defs.md#batchcreatecustomvocabularyitemresponsetypedef) 


```python
# batch_create_custom_vocabulary_item method usage example with argument unpacking

kwargs: BatchCreateCustomVocabularyItemRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "customVocabularyItemList": ...,
}

parent.batch_create_custom_vocabulary_item(**kwargs)
```

1. See [:material-code-braces: BatchCreateCustomVocabularyItemRequestRequestTypeDef](./type_defs.md#batchcreatecustomvocabularyitemrequestrequesttypedef) 

### batch\_delete\_custom\_vocabulary\_item

Delete a batch of custom vocabulary items for a given bot locale's custom
vocabulary.

Type annotations and code completion for `#!python session.create_client("lexv2-models").batch_delete_custom_vocabulary_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_delete_custom_vocabulary_item)

```python
# batch_delete_custom_vocabulary_item method definition

await def batch_delete_custom_vocabulary_item(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef],  # (1)
) -> BatchDeleteCustomVocabularyItemResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomVocabularyEntryIdTypeDef](./type_defs.md#customvocabularyentryidtypedef) 
2. See [:material-code-braces: BatchDeleteCustomVocabularyItemResponseTypeDef](./type_defs.md#batchdeletecustomvocabularyitemresponsetypedef) 


```python
# batch_delete_custom_vocabulary_item method usage example with argument unpacking

kwargs: BatchDeleteCustomVocabularyItemRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "customVocabularyItemList": ...,
}

parent.batch_delete_custom_vocabulary_item(**kwargs)
```

1. See [:material-code-braces: BatchDeleteCustomVocabularyItemRequestRequestTypeDef](./type_defs.md#batchdeletecustomvocabularyitemrequestrequesttypedef) 

### batch\_update\_custom\_vocabulary\_item

Update a batch of custom vocabulary items for a given bot locale's custom
vocabulary.

Type annotations and code completion for `#!python session.create_client("lexv2-models").batch_update_custom_vocabulary_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_update_custom_vocabulary_item)

```python
# batch_update_custom_vocabulary_item method definition

await def batch_update_custom_vocabulary_item(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef],  # (1)
) -> BatchUpdateCustomVocabularyItemResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomVocabularyItemTypeDef](./type_defs.md#customvocabularyitemtypedef) 
2. See [:material-code-braces: BatchUpdateCustomVocabularyItemResponseTypeDef](./type_defs.md#batchupdatecustomvocabularyitemresponsetypedef) 


```python
# batch_update_custom_vocabulary_item method usage example with argument unpacking

kwargs: BatchUpdateCustomVocabularyItemRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "customVocabularyItemList": ...,
}

parent.batch_update_custom_vocabulary_item(**kwargs)
```

1. See [:material-code-braces: BatchUpdateCustomVocabularyItemRequestRequestTypeDef](./type_defs.md#batchupdatecustomvocabularyitemrequestrequesttypedef) 

### build\_bot\_locale

Builds a bot, its intents, and its slot types into a specific locale.

Type annotations and code completion for `#!python session.create_client("lexv2-models").build_bot_locale` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.build_bot_locale)

```python
# build_bot_locale method definition

await def build_bot_locale(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
) -> BuildBotLocaleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BuildBotLocaleResponseTypeDef](./type_defs.md#buildbotlocaleresponsetypedef) 


```python
# build_bot_locale method usage example with argument unpacking

kwargs: BuildBotLocaleRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.build_bot_locale(**kwargs)
```

1. See [:material-code-braces: BuildBotLocaleRequestRequestTypeDef](./type_defs.md#buildbotlocalerequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("lexv2-models").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("lexv2-models").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_bot

Creates an Amazon Lex conversational bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)

```python
# create_bot method definition

await def create_bot(
    self,
    *,
    botName: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    description: str = ...,
    botTags: Mapping[str, str] = ...,
    testBotAliasTags: Mapping[str, str] = ...,
    botType: BotTypeType = ...,  # (2)
    botMembers: Sequence[BotMemberTypeDef] = ...,  # (3)
) -> CreateBotResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
3. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
4. See [:material-code-braces: CreateBotResponseTypeDef](./type_defs.md#createbotresponsetypedef) 


```python
# create_bot method usage example with argument unpacking

kwargs: CreateBotRequestRequestTypeDef = {  # (1)
    "botName": ...,
    "roleArn": ...,
    "dataPrivacy": ...,
    "idleSessionTTLInSeconds": ...,
}

parent.create_bot(**kwargs)
```

1. See [:material-code-braces: CreateBotRequestRequestTypeDef](./type_defs.md#createbotrequestrequesttypedef) 

### create\_bot\_alias

Creates an alias for the specified version of a bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_bot_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)

```python
# create_bot_alias method definition

await def create_bot_alias(
    self,
    *,
    botAliasName: str,
    botId: str,
    description: str = ...,
    botVersion: str = ...,
    botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,  # (1)
    conversationLogSettings: ConversationLogSettingsTypeDef = ...,  # (2)
    sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,  # (3)
    tags: Mapping[str, str] = ...,
) -> CreateBotAliasResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef) 
2. See [:material-code-braces: ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef) 
3. See [:material-code-braces: SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef) 
4. See [:material-code-braces: CreateBotAliasResponseTypeDef](./type_defs.md#createbotaliasresponsetypedef) 


```python
# create_bot_alias method usage example with argument unpacking

kwargs: CreateBotAliasRequestRequestTypeDef = {  # (1)
    "botAliasName": ...,
    "botId": ...,
}

parent.create_bot_alias(**kwargs)
```

1. See [:material-code-braces: CreateBotAliasRequestRequestTypeDef](./type_defs.md#createbotaliasrequestrequesttypedef) 

### create\_bot\_locale

Creates a locale in the bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_bot_locale` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_locale)

```python
# create_bot_locale method definition

await def create_bot_locale(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    nluIntentConfidenceThreshold: float,
    description: str = ...,
    voiceSettings: VoiceSettingsTypeDef = ...,  # (1)
    generativeAISettings: GenerativeAISettingsTypeDef = ...,  # (2)
) -> CreateBotLocaleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
2. See [:material-code-braces: GenerativeAISettingsTypeDef](./type_defs.md#generativeaisettingstypedef) 
3. See [:material-code-braces: CreateBotLocaleResponseTypeDef](./type_defs.md#createbotlocaleresponsetypedef) 


```python
# create_bot_locale method usage example with argument unpacking

kwargs: CreateBotLocaleRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "nluIntentConfidenceThreshold": ...,
}

parent.create_bot_locale(**kwargs)
```

1. See [:material-code-braces: CreateBotLocaleRequestRequestTypeDef](./type_defs.md#createbotlocalerequestrequesttypedef) 

### create\_bot\_replica

Action to create a replication of the source bot in the secondary region.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_bot_replica` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_replica)

```python
# create_bot_replica method definition

await def create_bot_replica(
    self,
    *,
    botId: str,
    replicaRegion: str,
) -> CreateBotReplicaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateBotReplicaResponseTypeDef](./type_defs.md#createbotreplicaresponsetypedef) 


```python
# create_bot_replica method usage example with argument unpacking

kwargs: CreateBotReplicaRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "replicaRegion": ...,
}

parent.create_bot_replica(**kwargs)
```

1. See [:material-code-braces: CreateBotReplicaRequestRequestTypeDef](./type_defs.md#createbotreplicarequestrequesttypedef) 

### create\_bot\_version

Creates an immutable version of the bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_bot_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_version)

```python
# create_bot_version method definition

await def create_bot_version(
    self,
    *,
    botId: str,
    botVersionLocaleSpecification: Mapping[str, BotVersionLocaleDetailsTypeDef],  # (1)
    description: str = ...,
) -> CreateBotVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BotVersionLocaleDetailsTypeDef](./type_defs.md#botversionlocaledetailstypedef) 
2. See [:material-code-braces: CreateBotVersionResponseTypeDef](./type_defs.md#createbotversionresponsetypedef) 


```python
# create_bot_version method usage example with argument unpacking

kwargs: CreateBotVersionRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersionLocaleSpecification": ...,
}

parent.create_bot_version(**kwargs)
```

1. See [:material-code-braces: CreateBotVersionRequestRequestTypeDef](./type_defs.md#createbotversionrequestrequesttypedef) 

### create\_export

Creates a zip archive containing the contents of a bot or a bot locale.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_export)

```python
# create_export method definition

await def create_export(
    self,
    *,
    resourceSpecification: ExportResourceSpecificationTypeDef,  # (1)
    fileFormat: ImportExportFileFormatType,  # (2)
    filePassword: str = ...,
) -> CreateExportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExportResourceSpecificationTypeDef](./type_defs.md#exportresourcespecificationtypedef) 
2. See [:material-code-brackets: ImportExportFileFormatType](./literals.md#importexportfileformattype) 
3. See [:material-code-braces: CreateExportResponseTypeDef](./type_defs.md#createexportresponsetypedef) 


```python
# create_export method usage example with argument unpacking

kwargs: CreateExportRequestRequestTypeDef = {  # (1)
    "resourceSpecification": ...,
    "fileFormat": ...,
}

parent.create_export(**kwargs)
```

1. See [:material-code-braces: CreateExportRequestRequestTypeDef](./type_defs.md#createexportrequestrequesttypedef) 

### create\_intent

Creates an intent.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_intent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)

```python
# create_intent method definition

await def create_intent(
    self,
    *,
    intentName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: str = ...,
    parentIntentSignature: str = ...,
    sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,  # (1)
    dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,  # (2)
    fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,  # (3)
    intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,  # (4)
    intentClosingSetting: IntentClosingSettingTypeDef = ...,  # (5)
    inputContexts: Sequence[InputContextTypeDef] = ...,  # (6)
    outputContexts: Sequence[OutputContextTypeDef] = ...,  # (7)
    kendraConfiguration: KendraConfigurationTypeDef = ...,  # (8)
    initialResponseSetting: InitialResponseSettingTypeDef = ...,  # (9)
    qnAIntentConfiguration: QnAIntentConfigurationTypeDef = ...,  # (10)
) -> CreateIntentResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
2. See [:material-code-braces: DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef) 
3. See [:material-code-braces: FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef) 
4. See [:material-code-braces: IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef) 
5. See [:material-code-braces: IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef) 
6. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
7. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
8. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
9. See [:material-code-braces: InitialResponseSettingTypeDef](./type_defs.md#initialresponsesettingtypedef) 
10. See [:material-code-braces: QnAIntentConfigurationTypeDef](./type_defs.md#qnaintentconfigurationtypedef) 
11. See [:material-code-braces: CreateIntentResponseTypeDef](./type_defs.md#createintentresponsetypedef) 


```python
# create_intent method usage example with argument unpacking

kwargs: CreateIntentRequestRequestTypeDef = {  # (1)
    "intentName": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.create_intent(**kwargs)
```

1. See [:material-code-braces: CreateIntentRequestRequestTypeDef](./type_defs.md#createintentrequestrequesttypedef) 

### create\_resource\_policy

Creates a new resource policy with the specified policy statements.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy)

```python
# create_resource_policy method definition

await def create_resource_policy(
    self,
    *,
    resourceArn: str,
    policy: str,
) -> CreateResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateResourcePolicyResponseTypeDef](./type_defs.md#createresourcepolicyresponsetypedef) 


```python
# create_resource_policy method usage example with argument unpacking

kwargs: CreateResourcePolicyRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "policy": ...,
}

parent.create_resource_policy(**kwargs)
```

1. See [:material-code-braces: CreateResourcePolicyRequestRequestTypeDef](./type_defs.md#createresourcepolicyrequestrequesttypedef) 

### create\_resource\_policy\_statement

Adds a new resource policy statement to a bot or bot alias.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_resource_policy_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)

```python
# create_resource_policy_statement method definition

await def create_resource_policy_statement(
    self,
    *,
    resourceArn: str,
    statementId: str,
    effect: EffectType,  # (1)
    principal: Sequence[PrincipalTypeDef],  # (2)
    action: Sequence[str],
    condition: Mapping[str, Mapping[str, str]] = ...,
    expectedRevisionId: str = ...,
) -> CreateResourcePolicyStatementResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EffectType](./literals.md#effecttype) 
2. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
3. See [:material-code-braces: CreateResourcePolicyStatementResponseTypeDef](./type_defs.md#createresourcepolicystatementresponsetypedef) 


```python
# create_resource_policy_statement method usage example with argument unpacking

kwargs: CreateResourcePolicyStatementRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "statementId": ...,
    "effect": ...,
    "principal": ...,
    "action": ...,
}

parent.create_resource_policy_statement(**kwargs)
```

1. See [:material-code-braces: CreateResourcePolicyStatementRequestRequestTypeDef](./type_defs.md#createresourcepolicystatementrequestrequesttypedef) 

### create\_slot

Creates a slot in an intent.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_slot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)

```python
# create_slot method definition

await def create_slot(
    self,
    *,
    slotName: str,
    valueElicitationSetting: SlotValueElicitationSettingTypeDef,  # (1)
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    description: str = ...,
    slotTypeId: str = ...,
    obfuscationSetting: ObfuscationSettingTypeDef = ...,  # (2)
    multipleValuesSetting: MultipleValuesSettingTypeDef = ...,  # (3)
    subSlotSetting: SubSlotSettingTypeDef = ...,  # (4)
) -> CreateSlotResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef) 
2. See [:material-code-braces: ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef) 
3. See [:material-code-braces: MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef) 
4. See [:material-code-braces: SubSlotSettingTypeDef](./type_defs.md#subslotsettingtypedef) 
5. See [:material-code-braces: CreateSlotResponseTypeDef](./type_defs.md#createslotresponsetypedef) 


```python
# create_slot method usage example with argument unpacking

kwargs: CreateSlotRequestRequestTypeDef = {  # (1)
    "slotName": ...,
    "valueElicitationSetting": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "intentId": ...,
}

parent.create_slot(**kwargs)
```

1. See [:material-code-braces: CreateSlotRequestRequestTypeDef](./type_defs.md#createslotrequestrequesttypedef) 

### create\_slot\_type

Creates a custom slot type To create a custom slot type, specify a name for the
slot type and a set of enumeration values, the values that a slot of this type
can
assume.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_slot_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)

```python
# create_slot_type method definition

await def create_slot_type(
    self,
    *,
    slotTypeName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: str = ...,
    slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,  # (1)
    valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,  # (2)
    parentSlotTypeSignature: str = ...,
    externalSourceSetting: ExternalSourceSettingTypeDef = ...,  # (3)
    compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...,  # (4)
) -> CreateSlotTypeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef) [:material-code-braces: SlotTypeValueOutputTypeDef](./type_defs.md#slottypevalueoutputtypedef) 
2. See [:material-code-braces: SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef) 
3. See [:material-code-braces: ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef) 
4. See [:material-code-braces: CompositeSlotTypeSettingTypeDef](./type_defs.md#compositeslottypesettingtypedef) 
5. See [:material-code-braces: CreateSlotTypeResponseTypeDef](./type_defs.md#createslottyperesponsetypedef) 


```python
# create_slot_type method usage example with argument unpacking

kwargs: CreateSlotTypeRequestRequestTypeDef = {  # (1)
    "slotTypeName": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.create_slot_type(**kwargs)
```

1. See [:material-code-braces: CreateSlotTypeRequestRequestTypeDef](./type_defs.md#createslottyperequestrequesttypedef) 

### create\_test\_set\_discrepancy\_report

Create a report that describes the differences between the bot and the test set.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_test_set_discrepancy_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_test_set_discrepancy_report)

```python
# create_test_set_discrepancy_report method definition

await def create_test_set_discrepancy_report(
    self,
    *,
    testSetId: str,
    target: TestSetDiscrepancyReportResourceTargetTypeDef,  # (1)
) -> CreateTestSetDiscrepancyReportResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TestSetDiscrepancyReportResourceTargetTypeDef](./type_defs.md#testsetdiscrepancyreportresourcetargettypedef) 
2. See [:material-code-braces: CreateTestSetDiscrepancyReportResponseTypeDef](./type_defs.md#createtestsetdiscrepancyreportresponsetypedef) 


```python
# create_test_set_discrepancy_report method usage example with argument unpacking

kwargs: CreateTestSetDiscrepancyReportRequestRequestTypeDef = {  # (1)
    "testSetId": ...,
    "target": ...,
}

parent.create_test_set_discrepancy_report(**kwargs)
```

1. See [:material-code-braces: CreateTestSetDiscrepancyReportRequestRequestTypeDef](./type_defs.md#createtestsetdiscrepancyreportrequestrequesttypedef) 

### create\_upload\_url

Gets a pre-signed S3 write URL that you use to upload the zip archive when
importing a bot or a bot
locale.

Type annotations and code completion for `#!python session.create_client("lexv2-models").create_upload_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_upload_url)

```python
# create_upload_url method definition

await def create_upload_url(
    self,
) -> CreateUploadUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateUploadUrlResponseTypeDef](./type_defs.md#createuploadurlresponsetypedef) 

### delete\_bot

Deletes all versions of a bot, including the `Draft` version.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot)

```python
# delete_bot method definition

await def delete_bot(
    self,
    *,
    botId: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteBotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBotResponseTypeDef](./type_defs.md#deletebotresponsetypedef) 


```python
# delete_bot method usage example with argument unpacking

kwargs: DeleteBotRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.delete_bot(**kwargs)
```

1. See [:material-code-braces: DeleteBotRequestRequestTypeDef](./type_defs.md#deletebotrequestrequesttypedef) 

### delete\_bot\_alias

Deletes the specified bot alias.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_bot_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_alias)

```python
# delete_bot_alias method definition

await def delete_bot_alias(
    self,
    *,
    botAliasId: str,
    botId: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteBotAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBotAliasResponseTypeDef](./type_defs.md#deletebotaliasresponsetypedef) 


```python
# delete_bot_alias method usage example with argument unpacking

kwargs: DeleteBotAliasRequestRequestTypeDef = {  # (1)
    "botAliasId": ...,
    "botId": ...,
}

parent.delete_bot_alias(**kwargs)
```

1. See [:material-code-braces: DeleteBotAliasRequestRequestTypeDef](./type_defs.md#deletebotaliasrequestrequesttypedef) 

### delete\_bot\_locale

Removes a locale from a bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_bot_locale` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_locale)

```python
# delete_bot_locale method definition

await def delete_bot_locale(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
) -> DeleteBotLocaleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBotLocaleResponseTypeDef](./type_defs.md#deletebotlocaleresponsetypedef) 


```python
# delete_bot_locale method usage example with argument unpacking

kwargs: DeleteBotLocaleRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.delete_bot_locale(**kwargs)
```

1. See [:material-code-braces: DeleteBotLocaleRequestRequestTypeDef](./type_defs.md#deletebotlocalerequestrequesttypedef) 

### delete\_bot\_replica

The action to delete the replicated bot in the secondary region.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_bot_replica` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_replica)

```python
# delete_bot_replica method definition

await def delete_bot_replica(
    self,
    *,
    botId: str,
    replicaRegion: str,
) -> DeleteBotReplicaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBotReplicaResponseTypeDef](./type_defs.md#deletebotreplicaresponsetypedef) 


```python
# delete_bot_replica method usage example with argument unpacking

kwargs: DeleteBotReplicaRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "replicaRegion": ...,
}

parent.delete_bot_replica(**kwargs)
```

1. See [:material-code-braces: DeleteBotReplicaRequestRequestTypeDef](./type_defs.md#deletebotreplicarequestrequesttypedef) 

### delete\_bot\_version

Deletes a specific version of a bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_bot_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_version)

```python
# delete_bot_version method definition

await def delete_bot_version(
    self,
    *,
    botId: str,
    botVersion: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteBotVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBotVersionResponseTypeDef](./type_defs.md#deletebotversionresponsetypedef) 


```python
# delete_bot_version method usage example with argument unpacking

kwargs: DeleteBotVersionRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
}

parent.delete_bot_version(**kwargs)
```

1. See [:material-code-braces: DeleteBotVersionRequestRequestTypeDef](./type_defs.md#deletebotversionrequestrequesttypedef) 

### delete\_custom\_vocabulary

Removes a custom vocabulary from the specified locale in the specified bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_custom_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_custom_vocabulary)

```python
# delete_custom_vocabulary method definition

await def delete_custom_vocabulary(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
) -> DeleteCustomVocabularyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCustomVocabularyResponseTypeDef](./type_defs.md#deletecustomvocabularyresponsetypedef) 


```python
# delete_custom_vocabulary method usage example with argument unpacking

kwargs: DeleteCustomVocabularyRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.delete_custom_vocabulary(**kwargs)
```

1. See [:material-code-braces: DeleteCustomVocabularyRequestRequestTypeDef](./type_defs.md#deletecustomvocabularyrequestrequesttypedef) 

### delete\_export

Removes a previous export and the associated files stored in an S3 bucket.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_export)

```python
# delete_export method definition

await def delete_export(
    self,
    *,
    exportId: str,
) -> DeleteExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteExportResponseTypeDef](./type_defs.md#deleteexportresponsetypedef) 


```python
# delete_export method usage example with argument unpacking

kwargs: DeleteExportRequestRequestTypeDef = {  # (1)
    "exportId": ...,
}

parent.delete_export(**kwargs)
```

1. See [:material-code-braces: DeleteExportRequestRequestTypeDef](./type_defs.md#deleteexportrequestrequesttypedef) 

### delete\_import

Removes a previous import and the associated file stored in an S3 bucket.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_import)

```python
# delete_import method definition

await def delete_import(
    self,
    *,
    importId: str,
) -> DeleteImportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteImportResponseTypeDef](./type_defs.md#deleteimportresponsetypedef) 


```python
# delete_import method usage example with argument unpacking

kwargs: DeleteImportRequestRequestTypeDef = {  # (1)
    "importId": ...,
}

parent.delete_import(**kwargs)
```

1. See [:material-code-braces: DeleteImportRequestRequestTypeDef](./type_defs.md#deleteimportrequestrequesttypedef) 

### delete\_intent

Removes the specified intent.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_intent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_intent)

```python
# delete_intent method definition

await def delete_intent(
    self,
    *,
    intentId: str,
    botId: str,
    botVersion: str,
    localeId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_intent method usage example with argument unpacking

kwargs: DeleteIntentRequestRequestTypeDef = {  # (1)
    "intentId": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.delete_intent(**kwargs)
```

1. See [:material-code-braces: DeleteIntentRequestRequestTypeDef](./type_defs.md#deleteintentrequestrequesttypedef) 

### delete\_resource\_policy

Removes an existing policy from a bot or bot alias.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    resourceArn: str,
    expectedRevisionId: str = ...,
) -> DeleteResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResourcePolicyResponseTypeDef](./type_defs.md#deleteresourcepolicyresponsetypedef) 


```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_resource\_policy\_statement

Deletes a policy statement from a resource policy.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_resource_policy_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy_statement)

```python
# delete_resource_policy_statement method definition

await def delete_resource_policy_statement(
    self,
    *,
    resourceArn: str,
    statementId: str,
    expectedRevisionId: str = ...,
) -> DeleteResourcePolicyStatementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResourcePolicyStatementResponseTypeDef](./type_defs.md#deleteresourcepolicystatementresponsetypedef) 


```python
# delete_resource_policy_statement method usage example with argument unpacking

kwargs: DeleteResourcePolicyStatementRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "statementId": ...,
}

parent.delete_resource_policy_statement(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyStatementRequestRequestTypeDef](./type_defs.md#deleteresourcepolicystatementrequestrequesttypedef) 

### delete\_slot

Deletes the specified slot from an intent.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_slot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot)

```python
# delete_slot method definition

await def delete_slot(
    self,
    *,
    slotId: str,
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_slot method usage example with argument unpacking

kwargs: DeleteSlotRequestRequestTypeDef = {  # (1)
    "slotId": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "intentId": ...,
}

parent.delete_slot(**kwargs)
```

1. See [:material-code-braces: DeleteSlotRequestRequestTypeDef](./type_defs.md#deleteslotrequestrequesttypedef) 

### delete\_slot\_type

Deletes a slot type from a bot locale.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_slot_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot_type)

```python
# delete_slot_type method definition

await def delete_slot_type(
    self,
    *,
    slotTypeId: str,
    botId: str,
    botVersion: str,
    localeId: str,
    skipResourceInUseCheck: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_slot_type method usage example with argument unpacking

kwargs: DeleteSlotTypeRequestRequestTypeDef = {  # (1)
    "slotTypeId": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.delete_slot_type(**kwargs)
```

1. See [:material-code-braces: DeleteSlotTypeRequestRequestTypeDef](./type_defs.md#deleteslottyperequestrequesttypedef) 

### delete\_test\_set

The action to delete the selected test set.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_test_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_test_set)

```python
# delete_test_set method definition

await def delete_test_set(
    self,
    *,
    testSetId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_test_set method usage example with argument unpacking

kwargs: DeleteTestSetRequestRequestTypeDef = {  # (1)
    "testSetId": ...,
}

parent.delete_test_set(**kwargs)
```

1. See [:material-code-braces: DeleteTestSetRequestRequestTypeDef](./type_defs.md#deletetestsetrequestrequesttypedef) 

### delete\_utterances

Deletes stored utterances.

Type annotations and code completion for `#!python session.create_client("lexv2-models").delete_utterances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_utterances)

```python
# delete_utterances method definition

await def delete_utterances(
    self,
    *,
    botId: str,
    localeId: str = ...,
    sessionId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_utterances method usage example with argument unpacking

kwargs: DeleteUtterancesRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.delete_utterances(**kwargs)
```

1. See [:material-code-braces: DeleteUtterancesRequestRequestTypeDef](./type_defs.md#deleteutterancesrequestrequesttypedef) 

### describe\_bot

Provides metadata information about a bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot)

```python
# describe_bot method definition

await def describe_bot(
    self,
    *,
    botId: str,
) -> DescribeBotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBotResponseTypeDef](./type_defs.md#describebotresponsetypedef) 


```python
# describe_bot method usage example with argument unpacking

kwargs: DescribeBotRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.describe_bot(**kwargs)
```

1. See [:material-code-braces: DescribeBotRequestRequestTypeDef](./type_defs.md#describebotrequestrequesttypedef) 

### describe\_bot\_alias

Get information about a specific bot alias.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_bot_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_alias)

```python
# describe_bot_alias method definition

await def describe_bot_alias(
    self,
    *,
    botAliasId: str,
    botId: str,
) -> DescribeBotAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBotAliasResponseTypeDef](./type_defs.md#describebotaliasresponsetypedef) 


```python
# describe_bot_alias method usage example with argument unpacking

kwargs: DescribeBotAliasRequestRequestTypeDef = {  # (1)
    "botAliasId": ...,
    "botId": ...,
}

parent.describe_bot_alias(**kwargs)
```

1. See [:material-code-braces: DescribeBotAliasRequestRequestTypeDef](./type_defs.md#describebotaliasrequestrequesttypedef) 

### describe\_bot\_locale

Describes the settings that a bot has for a specific locale.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_bot_locale` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_locale)

```python
# describe_bot_locale method definition

await def describe_bot_locale(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
) -> DescribeBotLocaleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBotLocaleResponseTypeDef](./type_defs.md#describebotlocaleresponsetypedef) 


```python
# describe_bot_locale method usage example with argument unpacking

kwargs: DescribeBotLocaleRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.describe_bot_locale(**kwargs)
```

1. See [:material-code-braces: DescribeBotLocaleRequestRequestTypeDef](./type_defs.md#describebotlocalerequestrequesttypedef) 

### describe\_bot\_recommendation

Provides metadata information about a bot recommendation.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_bot_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_recommendation)

```python
# describe_bot_recommendation method definition

await def describe_bot_recommendation(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
) -> DescribeBotRecommendationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBotRecommendationResponseTypeDef](./type_defs.md#describebotrecommendationresponsetypedef) 


```python
# describe_bot_recommendation method usage example with argument unpacking

kwargs: DescribeBotRecommendationRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "botRecommendationId": ...,
}

parent.describe_bot_recommendation(**kwargs)
```

1. See [:material-code-braces: DescribeBotRecommendationRequestRequestTypeDef](./type_defs.md#describebotrecommendationrequestrequesttypedef) 

### describe\_bot\_replica

Monitors the bot replication status through the UI console.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_bot_replica` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_replica)

```python
# describe_bot_replica method definition

await def describe_bot_replica(
    self,
    *,
    botId: str,
    replicaRegion: str,
) -> DescribeBotReplicaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBotReplicaResponseTypeDef](./type_defs.md#describebotreplicaresponsetypedef) 


```python
# describe_bot_replica method usage example with argument unpacking

kwargs: DescribeBotReplicaRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "replicaRegion": ...,
}

parent.describe_bot_replica(**kwargs)
```

1. See [:material-code-braces: DescribeBotReplicaRequestRequestTypeDef](./type_defs.md#describebotreplicarequestrequesttypedef) 

### describe\_bot\_resource\_generation

Returns information about a request to generate a bot through natural language
description, made through the `StartBotResource`
API.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_bot_resource_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_resource_generation)

```python
# describe_bot_resource_generation method definition

await def describe_bot_resource_generation(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    generationId: str,
) -> DescribeBotResourceGenerationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBotResourceGenerationResponseTypeDef](./type_defs.md#describebotresourcegenerationresponsetypedef) 


```python
# describe_bot_resource_generation method usage example with argument unpacking

kwargs: DescribeBotResourceGenerationRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "generationId": ...,
}

parent.describe_bot_resource_generation(**kwargs)
```

1. See [:material-code-braces: DescribeBotResourceGenerationRequestRequestTypeDef](./type_defs.md#describebotresourcegenerationrequestrequesttypedef) 

### describe\_bot\_version

Provides metadata about a version of a bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_bot_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_version)

```python
# describe_bot_version method definition

await def describe_bot_version(
    self,
    *,
    botId: str,
    botVersion: str,
) -> DescribeBotVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBotVersionResponseTypeDef](./type_defs.md#describebotversionresponsetypedef) 


```python
# describe_bot_version method usage example with argument unpacking

kwargs: DescribeBotVersionRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
}

parent.describe_bot_version(**kwargs)
```

1. See [:material-code-braces: DescribeBotVersionRequestRequestTypeDef](./type_defs.md#describebotversionrequestrequesttypedef) 

### describe\_custom\_vocabulary\_metadata

Provides metadata information about a custom vocabulary.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_custom_vocabulary_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_custom_vocabulary_metadata)

```python
# describe_custom_vocabulary_metadata method definition

await def describe_custom_vocabulary_metadata(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
) -> DescribeCustomVocabularyMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCustomVocabularyMetadataResponseTypeDef](./type_defs.md#describecustomvocabularymetadataresponsetypedef) 


```python
# describe_custom_vocabulary_metadata method usage example with argument unpacking

kwargs: DescribeCustomVocabularyMetadataRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.describe_custom_vocabulary_metadata(**kwargs)
```

1. See [:material-code-braces: DescribeCustomVocabularyMetadataRequestRequestTypeDef](./type_defs.md#describecustomvocabularymetadatarequestrequesttypedef) 

### describe\_export

Gets information about a specific export.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_export)

```python
# describe_export method definition

await def describe_export(
    self,
    *,
    exportId: str,
) -> DescribeExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeExportResponseTypeDef](./type_defs.md#describeexportresponsetypedef) 


```python
# describe_export method usage example with argument unpacking

kwargs: DescribeExportRequestRequestTypeDef = {  # (1)
    "exportId": ...,
}

parent.describe_export(**kwargs)
```

1. See [:material-code-braces: DescribeExportRequestRequestTypeDef](./type_defs.md#describeexportrequestrequesttypedef) 

### describe\_import

Gets information about a specific import.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_import)

```python
# describe_import method definition

await def describe_import(
    self,
    *,
    importId: str,
) -> DescribeImportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeImportResponseTypeDef](./type_defs.md#describeimportresponsetypedef) 


```python
# describe_import method usage example with argument unpacking

kwargs: DescribeImportRequestRequestTypeDef = {  # (1)
    "importId": ...,
}

parent.describe_import(**kwargs)
```

1. See [:material-code-braces: DescribeImportRequestRequestTypeDef](./type_defs.md#describeimportrequestrequesttypedef) 

### describe\_intent

Returns metadata about an intent.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_intent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_intent)

```python
# describe_intent method definition

await def describe_intent(
    self,
    *,
    intentId: str,
    botId: str,
    botVersion: str,
    localeId: str,
) -> DescribeIntentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIntentResponseTypeDef](./type_defs.md#describeintentresponsetypedef) 


```python
# describe_intent method usage example with argument unpacking

kwargs: DescribeIntentRequestRequestTypeDef = {  # (1)
    "intentId": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.describe_intent(**kwargs)
```

1. See [:material-code-braces: DescribeIntentRequestRequestTypeDef](./type_defs.md#describeintentrequestrequesttypedef) 

### describe\_resource\_policy

Gets the resource policy and policy revision for a bot or bot alias.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_resource_policy)

```python
# describe_resource_policy method definition

await def describe_resource_policy(
    self,
    *,
    resourceArn: str,
) -> DescribeResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef) 


```python
# describe_resource_policy method usage example with argument unpacking

kwargs: DescribeResourcePolicyRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.describe_resource_policy(**kwargs)
```

1. See [:material-code-braces: DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef) 

### describe\_slot

Gets metadata information about a slot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_slot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot)

```python
# describe_slot method definition

await def describe_slot(
    self,
    *,
    slotId: str,
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
) -> DescribeSlotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSlotResponseTypeDef](./type_defs.md#describeslotresponsetypedef) 


```python
# describe_slot method usage example with argument unpacking

kwargs: DescribeSlotRequestRequestTypeDef = {  # (1)
    "slotId": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "intentId": ...,
}

parent.describe_slot(**kwargs)
```

1. See [:material-code-braces: DescribeSlotRequestRequestTypeDef](./type_defs.md#describeslotrequestrequesttypedef) 

### describe\_slot\_type

Gets metadata information about a slot type.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_slot_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot_type)

```python
# describe_slot_type method definition

await def describe_slot_type(
    self,
    *,
    slotTypeId: str,
    botId: str,
    botVersion: str,
    localeId: str,
) -> DescribeSlotTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSlotTypeResponseTypeDef](./type_defs.md#describeslottyperesponsetypedef) 


```python
# describe_slot_type method usage example with argument unpacking

kwargs: DescribeSlotTypeRequestRequestTypeDef = {  # (1)
    "slotTypeId": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.describe_slot_type(**kwargs)
```

1. See [:material-code-braces: DescribeSlotTypeRequestRequestTypeDef](./type_defs.md#describeslottyperequestrequesttypedef) 

### describe\_test\_execution

Gets metadata information about the test execution.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_test_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_execution)

```python
# describe_test_execution method definition

await def describe_test_execution(
    self,
    *,
    testExecutionId: str,
) -> DescribeTestExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTestExecutionResponseTypeDef](./type_defs.md#describetestexecutionresponsetypedef) 


```python
# describe_test_execution method usage example with argument unpacking

kwargs: DescribeTestExecutionRequestRequestTypeDef = {  # (1)
    "testExecutionId": ...,
}

parent.describe_test_execution(**kwargs)
```

1. See [:material-code-braces: DescribeTestExecutionRequestRequestTypeDef](./type_defs.md#describetestexecutionrequestrequesttypedef) 

### describe\_test\_set

Gets metadata information about the test set.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_test_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set)

```python
# describe_test_set method definition

await def describe_test_set(
    self,
    *,
    testSetId: str,
) -> DescribeTestSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTestSetResponseTypeDef](./type_defs.md#describetestsetresponsetypedef) 


```python
# describe_test_set method usage example with argument unpacking

kwargs: DescribeTestSetRequestRequestTypeDef = {  # (1)
    "testSetId": ...,
}

parent.describe_test_set(**kwargs)
```

1. See [:material-code-braces: DescribeTestSetRequestRequestTypeDef](./type_defs.md#describetestsetrequestrequesttypedef) 

### describe\_test\_set\_discrepancy\_report

Gets metadata information about the test set discrepancy report.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_test_set_discrepancy_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set_discrepancy_report)

```python
# describe_test_set_discrepancy_report method definition

await def describe_test_set_discrepancy_report(
    self,
    *,
    testSetDiscrepancyReportId: str,
) -> DescribeTestSetDiscrepancyReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTestSetDiscrepancyReportResponseTypeDef](./type_defs.md#describetestsetdiscrepancyreportresponsetypedef) 


```python
# describe_test_set_discrepancy_report method usage example with argument unpacking

kwargs: DescribeTestSetDiscrepancyReportRequestRequestTypeDef = {  # (1)
    "testSetDiscrepancyReportId": ...,
}

parent.describe_test_set_discrepancy_report(**kwargs)
```

1. See [:material-code-braces: DescribeTestSetDiscrepancyReportRequestRequestTypeDef](./type_defs.md#describetestsetdiscrepancyreportrequestrequesttypedef) 

### describe\_test\_set\_generation

Gets metadata information about the test set generation.

Type annotations and code completion for `#!python session.create_client("lexv2-models").describe_test_set_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set_generation)

```python
# describe_test_set_generation method definition

await def describe_test_set_generation(
    self,
    *,
    testSetGenerationId: str,
) -> DescribeTestSetGenerationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTestSetGenerationResponseTypeDef](./type_defs.md#describetestsetgenerationresponsetypedef) 


```python
# describe_test_set_generation method usage example with argument unpacking

kwargs: DescribeTestSetGenerationRequestRequestTypeDef = {  # (1)
    "testSetGenerationId": ...,
}

parent.describe_test_set_generation(**kwargs)
```

1. See [:material-code-braces: DescribeTestSetGenerationRequestRequestTypeDef](./type_defs.md#describetestsetgenerationrequestrequesttypedef) 

### generate\_bot\_element

Generates sample utterances for an intent.

Type annotations and code completion for `#!python session.create_client("lexv2-models").generate_bot_element` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.generate_bot_element)

```python
# generate_bot_element method definition

await def generate_bot_element(
    self,
    *,
    intentId: str,
    botId: str,
    botVersion: str,
    localeId: str,
) -> GenerateBotElementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GenerateBotElementResponseTypeDef](./type_defs.md#generatebotelementresponsetypedef) 


```python
# generate_bot_element method usage example with argument unpacking

kwargs: GenerateBotElementRequestRequestTypeDef = {  # (1)
    "intentId": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.generate_bot_element(**kwargs)
```

1. See [:material-code-braces: GenerateBotElementRequestRequestTypeDef](./type_defs.md#generatebotelementrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("lexv2-models").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.generate_presigned_url)

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


### get\_test\_execution\_artifacts\_url

The pre-signed Amazon S3 URL to download the test execution result artifacts.

Type annotations and code completion for `#!python session.create_client("lexv2-models").get_test_execution_artifacts_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_test_execution_artifacts_url)

```python
# get_test_execution_artifacts_url method definition

await def get_test_execution_artifacts_url(
    self,
    *,
    testExecutionId: str,
) -> GetTestExecutionArtifactsUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTestExecutionArtifactsUrlResponseTypeDef](./type_defs.md#gettestexecutionartifactsurlresponsetypedef) 


```python
# get_test_execution_artifacts_url method usage example with argument unpacking

kwargs: GetTestExecutionArtifactsUrlRequestRequestTypeDef = {  # (1)
    "testExecutionId": ...,
}

parent.get_test_execution_artifacts_url(**kwargs)
```

1. See [:material-code-braces: GetTestExecutionArtifactsUrlRequestRequestTypeDef](./type_defs.md#gettestexecutionartifactsurlrequestrequesttypedef) 

### list\_aggregated\_utterances

Provides a list of utterances that users have sent to the bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_aggregated_utterances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_aggregated_utterances)

```python
# list_aggregated_utterances method definition

await def list_aggregated_utterances(
    self,
    *,
    botId: str,
    localeId: str,
    aggregationDuration: UtteranceAggregationDurationTypeDef,  # (1)
    botAliasId: str = ...,
    botVersion: str = ...,
    sortBy: AggregatedUtterancesSortByTypeDef = ...,  # (2)
    filters: Sequence[AggregatedUtterancesFilterTypeDef] = ...,  # (3)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAggregatedUtterancesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: UtteranceAggregationDurationTypeDef](./type_defs.md#utteranceaggregationdurationtypedef) 
2. See [:material-code-braces: AggregatedUtterancesSortByTypeDef](./type_defs.md#aggregatedutterancessortbytypedef) 
3. See [:material-code-braces: AggregatedUtterancesFilterTypeDef](./type_defs.md#aggregatedutterancesfiltertypedef) 
4. See [:material-code-braces: ListAggregatedUtterancesResponseTypeDef](./type_defs.md#listaggregatedutterancesresponsetypedef) 


```python
# list_aggregated_utterances method usage example with argument unpacking

kwargs: ListAggregatedUtterancesRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "localeId": ...,
    "aggregationDuration": ...,
}

parent.list_aggregated_utterances(**kwargs)
```

1. See [:material-code-braces: ListAggregatedUtterancesRequestRequestTypeDef](./type_defs.md#listaggregatedutterancesrequestrequesttypedef) 

### list\_bot\_alias\_replicas

The action to list the replicated bots created from the source bot alias.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_alias_replicas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_alias_replicas)

```python
# list_bot_alias_replicas method definition

await def list_bot_alias_replicas(
    self,
    *,
    botId: str,
    replicaRegion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBotAliasReplicasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBotAliasReplicasResponseTypeDef](./type_defs.md#listbotaliasreplicasresponsetypedef) 


```python
# list_bot_alias_replicas method usage example with argument unpacking

kwargs: ListBotAliasReplicasRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "replicaRegion": ...,
}

parent.list_bot_alias_replicas(**kwargs)
```

1. See [:material-code-braces: ListBotAliasReplicasRequestRequestTypeDef](./type_defs.md#listbotaliasreplicasrequestrequesttypedef) 

### list\_bot\_aliases

Gets a list of aliases for the specified bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_aliases)

```python
# list_bot_aliases method definition

await def list_bot_aliases(
    self,
    *,
    botId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBotAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBotAliasesResponseTypeDef](./type_defs.md#listbotaliasesresponsetypedef) 


```python
# list_bot_aliases method usage example with argument unpacking

kwargs: ListBotAliasesRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.list_bot_aliases(**kwargs)
```

1. See [:material-code-braces: ListBotAliasesRequestRequestTypeDef](./type_defs.md#listbotaliasesrequestrequesttypedef) 

### list\_bot\_locales

Gets a list of locales for the specified bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_locales` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_locales)

```python
# list_bot_locales method definition

await def list_bot_locales(
    self,
    *,
    botId: str,
    botVersion: str,
    sortBy: BotLocaleSortByTypeDef = ...,  # (1)
    filters: Sequence[BotLocaleFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBotLocalesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BotLocaleSortByTypeDef](./type_defs.md#botlocalesortbytypedef) 
2. See [:material-code-braces: BotLocaleFilterTypeDef](./type_defs.md#botlocalefiltertypedef) 
3. See [:material-code-braces: ListBotLocalesResponseTypeDef](./type_defs.md#listbotlocalesresponsetypedef) 


```python
# list_bot_locales method usage example with argument unpacking

kwargs: ListBotLocalesRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
}

parent.list_bot_locales(**kwargs)
```

1. See [:material-code-braces: ListBotLocalesRequestRequestTypeDef](./type_defs.md#listbotlocalesrequestrequesttypedef) 

### list\_bot\_recommendations

Get a list of bot recommendations that meet the specified criteria.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_recommendations)

```python
# list_bot_recommendations method definition

await def list_bot_recommendations(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBotRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBotRecommendationsResponseTypeDef](./type_defs.md#listbotrecommendationsresponsetypedef) 


```python
# list_bot_recommendations method usage example with argument unpacking

kwargs: ListBotRecommendationsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.list_bot_recommendations(**kwargs)
```

1. See [:material-code-braces: ListBotRecommendationsRequestRequestTypeDef](./type_defs.md#listbotrecommendationsrequestrequesttypedef) 

### list\_bot\_replicas

The action to list the replicated bots.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_replicas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_replicas)

```python
# list_bot_replicas method definition

await def list_bot_replicas(
    self,
    *,
    botId: str,
) -> ListBotReplicasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBotReplicasResponseTypeDef](./type_defs.md#listbotreplicasresponsetypedef) 


```python
# list_bot_replicas method usage example with argument unpacking

kwargs: ListBotReplicasRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.list_bot_replicas(**kwargs)
```

1. See [:material-code-braces: ListBotReplicasRequestRequestTypeDef](./type_defs.md#listbotreplicasrequestrequesttypedef) 

### list\_bot\_resource\_generations

Lists the generation requests made for a bot locale.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_resource_generations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_resource_generations)

```python
# list_bot_resource_generations method definition

await def list_bot_resource_generations(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    sortBy: GenerationSortByTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBotResourceGenerationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GenerationSortByTypeDef](./type_defs.md#generationsortbytypedef) 
2. See [:material-code-braces: ListBotResourceGenerationsResponseTypeDef](./type_defs.md#listbotresourcegenerationsresponsetypedef) 


```python
# list_bot_resource_generations method usage example with argument unpacking

kwargs: ListBotResourceGenerationsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.list_bot_resource_generations(**kwargs)
```

1. See [:material-code-braces: ListBotResourceGenerationsRequestRequestTypeDef](./type_defs.md#listbotresourcegenerationsrequestrequesttypedef) 

### list\_bot\_version\_replicas

Contains information about all the versions replication statuses applicable for
Global
Resiliency.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_version_replicas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_version_replicas)

```python
# list_bot_version_replicas method definition

await def list_bot_version_replicas(
    self,
    *,
    botId: str,
    replicaRegion: str,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: BotVersionReplicaSortByTypeDef = ...,  # (1)
) -> ListBotVersionReplicasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BotVersionReplicaSortByTypeDef](./type_defs.md#botversionreplicasortbytypedef) 
2. See [:material-code-braces: ListBotVersionReplicasResponseTypeDef](./type_defs.md#listbotversionreplicasresponsetypedef) 


```python
# list_bot_version_replicas method usage example with argument unpacking

kwargs: ListBotVersionReplicasRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "replicaRegion": ...,
}

parent.list_bot_version_replicas(**kwargs)
```

1. See [:material-code-braces: ListBotVersionReplicasRequestRequestTypeDef](./type_defs.md#listbotversionreplicasrequestrequesttypedef) 

### list\_bot\_versions

Gets information about all of the versions of a bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bot_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_versions)

```python
# list_bot_versions method definition

await def list_bot_versions(
    self,
    *,
    botId: str,
    sortBy: BotVersionSortByTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBotVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BotVersionSortByTypeDef](./type_defs.md#botversionsortbytypedef) 
2. See [:material-code-braces: ListBotVersionsResponseTypeDef](./type_defs.md#listbotversionsresponsetypedef) 


```python
# list_bot_versions method usage example with argument unpacking

kwargs: ListBotVersionsRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.list_bot_versions(**kwargs)
```

1. See [:material-code-braces: ListBotVersionsRequestRequestTypeDef](./type_defs.md#listbotversionsrequestrequesttypedef) 

### list\_bots

Gets a list of available bots.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_bots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bots)

```python
# list_bots method definition

await def list_bots(
    self,
    *,
    sortBy: BotSortByTypeDef = ...,  # (1)
    filters: Sequence[BotFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBotsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BotSortByTypeDef](./type_defs.md#botsortbytypedef) 
2. See [:material-code-braces: BotFilterTypeDef](./type_defs.md#botfiltertypedef) 
3. See [:material-code-braces: ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef) 


```python
# list_bots method usage example with argument unpacking

kwargs: ListBotsRequestRequestTypeDef = {  # (1)
    "sortBy": ...,
}

parent.list_bots(**kwargs)
```

1. See [:material-code-braces: ListBotsRequestRequestTypeDef](./type_defs.md#listbotsrequestrequesttypedef) 

### list\_built\_in\_intents

Gets a list of built-in intents provided by Amazon Lex that you can use in your
bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_built_in_intents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_intents)

```python
# list_built_in_intents method definition

await def list_built_in_intents(
    self,
    *,
    localeId: str,
    sortBy: BuiltInIntentSortByTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBuiltInIntentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BuiltInIntentSortByTypeDef](./type_defs.md#builtinintentsortbytypedef) 
2. See [:material-code-braces: ListBuiltInIntentsResponseTypeDef](./type_defs.md#listbuiltinintentsresponsetypedef) 


```python
# list_built_in_intents method usage example with argument unpacking

kwargs: ListBuiltInIntentsRequestRequestTypeDef = {  # (1)
    "localeId": ...,
}

parent.list_built_in_intents(**kwargs)
```

1. See [:material-code-braces: ListBuiltInIntentsRequestRequestTypeDef](./type_defs.md#listbuiltinintentsrequestrequesttypedef) 

### list\_built\_in\_slot\_types

Gets a list of built-in slot types that meet the specified criteria.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_built_in_slot_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_slot_types)

```python
# list_built_in_slot_types method definition

await def list_built_in_slot_types(
    self,
    *,
    localeId: str,
    sortBy: BuiltInSlotTypeSortByTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBuiltInSlotTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BuiltInSlotTypeSortByTypeDef](./type_defs.md#builtinslottypesortbytypedef) 
2. See [:material-code-braces: ListBuiltInSlotTypesResponseTypeDef](./type_defs.md#listbuiltinslottypesresponsetypedef) 


```python
# list_built_in_slot_types method usage example with argument unpacking

kwargs: ListBuiltInSlotTypesRequestRequestTypeDef = {  # (1)
    "localeId": ...,
}

parent.list_built_in_slot_types(**kwargs)
```

1. See [:material-code-braces: ListBuiltInSlotTypesRequestRequestTypeDef](./type_defs.md#listbuiltinslottypesrequestrequesttypedef) 

### list\_custom\_vocabulary\_items

Paginated list of custom vocabulary items for a given bot locale's custom
vocabulary.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_custom_vocabulary_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_custom_vocabulary_items)

```python
# list_custom_vocabulary_items method definition

await def list_custom_vocabulary_items(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListCustomVocabularyItemsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomVocabularyItemsResponseTypeDef](./type_defs.md#listcustomvocabularyitemsresponsetypedef) 


```python
# list_custom_vocabulary_items method usage example with argument unpacking

kwargs: ListCustomVocabularyItemsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.list_custom_vocabulary_items(**kwargs)
```

1. See [:material-code-braces: ListCustomVocabularyItemsRequestRequestTypeDef](./type_defs.md#listcustomvocabularyitemsrequestrequesttypedef) 

### list\_exports

Lists the exports for a bot, bot locale, or custom vocabulary.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_exports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_exports)

```python
# list_exports method definition

await def list_exports(
    self,
    *,
    botId: str = ...,
    botVersion: str = ...,
    sortBy: ExportSortByTypeDef = ...,  # (1)
    filters: Sequence[ExportFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    localeId: str = ...,
) -> ListExportsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExportSortByTypeDef](./type_defs.md#exportsortbytypedef) 
2. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
3. See [:material-code-braces: ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef) 


```python
# list_exports method usage example with argument unpacking

kwargs: ListExportsRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.list_exports(**kwargs)
```

1. See [:material-code-braces: ListExportsRequestRequestTypeDef](./type_defs.md#listexportsrequestrequesttypedef) 

### list\_imports

Lists the imports for a bot, bot locale, or custom vocabulary.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_imports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)

```python
# list_imports method definition

await def list_imports(
    self,
    *,
    botId: str = ...,
    botVersion: str = ...,
    sortBy: ImportSortByTypeDef = ...,  # (1)
    filters: Sequence[ImportFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    localeId: str = ...,
) -> ListImportsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ImportSortByTypeDef](./type_defs.md#importsortbytypedef) 
2. See [:material-code-braces: ImportFilterTypeDef](./type_defs.md#importfiltertypedef) 
3. See [:material-code-braces: ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef) 


```python
# list_imports method usage example with argument unpacking

kwargs: ListImportsRequestRequestTypeDef = {  # (1)
    "botId": ...,
}

parent.list_imports(**kwargs)
```

1. See [:material-code-braces: ListImportsRequestRequestTypeDef](./type_defs.md#listimportsrequestrequesttypedef) 

### list\_intent\_metrics

Retrieves summary metrics for the intents in your bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_intent_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_metrics)

```python
# list_intent_metrics method definition

await def list_intent_metrics(
    self,
    *,
    botId: str,
    startDateTime: TimestampTypeDef,
    endDateTime: TimestampTypeDef,
    metrics: Sequence[AnalyticsIntentMetricTypeDef],  # (1)
    binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,  # (2)
    groupBy: Sequence[AnalyticsIntentGroupBySpecificationTypeDef] = ...,  # (3)
    filters: Sequence[AnalyticsIntentFilterTypeDef] = ...,  # (4)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIntentMetricsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AnalyticsIntentMetricTypeDef](./type_defs.md#analyticsintentmetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsIntentGroupBySpecificationTypeDef](./type_defs.md#analyticsintentgroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsIntentFilterTypeDef](./type_defs.md#analyticsintentfiltertypedef) 
5. See [:material-code-braces: ListIntentMetricsResponseTypeDef](./type_defs.md#listintentmetricsresponsetypedef) 


```python
# list_intent_metrics method usage example with argument unpacking

kwargs: ListIntentMetricsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "startDateTime": ...,
    "endDateTime": ...,
    "metrics": ...,
}

parent.list_intent_metrics(**kwargs)
```

1. See [:material-code-braces: ListIntentMetricsRequestRequestTypeDef](./type_defs.md#listintentmetricsrequestrequesttypedef) 

### list\_intent\_paths

Retrieves summary statistics for a path of intents that users take over
sessions with your
bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_intent_paths` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_paths)

```python
# list_intent_paths method definition

await def list_intent_paths(
    self,
    *,
    botId: str,
    startDateTime: TimestampTypeDef,
    endDateTime: TimestampTypeDef,
    intentPath: str,
    filters: Sequence[AnalyticsPathFilterTypeDef] = ...,  # (1)
) -> ListIntentPathsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnalyticsPathFilterTypeDef](./type_defs.md#analyticspathfiltertypedef) 
2. See [:material-code-braces: ListIntentPathsResponseTypeDef](./type_defs.md#listintentpathsresponsetypedef) 


```python
# list_intent_paths method usage example with argument unpacking

kwargs: ListIntentPathsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "startDateTime": ...,
    "endDateTime": ...,
    "intentPath": ...,
}

parent.list_intent_paths(**kwargs)
```

1. See [:material-code-braces: ListIntentPathsRequestRequestTypeDef](./type_defs.md#listintentpathsrequestrequesttypedef) 

### list\_intent\_stage\_metrics

Retrieves summary metrics for the stages within intents in your bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_intent_stage_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)

```python
# list_intent_stage_metrics method definition

await def list_intent_stage_metrics(
    self,
    *,
    botId: str,
    startDateTime: TimestampTypeDef,
    endDateTime: TimestampTypeDef,
    metrics: Sequence[AnalyticsIntentStageMetricTypeDef],  # (1)
    binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,  # (2)
    groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,  # (3)
    filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,  # (4)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIntentStageMetricsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AnalyticsIntentStageMetricTypeDef](./type_defs.md#analyticsintentstagemetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsIntentStageGroupBySpecificationTypeDef](./type_defs.md#analyticsintentstagegroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsIntentStageFilterTypeDef](./type_defs.md#analyticsintentstagefiltertypedef) 
5. See [:material-code-braces: ListIntentStageMetricsResponseTypeDef](./type_defs.md#listintentstagemetricsresponsetypedef) 


```python
# list_intent_stage_metrics method usage example with argument unpacking

kwargs: ListIntentStageMetricsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "startDateTime": ...,
    "endDateTime": ...,
    "metrics": ...,
}

parent.list_intent_stage_metrics(**kwargs)
```

1. See [:material-code-braces: ListIntentStageMetricsRequestRequestTypeDef](./type_defs.md#listintentstagemetricsrequestrequesttypedef) 

### list\_intents

Get a list of intents that meet the specified criteria.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_intents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intents)

```python
# list_intents method definition

await def list_intents(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    sortBy: IntentSortByTypeDef = ...,  # (1)
    filters: Sequence[IntentFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIntentsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IntentSortByTypeDef](./type_defs.md#intentsortbytypedef) 
2. See [:material-code-braces: IntentFilterTypeDef](./type_defs.md#intentfiltertypedef) 
3. See [:material-code-braces: ListIntentsResponseTypeDef](./type_defs.md#listintentsresponsetypedef) 


```python
# list_intents method usage example with argument unpacking

kwargs: ListIntentsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.list_intents(**kwargs)
```

1. See [:material-code-braces: ListIntentsRequestRequestTypeDef](./type_defs.md#listintentsrequestrequesttypedef) 

### list\_recommended\_intents

Gets a list of recommended intents provided by the bot recommendation that you
can use in your
bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_recommended_intents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)

```python
# list_recommended_intents method definition

await def list_recommended_intents(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListRecommendedIntentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRecommendedIntentsResponseTypeDef](./type_defs.md#listrecommendedintentsresponsetypedef) 


```python
# list_recommended_intents method usage example with argument unpacking

kwargs: ListRecommendedIntentsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "botRecommendationId": ...,
}

parent.list_recommended_intents(**kwargs)
```

1. See [:material-code-braces: ListRecommendedIntentsRequestRequestTypeDef](./type_defs.md#listrecommendedintentsrequestrequesttypedef) 

### list\_session\_analytics\_data

Retrieves a list of metadata for individual user sessions with your bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_session_analytics_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_analytics_data)

```python
# list_session_analytics_data method definition

await def list_session_analytics_data(
    self,
    *,
    botId: str,
    startDateTime: TimestampTypeDef,
    endDateTime: TimestampTypeDef,
    sortBy: SessionDataSortByTypeDef = ...,  # (1)
    filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSessionAnalyticsDataResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SessionDataSortByTypeDef](./type_defs.md#sessiondatasortbytypedef) 
2. See [:material-code-braces: AnalyticsSessionFilterTypeDef](./type_defs.md#analyticssessionfiltertypedef) 
3. See [:material-code-braces: ListSessionAnalyticsDataResponseTypeDef](./type_defs.md#listsessionanalyticsdataresponsetypedef) 


```python
# list_session_analytics_data method usage example with argument unpacking

kwargs: ListSessionAnalyticsDataRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "startDateTime": ...,
    "endDateTime": ...,
}

parent.list_session_analytics_data(**kwargs)
```

1. See [:material-code-braces: ListSessionAnalyticsDataRequestRequestTypeDef](./type_defs.md#listsessionanalyticsdatarequestrequesttypedef) 

### list\_session\_metrics

Retrieves summary metrics for the user sessions with your bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_session_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_metrics)

```python
# list_session_metrics method definition

await def list_session_metrics(
    self,
    *,
    botId: str,
    startDateTime: TimestampTypeDef,
    endDateTime: TimestampTypeDef,
    metrics: Sequence[AnalyticsSessionMetricTypeDef],  # (1)
    binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,  # (2)
    groupBy: Sequence[AnalyticsSessionGroupBySpecificationTypeDef] = ...,  # (3)
    filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,  # (4)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSessionMetricsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AnalyticsSessionMetricTypeDef](./type_defs.md#analyticssessionmetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsSessionGroupBySpecificationTypeDef](./type_defs.md#analyticssessiongroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsSessionFilterTypeDef](./type_defs.md#analyticssessionfiltertypedef) 
5. See [:material-code-braces: ListSessionMetricsResponseTypeDef](./type_defs.md#listsessionmetricsresponsetypedef) 


```python
# list_session_metrics method usage example with argument unpacking

kwargs: ListSessionMetricsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "startDateTime": ...,
    "endDateTime": ...,
    "metrics": ...,
}

parent.list_session_metrics(**kwargs)
```

1. See [:material-code-braces: ListSessionMetricsRequestRequestTypeDef](./type_defs.md#listsessionmetricsrequestrequesttypedef) 

### list\_slot\_types

Gets a list of slot types that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_slot_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slot_types)

```python
# list_slot_types method definition

await def list_slot_types(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    sortBy: SlotTypeSortByTypeDef = ...,  # (1)
    filters: Sequence[SlotTypeFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSlotTypesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SlotTypeSortByTypeDef](./type_defs.md#slottypesortbytypedef) 
2. See [:material-code-braces: SlotTypeFilterTypeDef](./type_defs.md#slottypefiltertypedef) 
3. See [:material-code-braces: ListSlotTypesResponseTypeDef](./type_defs.md#listslottypesresponsetypedef) 


```python
# list_slot_types method usage example with argument unpacking

kwargs: ListSlotTypesRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.list_slot_types(**kwargs)
```

1. See [:material-code-braces: ListSlotTypesRequestRequestTypeDef](./type_defs.md#listslottypesrequestrequesttypedef) 

### list\_slots

Gets a list of slots that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_slots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slots)

```python
# list_slots method definition

await def list_slots(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    sortBy: SlotSortByTypeDef = ...,  # (1)
    filters: Sequence[SlotFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSlotsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SlotSortByTypeDef](./type_defs.md#slotsortbytypedef) 
2. See [:material-code-braces: SlotFilterTypeDef](./type_defs.md#slotfiltertypedef) 
3. See [:material-code-braces: ListSlotsResponseTypeDef](./type_defs.md#listslotsresponsetypedef) 


```python
# list_slots method usage example with argument unpacking

kwargs: ListSlotsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "intentId": ...,
}

parent.list_slots(**kwargs)
```

1. See [:material-code-braces: ListSlotsRequestRequestTypeDef](./type_defs.md#listslotsrequestrequesttypedef) 

### list\_tags\_for\_resource

Gets a list of tags associated with a resource.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_test\_execution\_result\_items

Gets a list of test execution result items.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_test_execution_result_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_execution_result_items)

```python
# list_test_execution_result_items method definition

await def list_test_execution_result_items(
    self,
    *,
    testExecutionId: str,
    resultFilterBy: TestExecutionResultFilterByTypeDef,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTestExecutionResultItemsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TestExecutionResultFilterByTypeDef](./type_defs.md#testexecutionresultfilterbytypedef) 
2. See [:material-code-braces: ListTestExecutionResultItemsResponseTypeDef](./type_defs.md#listtestexecutionresultitemsresponsetypedef) 


```python
# list_test_execution_result_items method usage example with argument unpacking

kwargs: ListTestExecutionResultItemsRequestRequestTypeDef = {  # (1)
    "testExecutionId": ...,
    "resultFilterBy": ...,
}

parent.list_test_execution_result_items(**kwargs)
```

1. See [:material-code-braces: ListTestExecutionResultItemsRequestRequestTypeDef](./type_defs.md#listtestexecutionresultitemsrequestrequesttypedef) 

### list\_test\_executions

The list of test set executions.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_test_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_executions)

```python
# list_test_executions method definition

await def list_test_executions(
    self,
    *,
    sortBy: TestExecutionSortByTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTestExecutionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TestExecutionSortByTypeDef](./type_defs.md#testexecutionsortbytypedef) 
2. See [:material-code-braces: ListTestExecutionsResponseTypeDef](./type_defs.md#listtestexecutionsresponsetypedef) 


```python
# list_test_executions method usage example with argument unpacking

kwargs: ListTestExecutionsRequestRequestTypeDef = {  # (1)
    "sortBy": ...,
}

parent.list_test_executions(**kwargs)
```

1. See [:material-code-braces: ListTestExecutionsRequestRequestTypeDef](./type_defs.md#listtestexecutionsrequestrequesttypedef) 

### list\_test\_set\_records

The list of test set records.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_test_set_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_set_records)

```python
# list_test_set_records method definition

await def list_test_set_records(
    self,
    *,
    testSetId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTestSetRecordsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTestSetRecordsResponseTypeDef](./type_defs.md#listtestsetrecordsresponsetypedef) 


```python
# list_test_set_records method usage example with argument unpacking

kwargs: ListTestSetRecordsRequestRequestTypeDef = {  # (1)
    "testSetId": ...,
}

parent.list_test_set_records(**kwargs)
```

1. See [:material-code-braces: ListTestSetRecordsRequestRequestTypeDef](./type_defs.md#listtestsetrecordsrequestrequesttypedef) 

### list\_test\_sets

The list of the test sets See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/models.lex.v2-2020-08-07/ListTestSets).

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_test_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_sets)

```python
# list_test_sets method definition

await def list_test_sets(
    self,
    *,
    sortBy: TestSetSortByTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTestSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TestSetSortByTypeDef](./type_defs.md#testsetsortbytypedef) 
2. See [:material-code-braces: ListTestSetsResponseTypeDef](./type_defs.md#listtestsetsresponsetypedef) 


```python
# list_test_sets method usage example with argument unpacking

kwargs: ListTestSetsRequestRequestTypeDef = {  # (1)
    "sortBy": ...,
}

parent.list_test_sets(**kwargs)
```

1. See [:material-code-braces: ListTestSetsRequestRequestTypeDef](./type_defs.md#listtestsetsrequestrequesttypedef) 

### list\_utterance\_analytics\_data

.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_utterance_analytics_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)

```python
# list_utterance_analytics_data method definition

await def list_utterance_analytics_data(
    self,
    *,
    botId: str,
    startDateTime: TimestampTypeDef,
    endDateTime: TimestampTypeDef,
    sortBy: UtteranceDataSortByTypeDef = ...,  # (1)
    filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListUtteranceAnalyticsDataResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UtteranceDataSortByTypeDef](./type_defs.md#utterancedatasortbytypedef) 
2. See [:material-code-braces: AnalyticsUtteranceFilterTypeDef](./type_defs.md#analyticsutterancefiltertypedef) 
3. See [:material-code-braces: ListUtteranceAnalyticsDataResponseTypeDef](./type_defs.md#listutteranceanalyticsdataresponsetypedef) 


```python
# list_utterance_analytics_data method usage example with argument unpacking

kwargs: ListUtteranceAnalyticsDataRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "startDateTime": ...,
    "endDateTime": ...,
}

parent.list_utterance_analytics_data(**kwargs)
```

1. See [:material-code-braces: ListUtteranceAnalyticsDataRequestRequestTypeDef](./type_defs.md#listutteranceanalyticsdatarequestrequesttypedef) 

### list\_utterance\_metrics

.

Type annotations and code completion for `#!python session.create_client("lexv2-models").list_utterance_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)

```python
# list_utterance_metrics method definition

await def list_utterance_metrics(
    self,
    *,
    botId: str,
    startDateTime: TimestampTypeDef,
    endDateTime: TimestampTypeDef,
    metrics: Sequence[AnalyticsUtteranceMetricTypeDef],  # (1)
    binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,  # (2)
    groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,  # (3)
    attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,  # (4)
    filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,  # (5)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListUtteranceMetricsResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: AnalyticsUtteranceMetricTypeDef](./type_defs.md#analyticsutterancemetrictypedef) 
2. See [:material-code-braces: AnalyticsBinBySpecificationTypeDef](./type_defs.md#analyticsbinbyspecificationtypedef) 
3. See [:material-code-braces: AnalyticsUtteranceGroupBySpecificationTypeDef](./type_defs.md#analyticsutterancegroupbyspecificationtypedef) 
4. See [:material-code-braces: AnalyticsUtteranceAttributeTypeDef](./type_defs.md#analyticsutteranceattributetypedef) 
5. See [:material-code-braces: AnalyticsUtteranceFilterTypeDef](./type_defs.md#analyticsutterancefiltertypedef) 
6. See [:material-code-braces: ListUtteranceMetricsResponseTypeDef](./type_defs.md#listutterancemetricsresponsetypedef) 


```python
# list_utterance_metrics method usage example with argument unpacking

kwargs: ListUtteranceMetricsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "startDateTime": ...,
    "endDateTime": ...,
    "metrics": ...,
}

parent.list_utterance_metrics(**kwargs)
```

1. See [:material-code-braces: ListUtteranceMetricsRequestRequestTypeDef](./type_defs.md#listutterancemetricsrequestrequesttypedef) 

### search\_associated\_transcripts

Search for associated transcripts that meet the specified criteria.

Type annotations and code completion for `#!python session.create_client("lexv2-models").search_associated_transcripts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.search_associated_transcripts)

```python
# search_associated_transcripts method definition

await def search_associated_transcripts(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    filters: Sequence[AssociatedTranscriptFilterTypeDef],  # (1)
    searchOrder: SearchOrderType = ...,  # (2)
    maxResults: int = ...,
    nextIndex: int = ...,
) -> SearchAssociatedTranscriptsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AssociatedTranscriptFilterTypeDef](./type_defs.md#associatedtranscriptfiltertypedef) 
2. See [:material-code-brackets: SearchOrderType](./literals.md#searchordertype) 
3. See [:material-code-braces: SearchAssociatedTranscriptsResponseTypeDef](./type_defs.md#searchassociatedtranscriptsresponsetypedef) 


```python
# search_associated_transcripts method usage example with argument unpacking

kwargs: SearchAssociatedTranscriptsRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "botRecommendationId": ...,
    "filters": ...,
}

parent.search_associated_transcripts(**kwargs)
```

1. See [:material-code-braces: SearchAssociatedTranscriptsRequestRequestTypeDef](./type_defs.md#searchassociatedtranscriptsrequestrequesttypedef) 

### start\_bot\_recommendation

Use this to provide your transcript data, and to start the bot recommendation
process.

Type annotations and code completion for `#!python session.create_client("lexv2-models").start_bot_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)

```python
# start_bot_recommendation method definition

await def start_bot_recommendation(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    transcriptSourceSetting: TranscriptSourceSettingTypeDef,  # (1)
    encryptionSetting: EncryptionSettingTypeDef = ...,  # (2)
) -> StartBotRecommendationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TranscriptSourceSettingTypeDef](./type_defs.md#transcriptsourcesettingtypedef) 
2. See [:material-code-braces: EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef) 
3. See [:material-code-braces: StartBotRecommendationResponseTypeDef](./type_defs.md#startbotrecommendationresponsetypedef) 


```python
# start_bot_recommendation method usage example with argument unpacking

kwargs: StartBotRecommendationRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "transcriptSourceSetting": ...,
}

parent.start_bot_recommendation(**kwargs)
```

1. See [:material-code-braces: StartBotRecommendationRequestRequestTypeDef](./type_defs.md#startbotrecommendationrequestrequesttypedef) 

### start\_bot\_resource\_generation

Starts a request for the descriptive bot builder to generate a bot locale
configuration based on the prompt you provide
it.

Type annotations and code completion for `#!python session.create_client("lexv2-models").start_bot_resource_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_resource_generation)

```python
# start_bot_resource_generation method definition

await def start_bot_resource_generation(
    self,
    *,
    generationInputPrompt: str,
    botId: str,
    botVersion: str,
    localeId: str,
) -> StartBotResourceGenerationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartBotResourceGenerationResponseTypeDef](./type_defs.md#startbotresourcegenerationresponsetypedef) 


```python
# start_bot_resource_generation method usage example with argument unpacking

kwargs: StartBotResourceGenerationRequestRequestTypeDef = {  # (1)
    "generationInputPrompt": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.start_bot_resource_generation(**kwargs)
```

1. See [:material-code-braces: StartBotResourceGenerationRequestRequestTypeDef](./type_defs.md#startbotresourcegenerationrequestrequesttypedef) 

### start\_import

Starts importing a bot, bot locale, or custom vocabulary from a zip archive
that you uploaded to an S3
bucket.

Type annotations and code completion for `#!python session.create_client("lexv2-models").start_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_import)

```python
# start_import method definition

await def start_import(
    self,
    *,
    importId: str,
    resourceSpecification: ImportResourceSpecificationTypeDef,  # (1)
    mergeStrategy: MergeStrategyType,  # (2)
    filePassword: str = ...,
) -> StartImportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ImportResourceSpecificationTypeDef](./type_defs.md#importresourcespecificationtypedef) 
2. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
3. See [:material-code-braces: StartImportResponseTypeDef](./type_defs.md#startimportresponsetypedef) 


```python
# start_import method usage example with argument unpacking

kwargs: StartImportRequestRequestTypeDef = {  # (1)
    "importId": ...,
    "resourceSpecification": ...,
    "mergeStrategy": ...,
}

parent.start_import(**kwargs)
```

1. See [:material-code-braces: StartImportRequestRequestTypeDef](./type_defs.md#startimportrequestrequesttypedef) 

### start\_test\_execution

The action to start test set execution.

Type annotations and code completion for `#!python session.create_client("lexv2-models").start_test_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_execution)

```python
# start_test_execution method definition

await def start_test_execution(
    self,
    *,
    testSetId: str,
    target: TestExecutionTargetTypeDef,  # (1)
    apiMode: TestExecutionApiModeType,  # (2)
    testExecutionModality: TestExecutionModalityType = ...,  # (3)
) -> StartTestExecutionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TestExecutionTargetTypeDef](./type_defs.md#testexecutiontargettypedef) 
2. See [:material-code-brackets: TestExecutionApiModeType](./literals.md#testexecutionapimodetype) 
3. See [:material-code-brackets: TestExecutionModalityType](./literals.md#testexecutionmodalitytype) 
4. See [:material-code-braces: StartTestExecutionResponseTypeDef](./type_defs.md#starttestexecutionresponsetypedef) 


```python
# start_test_execution method usage example with argument unpacking

kwargs: StartTestExecutionRequestRequestTypeDef = {  # (1)
    "testSetId": ...,
    "target": ...,
    "apiMode": ...,
}

parent.start_test_execution(**kwargs)
```

1. See [:material-code-braces: StartTestExecutionRequestRequestTypeDef](./type_defs.md#starttestexecutionrequestrequesttypedef) 

### start\_test\_set\_generation

The action to start the generation of test set.

Type annotations and code completion for `#!python session.create_client("lexv2-models").start_test_set_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_set_generation)

```python
# start_test_set_generation method definition

await def start_test_set_generation(
    self,
    *,
    testSetName: str,
    storageLocation: TestSetStorageLocationTypeDef,  # (1)
    generationDataSource: TestSetGenerationDataSourceTypeDef,  # (2)
    roleArn: str,
    description: str = ...,
    testSetTags: Mapping[str, str] = ...,
) -> StartTestSetGenerationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TestSetStorageLocationTypeDef](./type_defs.md#testsetstoragelocationtypedef) 
2. See [:material-code-braces: TestSetGenerationDataSourceTypeDef](./type_defs.md#testsetgenerationdatasourcetypedef) 
3. See [:material-code-braces: StartTestSetGenerationResponseTypeDef](./type_defs.md#starttestsetgenerationresponsetypedef) 


```python
# start_test_set_generation method usage example with argument unpacking

kwargs: StartTestSetGenerationRequestRequestTypeDef = {  # (1)
    "testSetName": ...,
    "storageLocation": ...,
    "generationDataSource": ...,
    "roleArn": ...,
}

parent.start_test_set_generation(**kwargs)
```

1. See [:material-code-braces: StartTestSetGenerationRequestRequestTypeDef](./type_defs.md#starttestsetgenerationrequestrequesttypedef) 

### stop\_bot\_recommendation

Stop an already running Bot Recommendation request.

Type annotations and code completion for `#!python session.create_client("lexv2-models").stop_bot_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.stop_bot_recommendation)

```python
# stop_bot_recommendation method definition

await def stop_bot_recommendation(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
) -> StopBotRecommendationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopBotRecommendationResponseTypeDef](./type_defs.md#stopbotrecommendationresponsetypedef) 


```python
# stop_bot_recommendation method usage example with argument unpacking

kwargs: StopBotRecommendationRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "botRecommendationId": ...,
}

parent.stop_bot_recommendation(**kwargs)
```

1. See [:material-code-braces: StopBotRecommendationRequestRequestTypeDef](./type_defs.md#stopbotrecommendationrequestrequesttypedef) 

### tag\_resource

Adds the specified tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("lexv2-models").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceARN: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a bot, bot alias, or bot channel.

Type annotations and code completion for `#!python session.create_client("lexv2-models").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceARN: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_bot

Updates the configuration of an existing bot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)

```python
# update_bot method definition

await def update_bot(
    self,
    *,
    botId: str,
    botName: str,
    roleArn: str,
    dataPrivacy: DataPrivacyTypeDef,  # (1)
    idleSessionTTLInSeconds: int,
    description: str = ...,
    botType: BotTypeType = ...,  # (2)
    botMembers: Sequence[BotMemberTypeDef] = ...,  # (3)
) -> UpdateBotResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef) 
2. See [:material-code-brackets: BotTypeType](./literals.md#bottypetype) 
3. See [:material-code-braces: BotMemberTypeDef](./type_defs.md#botmembertypedef) 
4. See [:material-code-braces: UpdateBotResponseTypeDef](./type_defs.md#updatebotresponsetypedef) 


```python
# update_bot method usage example with argument unpacking

kwargs: UpdateBotRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botName": ...,
    "roleArn": ...,
    "dataPrivacy": ...,
    "idleSessionTTLInSeconds": ...,
}

parent.update_bot(**kwargs)
```

1. See [:material-code-braces: UpdateBotRequestRequestTypeDef](./type_defs.md#updatebotrequestrequesttypedef) 

### update\_bot\_alias

Updates the configuration of an existing bot alias.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_bot_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)

```python
# update_bot_alias method definition

await def update_bot_alias(
    self,
    *,
    botAliasId: str,
    botAliasName: str,
    botId: str,
    description: str = ...,
    botVersion: str = ...,
    botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,  # (1)
    conversationLogSettings: ConversationLogSettingsTypeDef = ...,  # (2)
    sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,  # (3)
) -> UpdateBotAliasResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef) 
2. See [:material-code-braces: ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef) 
3. See [:material-code-braces: SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef) 
4. See [:material-code-braces: UpdateBotAliasResponseTypeDef](./type_defs.md#updatebotaliasresponsetypedef) 


```python
# update_bot_alias method usage example with argument unpacking

kwargs: UpdateBotAliasRequestRequestTypeDef = {  # (1)
    "botAliasId": ...,
    "botAliasName": ...,
    "botId": ...,
}

parent.update_bot_alias(**kwargs)
```

1. See [:material-code-braces: UpdateBotAliasRequestRequestTypeDef](./type_defs.md#updatebotaliasrequestrequesttypedef) 

### update\_bot\_locale

Updates the settings that a bot has for a specific locale.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_bot_locale` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_locale)

```python
# update_bot_locale method definition

await def update_bot_locale(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    nluIntentConfidenceThreshold: float,
    description: str = ...,
    voiceSettings: VoiceSettingsTypeDef = ...,  # (1)
    generativeAISettings: GenerativeAISettingsTypeDef = ...,  # (2)
) -> UpdateBotLocaleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef) 
2. See [:material-code-braces: GenerativeAISettingsTypeDef](./type_defs.md#generativeaisettingstypedef) 
3. See [:material-code-braces: UpdateBotLocaleResponseTypeDef](./type_defs.md#updatebotlocaleresponsetypedef) 


```python
# update_bot_locale method usage example with argument unpacking

kwargs: UpdateBotLocaleRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "nluIntentConfidenceThreshold": ...,
}

parent.update_bot_locale(**kwargs)
```

1. See [:material-code-braces: UpdateBotLocaleRequestRequestTypeDef](./type_defs.md#updatebotlocalerequestrequesttypedef) 

### update\_bot\_recommendation

Updates an existing bot recommendation request.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_bot_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_recommendation)

```python
# update_bot_recommendation method definition

await def update_bot_recommendation(
    self,
    *,
    botId: str,
    botVersion: str,
    localeId: str,
    botRecommendationId: str,
    encryptionSetting: EncryptionSettingTypeDef,  # (1)
) -> UpdateBotRecommendationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef) 
2. See [:material-code-braces: UpdateBotRecommendationResponseTypeDef](./type_defs.md#updatebotrecommendationresponsetypedef) 


```python
# update_bot_recommendation method usage example with argument unpacking

kwargs: UpdateBotRecommendationRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "botRecommendationId": ...,
    "encryptionSetting": ...,
}

parent.update_bot_recommendation(**kwargs)
```

1. See [:material-code-braces: UpdateBotRecommendationRequestRequestTypeDef](./type_defs.md#updatebotrecommendationrequestrequesttypedef) 

### update\_export

Updates the password used to protect an export zip archive.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_export)

```python
# update_export method definition

await def update_export(
    self,
    *,
    exportId: str,
    filePassword: str = ...,
) -> UpdateExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateExportResponseTypeDef](./type_defs.md#updateexportresponsetypedef) 


```python
# update_export method usage example with argument unpacking

kwargs: UpdateExportRequestRequestTypeDef = {  # (1)
    "exportId": ...,
}

parent.update_export(**kwargs)
```

1. See [:material-code-braces: UpdateExportRequestRequestTypeDef](./type_defs.md#updateexportrequestrequesttypedef) 

### update\_intent

Updates the settings for an intent.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_intent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)

```python
# update_intent method definition

await def update_intent(
    self,
    *,
    intentId: str,
    intentName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: str = ...,
    parentIntentSignature: str = ...,
    sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,  # (1)
    dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,  # (2)
    fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,  # (3)
    slotPriorities: Sequence[SlotPriorityTypeDef] = ...,  # (4)
    intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,  # (5)
    intentClosingSetting: IntentClosingSettingTypeDef = ...,  # (6)
    inputContexts: Sequence[InputContextTypeDef] = ...,  # (7)
    outputContexts: Sequence[OutputContextTypeDef] = ...,  # (8)
    kendraConfiguration: KendraConfigurationTypeDef = ...,  # (9)
    initialResponseSetting: InitialResponseSettingTypeDef = ...,  # (10)
    qnAIntentConfiguration: QnAIntentConfigurationTypeDef = ...,  # (11)
) -> UpdateIntentResponseTypeDef:  # (12)
    ...
```

1. See [:material-code-braces: SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef) 
2. See [:material-code-braces: DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef) 
3. See [:material-code-braces: FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef) 
4. See [:material-code-braces: SlotPriorityTypeDef](./type_defs.md#slotprioritytypedef) 
5. See [:material-code-braces: IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef) 
6. See [:material-code-braces: IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef) 
7. See [:material-code-braces: InputContextTypeDef](./type_defs.md#inputcontexttypedef) 
8. See [:material-code-braces: OutputContextTypeDef](./type_defs.md#outputcontexttypedef) 
9. See [:material-code-braces: KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef) 
10. See [:material-code-braces: InitialResponseSettingTypeDef](./type_defs.md#initialresponsesettingtypedef) 
11. See [:material-code-braces: QnAIntentConfigurationTypeDef](./type_defs.md#qnaintentconfigurationtypedef) 
12. See [:material-code-braces: UpdateIntentResponseTypeDef](./type_defs.md#updateintentresponsetypedef) 


```python
# update_intent method usage example with argument unpacking

kwargs: UpdateIntentRequestRequestTypeDef = {  # (1)
    "intentId": ...,
    "intentName": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.update_intent(**kwargs)
```

1. See [:material-code-braces: UpdateIntentRequestRequestTypeDef](./type_defs.md#updateintentrequestrequesttypedef) 

### update\_resource\_policy

Replaces the existing resource policy for a bot or bot alias with a new one.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_resource_policy)

```python
# update_resource_policy method definition

await def update_resource_policy(
    self,
    *,
    resourceArn: str,
    policy: str,
    expectedRevisionId: str = ...,
) -> UpdateResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateResourcePolicyResponseTypeDef](./type_defs.md#updateresourcepolicyresponsetypedef) 


```python
# update_resource_policy method usage example with argument unpacking

kwargs: UpdateResourcePolicyRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "policy": ...,
}

parent.update_resource_policy(**kwargs)
```

1. See [:material-code-braces: UpdateResourcePolicyRequestRequestTypeDef](./type_defs.md#updateresourcepolicyrequestrequesttypedef) 

### update\_slot

Updates the settings for a slot.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_slot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)

```python
# update_slot method definition

await def update_slot(
    self,
    *,
    slotId: str,
    slotName: str,
    valueElicitationSetting: SlotValueElicitationSettingTypeDef,  # (1)
    botId: str,
    botVersion: str,
    localeId: str,
    intentId: str,
    description: str = ...,
    slotTypeId: str = ...,
    obfuscationSetting: ObfuscationSettingTypeDef = ...,  # (2)
    multipleValuesSetting: MultipleValuesSettingTypeDef = ...,  # (3)
    subSlotSetting: SubSlotSettingTypeDef = ...,  # (4)
) -> UpdateSlotResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef) 
2. See [:material-code-braces: ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef) 
3. See [:material-code-braces: MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef) 
4. See [:material-code-braces: SubSlotSettingTypeDef](./type_defs.md#subslotsettingtypedef) 
5. See [:material-code-braces: UpdateSlotResponseTypeDef](./type_defs.md#updateslotresponsetypedef) 


```python
# update_slot method usage example with argument unpacking

kwargs: UpdateSlotRequestRequestTypeDef = {  # (1)
    "slotId": ...,
    "slotName": ...,
    "valueElicitationSetting": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
    "intentId": ...,
}

parent.update_slot(**kwargs)
```

1. See [:material-code-braces: UpdateSlotRequestRequestTypeDef](./type_defs.md#updateslotrequestrequesttypedef) 

### update\_slot\_type

Updates the configuration of an existing slot type.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_slot_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)

```python
# update_slot_type method definition

await def update_slot_type(
    self,
    *,
    slotTypeId: str,
    slotTypeName: str,
    botId: str,
    botVersion: str,
    localeId: str,
    description: str = ...,
    slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,  # (1)
    valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,  # (2)
    parentSlotTypeSignature: str = ...,
    externalSourceSetting: ExternalSourceSettingTypeDef = ...,  # (3)
    compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...,  # (4)
) -> UpdateSlotTypeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef) 
2. See [:material-code-braces: SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef) 
3. See [:material-code-braces: ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef) 
4. See [:material-code-braces: CompositeSlotTypeSettingTypeDef](./type_defs.md#compositeslottypesettingtypedef) 
5. See [:material-code-braces: UpdateSlotTypeResponseTypeDef](./type_defs.md#updateslottyperesponsetypedef) 


```python
# update_slot_type method usage example with argument unpacking

kwargs: UpdateSlotTypeRequestRequestTypeDef = {  # (1)
    "slotTypeId": ...,
    "slotTypeName": ...,
    "botId": ...,
    "botVersion": ...,
    "localeId": ...,
}

parent.update_slot_type(**kwargs)
```

1. See [:material-code-braces: UpdateSlotTypeRequestRequestTypeDef](./type_defs.md#updateslottyperequestrequesttypedef) 

### update\_test\_set

The action to update the test set.

Type annotations and code completion for `#!python session.create_client("lexv2-models").update_test_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_test_set)

```python
# update_test_set method definition

await def update_test_set(
    self,
    *,
    testSetId: str,
    testSetName: str,
    description: str = ...,
) -> UpdateTestSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTestSetResponseTypeDef](./type_defs.md#updatetestsetresponsetypedef) 


```python
# update_test_set method usage example with argument unpacking

kwargs: UpdateTestSetRequestRequestTypeDef = {  # (1)
    "testSetId": ...,
    "testSetName": ...,
}

parent.update_test_set(**kwargs)
```

1. See [:material-code-braces: UpdateTestSetRequestRequestTypeDef](./type_defs.md#updatetestsetrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("lexv2-models").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "LexModelsV2Client":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("lexv2-models").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.__aexit__)

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






### get_waiter

Type annotations and code completion for `#!python session.create_client("lexv2-models").get_waiter` method with overloads.

- `client.get_waiter("bot_alias_available")` -> [BotAliasAvailableWaiter](./waiters.md#botaliasavailablewaiter)
- `client.get_waiter("bot_available")` -> [BotAvailableWaiter](./waiters.md#botavailablewaiter)
- `client.get_waiter("bot_export_completed")` -> [BotExportCompletedWaiter](./waiters.md#botexportcompletedwaiter)
- `client.get_waiter("bot_import_completed")` -> [BotImportCompletedWaiter](./waiters.md#botimportcompletedwaiter)
- `client.get_waiter("bot_locale_built")` -> [BotLocaleBuiltWaiter](./waiters.md#botlocalebuiltwaiter)
- `client.get_waiter("bot_locale_created")` -> [BotLocaleCreatedWaiter](./waiters.md#botlocalecreatedwaiter)
- `client.get_waiter("bot_locale_express_testing_available")` -> [BotLocaleExpressTestingAvailableWaiter](./waiters.md#botlocaleexpresstestingavailablewaiter)
- `client.get_waiter("bot_version_available")` -> [BotVersionAvailableWaiter](./waiters.md#botversionavailablewaiter)


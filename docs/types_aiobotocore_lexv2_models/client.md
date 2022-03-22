<a id="lexmodelsv2client-for-aiobotocore-lexmodelsv2-module"></a>

# LexModelsV2Client for aiobotocore LexModelsV2 module

> [Index](../README.md) > [LexModelsV2](./README.md) > LexModelsV2Client

Auto-generated documentation for
[LexModelsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
type annotations stubs module
[types-aiobotocore-lexv2-models](https://pypi.org/project/types-aiobotocore-lexv2-models/).

- [LexModelsV2Client for aiobotocore LexModelsV2 module](#lexmodelsv2client-for-aiobotocore-lexmodelsv2-module)
  - [LexModelsV2Client](#lexmodelsv2client)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [build_bot_locale](#build_bot_locale)
    - [can_paginate](#can_paginate)
    - [create_bot](#create_bot)
    - [create_bot_alias](#create_bot_alias)
    - [create_bot_locale](#create_bot_locale)
    - [create_bot_version](#create_bot_version)
    - [create_export](#create_export)
    - [create_intent](#create_intent)
    - [create_resource_policy](#create_resource_policy)
    - [create_resource_policy_statement](#create_resource_policy_statement)
    - [create_slot](#create_slot)
    - [create_slot_type](#create_slot_type)
    - [create_upload_url](#create_upload_url)
    - [delete_bot](#delete_bot)
    - [delete_bot_alias](#delete_bot_alias)
    - [delete_bot_locale](#delete_bot_locale)
    - [delete_bot_version](#delete_bot_version)
    - [delete_custom_vocabulary](#delete_custom_vocabulary)
    - [delete_export](#delete_export)
    - [delete_import](#delete_import)
    - [delete_intent](#delete_intent)
    - [delete_resource_policy](#delete_resource_policy)
    - [delete_resource_policy_statement](#delete_resource_policy_statement)
    - [delete_slot](#delete_slot)
    - [delete_slot_type](#delete_slot_type)
    - [delete_utterances](#delete_utterances)
    - [describe_bot](#describe_bot)
    - [describe_bot_alias](#describe_bot_alias)
    - [describe_bot_locale](#describe_bot_locale)
    - [describe_bot_recommendation](#describe_bot_recommendation)
    - [describe_bot_version](#describe_bot_version)
    - [describe_custom_vocabulary_metadata](#describe_custom_vocabulary_metadata)
    - [describe_export](#describe_export)
    - [describe_import](#describe_import)
    - [describe_intent](#describe_intent)
    - [describe_resource_policy](#describe_resource_policy)
    - [describe_slot](#describe_slot)
    - [describe_slot_type](#describe_slot_type)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_aggregated_utterances](#list_aggregated_utterances)
    - [list_bot_aliases](#list_bot_aliases)
    - [list_bot_locales](#list_bot_locales)
    - [list_bot_recommendations](#list_bot_recommendations)
    - [list_bot_versions](#list_bot_versions)
    - [list_bots](#list_bots)
    - [list_built_in_intents](#list_built_in_intents)
    - [list_built_in_slot_types](#list_built_in_slot_types)
    - [list_exports](#list_exports)
    - [list_imports](#list_imports)
    - [list_intents](#list_intents)
    - [list_recommended_intents](#list_recommended_intents)
    - [list_slot_types](#list_slot_types)
    - [list_slots](#list_slots)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [search_associated_transcripts](#search_associated_transcripts)
    - [start_bot_recommendation](#start_bot_recommendation)
    - [start_import](#start_import)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_bot](#update_bot)
    - [update_bot_alias](#update_bot_alias)
    - [update_bot_locale](#update_bot_locale)
    - [update_bot_recommendation](#update_bot_recommendation)
    - [update_export](#update_export)
    - [update_intent](#update_intent)
    - [update_resource_policy](#update_resource_policy)
    - [update_slot](#update_slot)
    - [update_slot_type](#update_slot_type)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_waiter](#get_waiter)

<a id="lexmodelsv2client"></a>

## LexModelsV2Client

Type annotations for `session.create_client("lexv2-models")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_lexv2_models.client import LexModelsV2Client

session = get_session()
async with session.create_client("lexv2-models") as client:
    client: LexModelsV2Client
```

Boto3 documentation:
[LexModelsV2.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_lexv2_models.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.PreconditionFailedException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

LexModelsV2Client exceptions.

Type annotations for `session.create_client("lexv2-models").exceptions` method.

Boto3 documentation:
[LexModelsV2.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="build\_bot\_locale"></a>

### build_bot_locale

Builds a bot, its intents, and its slot types into a specific locale.

Type annotations for `session.create_client("lexv2-models").build_bot_locale`
method.

Boto3 documentation:
[LexModelsV2.Client.build_bot_locale](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.build_bot_locale)

Asynchronous method. Use `await build_bot_locale(...)` for a synchronous call.

Arguments mapping described in
[BuildBotLocaleRequestRequestTypeDef](./type_defs.md#buildbotlocalerequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

Returns a `Coroutine` for
[BuildBotLocaleResponseTypeDef](./type_defs.md#buildbotlocaleresponsetypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("lexv2-models").can_paginate`
method.

Boto3 documentation:
[LexModelsV2.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_bot"></a>

### create_bot

Creates an Amazon Lex conversational bot.

Type annotations for `session.create_client("lexv2-models").create_bot` method.

Boto3 documentation:
[LexModelsV2.Client.create_bot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)

Asynchronous method. Use `await create_bot(...)` for a synchronous call.

Arguments mapping described in
[CreateBotRequestRequestTypeDef](./type_defs.md#createbotrequestrequesttypedef).

Keyword-only arguments:

- `botName`: `str` *(required)*
- `roleArn`: `str` *(required)*
- `dataPrivacy`: [DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef)
  *(required)*
- `idleSessionTTLInSeconds`: `int` *(required)*
- `description`: `str`
- `botTags`: `Mapping`\[`str`, `str`\]
- `testBotAliasTags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateBotResponseTypeDef](./type_defs.md#createbotresponsetypedef).

<a id="create\_bot\_alias"></a>

### create_bot_alias

Creates an alias for the specified version of a bot.

Type annotations for `session.create_client("lexv2-models").create_bot_alias`
method.

Boto3 documentation:
[LexModelsV2.Client.create_bot_alias](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)

Asynchronous method. Use `await create_bot_alias(...)` for a synchronous call.

Arguments mapping described in
[CreateBotAliasRequestRequestTypeDef](./type_defs.md#createbotaliasrequestrequesttypedef).

Keyword-only arguments:

- `botAliasName`: `str` *(required)*
- `botId`: `str` *(required)*
- `description`: `str`
- `botVersion`: `str`
- `botAliasLocaleSettings`: `Mapping`\[`str`,
  [BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef)\]
- `conversationLogSettings`:
  [ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef)
- `sentimentAnalysisSettings`:
  [SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateBotAliasResponseTypeDef](./type_defs.md#createbotaliasresponsetypedef).

<a id="create\_bot\_locale"></a>

### create_bot_locale

Creates a locale in the bot.

Type annotations for `session.create_client("lexv2-models").create_bot_locale`
method.

Boto3 documentation:
[LexModelsV2.Client.create_bot_locale](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_locale)

Asynchronous method. Use `await create_bot_locale(...)` for a synchronous call.

Arguments mapping described in
[CreateBotLocaleRequestRequestTypeDef](./type_defs.md#createbotlocalerequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `nluIntentConfidenceThreshold`: `float` *(required)*
- `description`: `str`
- `voiceSettings`: [VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef)

Returns a `Coroutine` for
[CreateBotLocaleResponseTypeDef](./type_defs.md#createbotlocaleresponsetypedef).

<a id="create\_bot\_version"></a>

### create_bot_version

Creates a new version of the bot based on the `DRAFT` version.

Type annotations for `session.create_client("lexv2-models").create_bot_version`
method.

Boto3 documentation:
[LexModelsV2.Client.create_bot_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_version)

Asynchronous method. Use `await create_bot_version(...)` for a synchronous
call.

Arguments mapping described in
[CreateBotVersionRequestRequestTypeDef](./type_defs.md#createbotversionrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersionLocaleSpecification`: `Mapping`\[`str`,
  [BotVersionLocaleDetailsTypeDef](./type_defs.md#botversionlocaledetailstypedef)\]
  *(required)*
- `description`: `str`

Returns a `Coroutine` for
[CreateBotVersionResponseTypeDef](./type_defs.md#createbotversionresponsetypedef).

<a id="create\_export"></a>

### create_export

Creates a zip archive containing the contents of a bot or a bot locale.

Type annotations for `session.create_client("lexv2-models").create_export`
method.

Boto3 documentation:
[LexModelsV2.Client.create_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_export)

Asynchronous method. Use `await create_export(...)` for a synchronous call.

Arguments mapping described in
[CreateExportRequestRequestTypeDef](./type_defs.md#createexportrequestrequesttypedef).

Keyword-only arguments:

- `resourceSpecification`:
  [ExportResourceSpecificationTypeDef](./type_defs.md#exportresourcespecificationtypedef)
  *(required)*
- `fileFormat`:
  [ImportExportFileFormatType](./literals.md#importexportfileformattype)
  *(required)*
- `filePassword`: `str`

Returns a `Coroutine` for
[CreateExportResponseTypeDef](./type_defs.md#createexportresponsetypedef).

<a id="create\_intent"></a>

### create_intent

Creates an intent.

Type annotations for `session.create_client("lexv2-models").create_intent`
method.

Boto3 documentation:
[LexModelsV2.Client.create_intent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)

Asynchronous method. Use `await create_intent(...)` for a synchronous call.

Arguments mapping described in
[CreateIntentRequestRequestTypeDef](./type_defs.md#createintentrequestrequesttypedef).

Keyword-only arguments:

- `intentName`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `description`: `str`
- `parentIntentSignature`: `str`
- `sampleUtterances`:
  `Sequence`\[[SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef)\]
- `dialogCodeHook`:
  [DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef)
- `fulfillmentCodeHook`:
  [FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef)
- `intentConfirmationSetting`:
  [IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef)
- `intentClosingSetting`:
  [IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef)
- `inputContexts`:
  `Sequence`\[[InputContextTypeDef](./type_defs.md#inputcontexttypedef)\]
- `outputContexts`:
  `Sequence`\[[OutputContextTypeDef](./type_defs.md#outputcontexttypedef)\]
- `kendraConfiguration`:
  [KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef)

Returns a `Coroutine` for
[CreateIntentResponseTypeDef](./type_defs.md#createintentresponsetypedef).

<a id="create\_resource\_policy"></a>

### create_resource_policy

Creates a new resource policy with the specified policy statements.

Type annotations for
`session.create_client("lexv2-models").create_resource_policy` method.

Boto3 documentation:
[LexModelsV2.Client.create_resource_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy)

Asynchronous method. Use `await create_resource_policy(...)` for a synchronous
call.

Arguments mapping described in
[CreateResourcePolicyRequestRequestTypeDef](./type_defs.md#createresourcepolicyrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `policy`: `str` *(required)*

Returns a `Coroutine` for
[CreateResourcePolicyResponseTypeDef](./type_defs.md#createresourcepolicyresponsetypedef).

<a id="create\_resource\_policy\_statement"></a>

### create_resource_policy_statement

Adds a new resource policy statement to a bot or bot alias.

Type annotations for
`session.create_client("lexv2-models").create_resource_policy_statement`
method.

Boto3 documentation:
[LexModelsV2.Client.create_resource_policy_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)

Asynchronous method. Use `await create_resource_policy_statement(...)` for a
synchronous call.

Arguments mapping described in
[CreateResourcePolicyStatementRequestRequestTypeDef](./type_defs.md#createresourcepolicystatementrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `statementId`: `str` *(required)*
- `effect`: [EffectType](./literals.md#effecttype) *(required)*
- `principal`:
  `Sequence`\[[PrincipalTypeDef](./type_defs.md#principaltypedef)\]
  *(required)*
- `action`: `Sequence`\[`str`\] *(required)*
- `condition`: `Mapping`\[`str`, `Mapping`\[`str`, `str`\]\]
- `expectedRevisionId`: `str`

Returns a `Coroutine` for
[CreateResourcePolicyStatementResponseTypeDef](./type_defs.md#createresourcepolicystatementresponsetypedef).

<a id="create\_slot"></a>

### create_slot

Creates a slot in an intent.

Type annotations for `session.create_client("lexv2-models").create_slot`
method.

Boto3 documentation:
[LexModelsV2.Client.create_slot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)

Asynchronous method. Use `await create_slot(...)` for a synchronous call.

Arguments mapping described in
[CreateSlotRequestRequestTypeDef](./type_defs.md#createslotrequestrequesttypedef).

Keyword-only arguments:

- `slotName`: `str` *(required)*
- `valueElicitationSetting`:
  [SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef)
  *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `intentId`: `str` *(required)*
- `description`: `str`
- `slotTypeId`: `str`
- `obfuscationSetting`:
  [ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef)
- `multipleValuesSetting`:
  [MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef)

Returns a `Coroutine` for
[CreateSlotResponseTypeDef](./type_defs.md#createslotresponsetypedef).

<a id="create\_slot\_type"></a>

### create_slot_type

Creates a custom slot type To create a custom slot type, specify a name for the
slot type and a set of enumeration values, the values that a slot of this type
can assume.

Type annotations for `session.create_client("lexv2-models").create_slot_type`
method.

Boto3 documentation:
[LexModelsV2.Client.create_slot_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)

Asynchronous method. Use `await create_slot_type(...)` for a synchronous call.

Arguments mapping described in
[CreateSlotTypeRequestRequestTypeDef](./type_defs.md#createslottyperequestrequesttypedef).

Keyword-only arguments:

- `slotTypeName`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `description`: `str`
- `slotTypeValues`:
  `Sequence`\[[SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef)\]
- `valueSelectionSetting`:
  [SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef)
- `parentSlotTypeSignature`: `str`
- `externalSourceSetting`:
  [ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef)

Returns a `Coroutine` for
[CreateSlotTypeResponseTypeDef](./type_defs.md#createslottyperesponsetypedef).

<a id="create\_upload\_url"></a>

### create_upload_url

Gets a pre-signed S3 write URL that you use to upload the zip archive when
importing a bot or a bot locale.

Type annotations for `session.create_client("lexv2-models").create_upload_url`
method.

Boto3 documentation:
[LexModelsV2.Client.create_upload_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_upload_url)

Asynchronous method. Use `await create_upload_url(...)` for a synchronous call.

Returns a `Coroutine` for
[CreateUploadUrlResponseTypeDef](./type_defs.md#createuploadurlresponsetypedef).

<a id="delete\_bot"></a>

### delete_bot

Deletes all versions of a bot, including the `Draft` version.

Type annotations for `session.create_client("lexv2-models").delete_bot` method.

Boto3 documentation:
[LexModelsV2.Client.delete_bot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot)

Asynchronous method. Use `await delete_bot(...)` for a synchronous call.

Arguments mapping described in
[DeleteBotRequestRequestTypeDef](./type_defs.md#deletebotrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `skipResourceInUseCheck`: `bool`

Returns a `Coroutine` for
[DeleteBotResponseTypeDef](./type_defs.md#deletebotresponsetypedef).

<a id="delete\_bot\_alias"></a>

### delete_bot_alias

Deletes the specified bot alias.

Type annotations for `session.create_client("lexv2-models").delete_bot_alias`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_bot_alias](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_alias)

Asynchronous method. Use `await delete_bot_alias(...)` for a synchronous call.

Arguments mapping described in
[DeleteBotAliasRequestRequestTypeDef](./type_defs.md#deletebotaliasrequestrequesttypedef).

Keyword-only arguments:

- `botAliasId`: `str` *(required)*
- `botId`: `str` *(required)*
- `skipResourceInUseCheck`: `bool`

Returns a `Coroutine` for
[DeleteBotAliasResponseTypeDef](./type_defs.md#deletebotaliasresponsetypedef).

<a id="delete\_bot\_locale"></a>

### delete_bot_locale

Removes a locale from a bot.

Type annotations for `session.create_client("lexv2-models").delete_bot_locale`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_bot_locale](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_locale)

Asynchronous method. Use `await delete_bot_locale(...)` for a synchronous call.

Arguments mapping described in
[DeleteBotLocaleRequestRequestTypeDef](./type_defs.md#deletebotlocalerequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteBotLocaleResponseTypeDef](./type_defs.md#deletebotlocaleresponsetypedef).

<a id="delete\_bot\_version"></a>

### delete_bot_version

Deletes a specific version of a bot.

Type annotations for `session.create_client("lexv2-models").delete_bot_version`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_bot_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_version)

Asynchronous method. Use `await delete_bot_version(...)` for a synchronous
call.

Arguments mapping described in
[DeleteBotVersionRequestRequestTypeDef](./type_defs.md#deletebotversionrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `skipResourceInUseCheck`: `bool`

Returns a `Coroutine` for
[DeleteBotVersionResponseTypeDef](./type_defs.md#deletebotversionresponsetypedef).

<a id="delete\_custom\_vocabulary"></a>

### delete_custom_vocabulary

Removes a custom vocabulary from the specified locale in the specified bot.

Type annotations for
`session.create_client("lexv2-models").delete_custom_vocabulary` method.

Boto3 documentation:
[LexModelsV2.Client.delete_custom_vocabulary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_custom_vocabulary)

Asynchronous method. Use `await delete_custom_vocabulary(...)` for a
synchronous call.

Arguments mapping described in
[DeleteCustomVocabularyRequestRequestTypeDef](./type_defs.md#deletecustomvocabularyrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteCustomVocabularyResponseTypeDef](./type_defs.md#deletecustomvocabularyresponsetypedef).

<a id="delete\_export"></a>

### delete_export

Removes a previous export and the associated files stored in an S3 bucket.

Type annotations for `session.create_client("lexv2-models").delete_export`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_export)

Asynchronous method. Use `await delete_export(...)` for a synchronous call.

Arguments mapping described in
[DeleteExportRequestRequestTypeDef](./type_defs.md#deleteexportrequestrequesttypedef).

Keyword-only arguments:

- `exportId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteExportResponseTypeDef](./type_defs.md#deleteexportresponsetypedef).

<a id="delete\_import"></a>

### delete_import

Removes a previous import and the associated file stored in an S3 bucket.

Type annotations for `session.create_client("lexv2-models").delete_import`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_import](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_import)

Asynchronous method. Use `await delete_import(...)` for a synchronous call.

Arguments mapping described in
[DeleteImportRequestRequestTypeDef](./type_defs.md#deleteimportrequestrequesttypedef).

Keyword-only arguments:

- `importId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteImportResponseTypeDef](./type_defs.md#deleteimportresponsetypedef).

<a id="delete\_intent"></a>

### delete_intent

Removes the specified intent.

Type annotations for `session.create_client("lexv2-models").delete_intent`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_intent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_intent)

Asynchronous method. Use `await delete_intent(...)` for a synchronous call.

Arguments mapping described in
[DeleteIntentRequestRequestTypeDef](./type_defs.md#deleteintentrequestrequesttypedef).

Keyword-only arguments:

- `intentId`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

<a id="delete\_resource\_policy"></a>

### delete_resource_policy

Removes an existing policy from a bot or bot alias.

Type annotations for
`session.create_client("lexv2-models").delete_resource_policy` method.

Boto3 documentation:
[LexModelsV2.Client.delete_resource_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy)

Asynchronous method. Use `await delete_resource_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `expectedRevisionId`: `str`

Returns a `Coroutine` for
[DeleteResourcePolicyResponseTypeDef](./type_defs.md#deleteresourcepolicyresponsetypedef).

<a id="delete\_resource\_policy\_statement"></a>

### delete_resource_policy_statement

Deletes a policy statement from a resource policy.

Type annotations for
`session.create_client("lexv2-models").delete_resource_policy_statement`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_resource_policy_statement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy_statement)

Asynchronous method. Use `await delete_resource_policy_statement(...)` for a
synchronous call.

Arguments mapping described in
[DeleteResourcePolicyStatementRequestRequestTypeDef](./type_defs.md#deleteresourcepolicystatementrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `statementId`: `str` *(required)*
- `expectedRevisionId`: `str`

Returns a `Coroutine` for
[DeleteResourcePolicyStatementResponseTypeDef](./type_defs.md#deleteresourcepolicystatementresponsetypedef).

<a id="delete\_slot"></a>

### delete_slot

Deletes the specified slot from an intent.

Type annotations for `session.create_client("lexv2-models").delete_slot`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_slot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot)

Asynchronous method. Use `await delete_slot(...)` for a synchronous call.

Arguments mapping described in
[DeleteSlotRequestRequestTypeDef](./type_defs.md#deleteslotrequestrequesttypedef).

Keyword-only arguments:

- `slotId`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `intentId`: `str` *(required)*

<a id="delete\_slot\_type"></a>

### delete_slot_type

Deletes a slot type from a bot locale.

Type annotations for `session.create_client("lexv2-models").delete_slot_type`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_slot_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot_type)

Asynchronous method. Use `await delete_slot_type(...)` for a synchronous call.

Arguments mapping described in
[DeleteSlotTypeRequestRequestTypeDef](./type_defs.md#deleteslottyperequestrequesttypedef).

Keyword-only arguments:

- `slotTypeId`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `skipResourceInUseCheck`: `bool`

<a id="delete\_utterances"></a>

### delete_utterances

Deletes stored utterances.

Type annotations for `session.create_client("lexv2-models").delete_utterances`
method.

Boto3 documentation:
[LexModelsV2.Client.delete_utterances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_utterances)

Asynchronous method. Use `await delete_utterances(...)` for a synchronous call.

Arguments mapping described in
[DeleteUtterancesRequestRequestTypeDef](./type_defs.md#deleteutterancesrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `localeId`: `str`
- `sessionId`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_bot"></a>

### describe_bot

Provides metadata information about a bot.

Type annotations for `session.create_client("lexv2-models").describe_bot`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_bot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot)

Asynchronous method. Use `await describe_bot(...)` for a synchronous call.

Arguments mapping described in
[DescribeBotRequestRequestTypeDef](./type_defs.md#describebotrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBotResponseTypeDef](./type_defs.md#describebotresponsetypedef).

<a id="describe\_bot\_alias"></a>

### describe_bot_alias

Get information about a specific bot alias.

Type annotations for `session.create_client("lexv2-models").describe_bot_alias`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_bot_alias](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_alias)

Asynchronous method. Use `await describe_bot_alias(...)` for a synchronous
call.

Arguments mapping described in
[DescribeBotAliasRequestRequestTypeDef](./type_defs.md#describebotaliasrequestrequesttypedef).

Keyword-only arguments:

- `botAliasId`: `str` *(required)*
- `botId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBotAliasResponseTypeDef](./type_defs.md#describebotaliasresponsetypedef).

<a id="describe\_bot\_locale"></a>

### describe_bot_locale

Describes the settings that a bot has for a specific locale.

Type annotations for
`session.create_client("lexv2-models").describe_bot_locale` method.

Boto3 documentation:
[LexModelsV2.Client.describe_bot_locale](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_locale)

Asynchronous method. Use `await describe_bot_locale(...)` for a synchronous
call.

Arguments mapping described in
[DescribeBotLocaleRequestRequestTypeDef](./type_defs.md#describebotlocalerequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBotLocaleResponseTypeDef](./type_defs.md#describebotlocaleresponsetypedef).

<a id="describe\_bot\_recommendation"></a>

### describe_bot_recommendation

Provides metadata information about a bot recommendation.

Type annotations for
`session.create_client("lexv2-models").describe_bot_recommendation` method.

Boto3 documentation:
[LexModelsV2.Client.describe_bot_recommendation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_recommendation)

Asynchronous method. Use `await describe_bot_recommendation(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBotRecommendationRequestRequestTypeDef](./type_defs.md#describebotrecommendationrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `botRecommendationId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBotRecommendationResponseTypeDef](./type_defs.md#describebotrecommendationresponsetypedef).

<a id="describe\_bot\_version"></a>

### describe_bot_version

Provides metadata about a version of a bot.

Type annotations for
`session.create_client("lexv2-models").describe_bot_version` method.

Boto3 documentation:
[LexModelsV2.Client.describe_bot_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_version)

Asynchronous method. Use `await describe_bot_version(...)` for a synchronous
call.

Arguments mapping described in
[DescribeBotVersionRequestRequestTypeDef](./type_defs.md#describebotversionrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBotVersionResponseTypeDef](./type_defs.md#describebotversionresponsetypedef).

<a id="describe\_custom\_vocabulary\_metadata"></a>

### describe_custom_vocabulary_metadata

Provides metadata information about a custom vocabulary.

Type annotations for
`session.create_client("lexv2-models").describe_custom_vocabulary_metadata`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_custom_vocabulary_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_custom_vocabulary_metadata)

Asynchronous method. Use `await describe_custom_vocabulary_metadata(...)` for a
synchronous call.

Arguments mapping described in
[DescribeCustomVocabularyMetadataRequestRequestTypeDef](./type_defs.md#describecustomvocabularymetadatarequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeCustomVocabularyMetadataResponseTypeDef](./type_defs.md#describecustomvocabularymetadataresponsetypedef).

<a id="describe\_export"></a>

### describe_export

Gets information about a specific export.

Type annotations for `session.create_client("lexv2-models").describe_export`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_export)

Asynchronous method. Use `await describe_export(...)` for a synchronous call.

Arguments mapping described in
[DescribeExportRequestRequestTypeDef](./type_defs.md#describeexportrequestrequesttypedef).

Keyword-only arguments:

- `exportId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeExportResponseTypeDef](./type_defs.md#describeexportresponsetypedef).

<a id="describe\_import"></a>

### describe_import

Gets information about a specific import.

Type annotations for `session.create_client("lexv2-models").describe_import`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_import](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_import)

Asynchronous method. Use `await describe_import(...)` for a synchronous call.

Arguments mapping described in
[DescribeImportRequestRequestTypeDef](./type_defs.md#describeimportrequestrequesttypedef).

Keyword-only arguments:

- `importId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeImportResponseTypeDef](./type_defs.md#describeimportresponsetypedef).

<a id="describe\_intent"></a>

### describe_intent

Returns metadata about an intent.

Type annotations for `session.create_client("lexv2-models").describe_intent`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_intent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_intent)

Asynchronous method. Use `await describe_intent(...)` for a synchronous call.

Arguments mapping described in
[DescribeIntentRequestRequestTypeDef](./type_defs.md#describeintentrequestrequesttypedef).

Keyword-only arguments:

- `intentId`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeIntentResponseTypeDef](./type_defs.md#describeintentresponsetypedef).

<a id="describe\_resource\_policy"></a>

### describe_resource_policy

Gets the resource policy and policy revision for a bot or bot alias.

Type annotations for
`session.create_client("lexv2-models").describe_resource_policy` method.

Boto3 documentation:
[LexModelsV2.Client.describe_resource_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_resource_policy)

Asynchronous method. Use `await describe_resource_policy(...)` for a
synchronous call.

Arguments mapping described in
[DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef).

<a id="describe\_slot"></a>

### describe_slot

Gets metadata information about a slot.

Type annotations for `session.create_client("lexv2-models").describe_slot`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_slot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot)

Asynchronous method. Use `await describe_slot(...)` for a synchronous call.

Arguments mapping described in
[DescribeSlotRequestRequestTypeDef](./type_defs.md#describeslotrequestrequesttypedef).

Keyword-only arguments:

- `slotId`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `intentId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSlotResponseTypeDef](./type_defs.md#describeslotresponsetypedef).

<a id="describe\_slot\_type"></a>

### describe_slot_type

Gets metadata information about a slot type.

Type annotations for `session.create_client("lexv2-models").describe_slot_type`
method.

Boto3 documentation:
[LexModelsV2.Client.describe_slot_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot_type)

Asynchronous method. Use `await describe_slot_type(...)` for a synchronous
call.

Arguments mapping described in
[DescribeSlotTypeRequestRequestTypeDef](./type_defs.md#describeslottyperequestrequesttypedef).

Keyword-only arguments:

- `slotTypeId`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSlotTypeResponseTypeDef](./type_defs.md#describeslottyperesponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("lexv2-models").generate_presigned_url` method.

Boto3 documentation:
[LexModelsV2.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_aggregated\_utterances"></a>

### list_aggregated_utterances

Provides a list of utterances that users have sent to the bot.

Type annotations for
`session.create_client("lexv2-models").list_aggregated_utterances` method.

Boto3 documentation:
[LexModelsV2.Client.list_aggregated_utterances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_aggregated_utterances)

Asynchronous method. Use `await list_aggregated_utterances(...)` for a
synchronous call.

Arguments mapping described in
[ListAggregatedUtterancesRequestRequestTypeDef](./type_defs.md#listaggregatedutterancesrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `localeId`: `str` *(required)*
- `aggregationDuration`:
  [UtteranceAggregationDurationTypeDef](./type_defs.md#utteranceaggregationdurationtypedef)
  *(required)*
- `botAliasId`: `str`
- `botVersion`: `str`
- `sortBy`:
  [AggregatedUtterancesSortByTypeDef](./type_defs.md#aggregatedutterancessortbytypedef)
- `filters`:
  `Sequence`\[[AggregatedUtterancesFilterTypeDef](./type_defs.md#aggregatedutterancesfiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListAggregatedUtterancesResponseTypeDef](./type_defs.md#listaggregatedutterancesresponsetypedef).

<a id="list\_bot\_aliases"></a>

### list_bot_aliases

Gets a list of aliases for the specified bot.

Type annotations for `session.create_client("lexv2-models").list_bot_aliases`
method.

Boto3 documentation:
[LexModelsV2.Client.list_bot_aliases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_aliases)

Asynchronous method. Use `await list_bot_aliases(...)` for a synchronous call.

Arguments mapping described in
[ListBotAliasesRequestRequestTypeDef](./type_defs.md#listbotaliasesrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBotAliasesResponseTypeDef](./type_defs.md#listbotaliasesresponsetypedef).

<a id="list\_bot\_locales"></a>

### list_bot_locales

Gets a list of locales for the specified bot.

Type annotations for `session.create_client("lexv2-models").list_bot_locales`
method.

Boto3 documentation:
[LexModelsV2.Client.list_bot_locales](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_locales)

Asynchronous method. Use `await list_bot_locales(...)` for a synchronous call.

Arguments mapping described in
[ListBotLocalesRequestRequestTypeDef](./type_defs.md#listbotlocalesrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `sortBy`: [BotLocaleSortByTypeDef](./type_defs.md#botlocalesortbytypedef)
- `filters`:
  `Sequence`\[[BotLocaleFilterTypeDef](./type_defs.md#botlocalefiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBotLocalesResponseTypeDef](./type_defs.md#listbotlocalesresponsetypedef).

<a id="list\_bot\_recommendations"></a>

### list_bot_recommendations

Get a list of bot recommendations that meet the specified criteria.

Type annotations for
`session.create_client("lexv2-models").list_bot_recommendations` method.

Boto3 documentation:
[LexModelsV2.Client.list_bot_recommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_recommendations)

Asynchronous method. Use `await list_bot_recommendations(...)` for a
synchronous call.

Arguments mapping described in
[ListBotRecommendationsRequestRequestTypeDef](./type_defs.md#listbotrecommendationsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBotRecommendationsResponseTypeDef](./type_defs.md#listbotrecommendationsresponsetypedef).

<a id="list\_bot\_versions"></a>

### list_bot_versions

Gets information about all of the versions of a bot.

Type annotations for `session.create_client("lexv2-models").list_bot_versions`
method.

Boto3 documentation:
[LexModelsV2.Client.list_bot_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_versions)

Asynchronous method. Use `await list_bot_versions(...)` for a synchronous call.

Arguments mapping described in
[ListBotVersionsRequestRequestTypeDef](./type_defs.md#listbotversionsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `sortBy`: [BotVersionSortByTypeDef](./type_defs.md#botversionsortbytypedef)
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBotVersionsResponseTypeDef](./type_defs.md#listbotversionsresponsetypedef).

<a id="list\_bots"></a>

### list_bots

Gets a list of available bots.

Type annotations for `session.create_client("lexv2-models").list_bots` method.

Boto3 documentation:
[LexModelsV2.Client.list_bots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bots)

Asynchronous method. Use `await list_bots(...)` for a synchronous call.

Arguments mapping described in
[ListBotsRequestRequestTypeDef](./type_defs.md#listbotsrequestrequesttypedef).

Keyword-only arguments:

- `sortBy`: [BotSortByTypeDef](./type_defs.md#botsortbytypedef)
- `filters`: `Sequence`\[[BotFilterTypeDef](./type_defs.md#botfiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef).

<a id="list\_built\_in\_intents"></a>

### list_built_in_intents

Gets a list of built-in intents provided by Amazon Lex that you can use in your
bot.

Type annotations for
`session.create_client("lexv2-models").list_built_in_intents` method.

Boto3 documentation:
[LexModelsV2.Client.list_built_in_intents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_intents)

Asynchronous method. Use `await list_built_in_intents(...)` for a synchronous
call.

Arguments mapping described in
[ListBuiltInIntentsRequestRequestTypeDef](./type_defs.md#listbuiltinintentsrequestrequesttypedef).

Keyword-only arguments:

- `localeId`: `str` *(required)*
- `sortBy`:
  [BuiltInIntentSortByTypeDef](./type_defs.md#builtinintentsortbytypedef)
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBuiltInIntentsResponseTypeDef](./type_defs.md#listbuiltinintentsresponsetypedef).

<a id="list\_built\_in\_slot\_types"></a>

### list_built_in_slot_types

Gets a list of built-in slot types that meet the specified criteria.

Type annotations for
`session.create_client("lexv2-models").list_built_in_slot_types` method.

Boto3 documentation:
[LexModelsV2.Client.list_built_in_slot_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_slot_types)

Asynchronous method. Use `await list_built_in_slot_types(...)` for a
synchronous call.

Arguments mapping described in
[ListBuiltInSlotTypesRequestRequestTypeDef](./type_defs.md#listbuiltinslottypesrequestrequesttypedef).

Keyword-only arguments:

- `localeId`: `str` *(required)*
- `sortBy`:
  [BuiltInSlotTypeSortByTypeDef](./type_defs.md#builtinslottypesortbytypedef)
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBuiltInSlotTypesResponseTypeDef](./type_defs.md#listbuiltinslottypesresponsetypedef).

<a id="list\_exports"></a>

### list_exports

Lists the exports for a bot, bot locale, or custom vocabulary.

Type annotations for `session.create_client("lexv2-models").list_exports`
method.

Boto3 documentation:
[LexModelsV2.Client.list_exports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_exports)

Asynchronous method. Use `await list_exports(...)` for a synchronous call.

Arguments mapping described in
[ListExportsRequestRequestTypeDef](./type_defs.md#listexportsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str`
- `botVersion`: `str`
- `sortBy`: [ExportSortByTypeDef](./type_defs.md#exportsortbytypedef)
- `filters`:
  `Sequence`\[[ExportFilterTypeDef](./type_defs.md#exportfiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`
- `localeId`: `str`

Returns a `Coroutine` for
[ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef).

<a id="list\_imports"></a>

### list_imports

Lists the imports for a bot, bot locale, or custom vocabulary.

Type annotations for `session.create_client("lexv2-models").list_imports`
method.

Boto3 documentation:
[LexModelsV2.Client.list_imports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)

Asynchronous method. Use `await list_imports(...)` for a synchronous call.

Arguments mapping described in
[ListImportsRequestRequestTypeDef](./type_defs.md#listimportsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str`
- `botVersion`: `str`
- `sortBy`: [ImportSortByTypeDef](./type_defs.md#importsortbytypedef)
- `filters`:
  `Sequence`\[[ImportFilterTypeDef](./type_defs.md#importfiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`
- `localeId`: `str`

Returns a `Coroutine` for
[ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef).

<a id="list\_intents"></a>

### list_intents

Get a list of intents that meet the specified criteria.

Type annotations for `session.create_client("lexv2-models").list_intents`
method.

Boto3 documentation:
[LexModelsV2.Client.list_intents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intents)

Asynchronous method. Use `await list_intents(...)` for a synchronous call.

Arguments mapping described in
[ListIntentsRequestRequestTypeDef](./type_defs.md#listintentsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `sortBy`: [IntentSortByTypeDef](./type_defs.md#intentsortbytypedef)
- `filters`:
  `Sequence`\[[IntentFilterTypeDef](./type_defs.md#intentfiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListIntentsResponseTypeDef](./type_defs.md#listintentsresponsetypedef).

<a id="list\_recommended\_intents"></a>

### list_recommended_intents

Gets a list of recommended intents provided by the bot recommendation that you
can use in your bot.

Type annotations for
`session.create_client("lexv2-models").list_recommended_intents` method.

Boto3 documentation:
[LexModelsV2.Client.list_recommended_intents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)

Asynchronous method. Use `await list_recommended_intents(...)` for a
synchronous call.

Arguments mapping described in
[ListRecommendedIntentsRequestRequestTypeDef](./type_defs.md#listrecommendedintentsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `botRecommendationId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListRecommendedIntentsResponseTypeDef](./type_defs.md#listrecommendedintentsresponsetypedef).

<a id="list\_slot\_types"></a>

### list_slot_types

Gets a list of slot types that match the specified criteria.

Type annotations for `session.create_client("lexv2-models").list_slot_types`
method.

Boto3 documentation:
[LexModelsV2.Client.list_slot_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slot_types)

Asynchronous method. Use `await list_slot_types(...)` for a synchronous call.

Arguments mapping described in
[ListSlotTypesRequestRequestTypeDef](./type_defs.md#listslottypesrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `sortBy`: [SlotTypeSortByTypeDef](./type_defs.md#slottypesortbytypedef)
- `filters`:
  `Sequence`\[[SlotTypeFilterTypeDef](./type_defs.md#slottypefiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListSlotTypesResponseTypeDef](./type_defs.md#listslottypesresponsetypedef).

<a id="list\_slots"></a>

### list_slots

Gets a list of slots that match the specified criteria.

Type annotations for `session.create_client("lexv2-models").list_slots` method.

Boto3 documentation:
[LexModelsV2.Client.list_slots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slots)

Asynchronous method. Use `await list_slots(...)` for a synchronous call.

Arguments mapping described in
[ListSlotsRequestRequestTypeDef](./type_defs.md#listslotsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `intentId`: `str` *(required)*
- `sortBy`: [SlotSortByTypeDef](./type_defs.md#slotsortbytypedef)
- `filters`:
  `Sequence`\[[SlotFilterTypeDef](./type_defs.md#slotfiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListSlotsResponseTypeDef](./type_defs.md#listslotsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Gets a list of tags associated with a resource.

Type annotations for
`session.create_client("lexv2-models").list_tags_for_resource` method.

Boto3 documentation:
[LexModelsV2.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceARN`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="search\_associated\_transcripts"></a>

### search_associated_transcripts

Search for associated transcripts that meet the specified criteria.

Type annotations for
`session.create_client("lexv2-models").search_associated_transcripts` method.

Boto3 documentation:
[LexModelsV2.Client.search_associated_transcripts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.search_associated_transcripts)

Asynchronous method. Use `await search_associated_transcripts(...)` for a
synchronous call.

Arguments mapping described in
[SearchAssociatedTranscriptsRequestRequestTypeDef](./type_defs.md#searchassociatedtranscriptsrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `botRecommendationId`: `str` *(required)*
- `filters`:
  `Sequence`\[[AssociatedTranscriptFilterTypeDef](./type_defs.md#associatedtranscriptfiltertypedef)\]
  *(required)*
- `searchOrder`: [SearchOrderType](./literals.md#searchordertype)
- `maxResults`: `int`
- `nextIndex`: `int`

Returns a `Coroutine` for
[SearchAssociatedTranscriptsResponseTypeDef](./type_defs.md#searchassociatedtranscriptsresponsetypedef).

<a id="start\_bot\_recommendation"></a>

### start_bot_recommendation

Use this to provide your transcript data, and to start the bot recommendation
process.

Type annotations for
`session.create_client("lexv2-models").start_bot_recommendation` method.

Boto3 documentation:
[LexModelsV2.Client.start_bot_recommendation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)

Asynchronous method. Use `await start_bot_recommendation(...)` for a
synchronous call.

Arguments mapping described in
[StartBotRecommendationRequestRequestTypeDef](./type_defs.md#startbotrecommendationrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `transcriptSourceSetting`:
  [TranscriptSourceSettingTypeDef](./type_defs.md#transcriptsourcesettingtypedef)
  *(required)*
- `encryptionSetting`:
  [EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef)

Returns a `Coroutine` for
[StartBotRecommendationResponseTypeDef](./type_defs.md#startbotrecommendationresponsetypedef).

<a id="start\_import"></a>

### start_import

Starts importing a bot, bot locale, or custom vocabulary from a zip archive
that you uploaded to an S3 bucket.

Type annotations for `session.create_client("lexv2-models").start_import`
method.

Boto3 documentation:
[LexModelsV2.Client.start_import](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_import)

Asynchronous method. Use `await start_import(...)` for a synchronous call.

Arguments mapping described in
[StartImportRequestRequestTypeDef](./type_defs.md#startimportrequestrequesttypedef).

Keyword-only arguments:

- `importId`: `str` *(required)*
- `resourceSpecification`:
  [ImportResourceSpecificationTypeDef](./type_defs.md#importresourcespecificationtypedef)
  *(required)*
- `mergeStrategy`: [MergeStrategyType](./literals.md#mergestrategytype)
  *(required)*
- `filePassword`: `str`

Returns a `Coroutine` for
[StartImportResponseTypeDef](./type_defs.md#startimportresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds the specified tags to the specified resource.

Type annotations for `session.create_client("lexv2-models").tag_resource`
method.

Boto3 documentation:
[LexModelsV2.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceARN`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes tags from a bot, bot alias, or bot channel.

Type annotations for `session.create_client("lexv2-models").untag_resource`
method.

Boto3 documentation:
[LexModelsV2.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceARN`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_bot"></a>

### update_bot

Updates the configuration of an existing bot.

Type annotations for `session.create_client("lexv2-models").update_bot` method.

Boto3 documentation:
[LexModelsV2.Client.update_bot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)

Asynchronous method. Use `await update_bot(...)` for a synchronous call.

Arguments mapping described in
[UpdateBotRequestRequestTypeDef](./type_defs.md#updatebotrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botName`: `str` *(required)*
- `roleArn`: `str` *(required)*
- `dataPrivacy`: [DataPrivacyTypeDef](./type_defs.md#dataprivacytypedef)
  *(required)*
- `idleSessionTTLInSeconds`: `int` *(required)*
- `description`: `str`

Returns a `Coroutine` for
[UpdateBotResponseTypeDef](./type_defs.md#updatebotresponsetypedef).

<a id="update\_bot\_alias"></a>

### update_bot_alias

Updates the configuration of an existing bot alias.

Type annotations for `session.create_client("lexv2-models").update_bot_alias`
method.

Boto3 documentation:
[LexModelsV2.Client.update_bot_alias](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)

Asynchronous method. Use `await update_bot_alias(...)` for a synchronous call.

Arguments mapping described in
[UpdateBotAliasRequestRequestTypeDef](./type_defs.md#updatebotaliasrequestrequesttypedef).

Keyword-only arguments:

- `botAliasId`: `str` *(required)*
- `botAliasName`: `str` *(required)*
- `botId`: `str` *(required)*
- `description`: `str`
- `botVersion`: `str`
- `botAliasLocaleSettings`: `Mapping`\[`str`,
  [BotAliasLocaleSettingsTypeDef](./type_defs.md#botaliaslocalesettingstypedef)\]
- `conversationLogSettings`:
  [ConversationLogSettingsTypeDef](./type_defs.md#conversationlogsettingstypedef)
- `sentimentAnalysisSettings`:
  [SentimentAnalysisSettingsTypeDef](./type_defs.md#sentimentanalysissettingstypedef)

Returns a `Coroutine` for
[UpdateBotAliasResponseTypeDef](./type_defs.md#updatebotaliasresponsetypedef).

<a id="update\_bot\_locale"></a>

### update_bot_locale

Updates the settings that a bot has for a specific locale.

Type annotations for `session.create_client("lexv2-models").update_bot_locale`
method.

Boto3 documentation:
[LexModelsV2.Client.update_bot_locale](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_locale)

Asynchronous method. Use `await update_bot_locale(...)` for a synchronous call.

Arguments mapping described in
[UpdateBotLocaleRequestRequestTypeDef](./type_defs.md#updatebotlocalerequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `nluIntentConfidenceThreshold`: `float` *(required)*
- `description`: `str`
- `voiceSettings`: [VoiceSettingsTypeDef](./type_defs.md#voicesettingstypedef)

Returns a `Coroutine` for
[UpdateBotLocaleResponseTypeDef](./type_defs.md#updatebotlocaleresponsetypedef).

<a id="update\_bot\_recommendation"></a>

### update_bot_recommendation

Updates an existing bot recommendation request.

Type annotations for
`session.create_client("lexv2-models").update_bot_recommendation` method.

Boto3 documentation:
[LexModelsV2.Client.update_bot_recommendation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_recommendation)

Asynchronous method. Use `await update_bot_recommendation(...)` for a
synchronous call.

Arguments mapping described in
[UpdateBotRecommendationRequestRequestTypeDef](./type_defs.md#updatebotrecommendationrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `botRecommendationId`: `str` *(required)*
- `encryptionSetting`:
  [EncryptionSettingTypeDef](./type_defs.md#encryptionsettingtypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateBotRecommendationResponseTypeDef](./type_defs.md#updatebotrecommendationresponsetypedef).

<a id="update\_export"></a>

### update_export

Updates the password used to protect an export zip archive.

Type annotations for `session.create_client("lexv2-models").update_export`
method.

Boto3 documentation:
[LexModelsV2.Client.update_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_export)

Asynchronous method. Use `await update_export(...)` for a synchronous call.

Arguments mapping described in
[UpdateExportRequestRequestTypeDef](./type_defs.md#updateexportrequestrequesttypedef).

Keyword-only arguments:

- `exportId`: `str` *(required)*
- `filePassword`: `str`

Returns a `Coroutine` for
[UpdateExportResponseTypeDef](./type_defs.md#updateexportresponsetypedef).

<a id="update\_intent"></a>

### update_intent

Updates the settings for an intent.

Type annotations for `session.create_client("lexv2-models").update_intent`
method.

Boto3 documentation:
[LexModelsV2.Client.update_intent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)

Asynchronous method. Use `await update_intent(...)` for a synchronous call.

Arguments mapping described in
[UpdateIntentRequestRequestTypeDef](./type_defs.md#updateintentrequestrequesttypedef).

Keyword-only arguments:

- `intentId`: `str` *(required)*
- `intentName`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `description`: `str`
- `parentIntentSignature`: `str`
- `sampleUtterances`:
  `Sequence`\[[SampleUtteranceTypeDef](./type_defs.md#sampleutterancetypedef)\]
- `dialogCodeHook`:
  [DialogCodeHookSettingsTypeDef](./type_defs.md#dialogcodehooksettingstypedef)
- `fulfillmentCodeHook`:
  [FulfillmentCodeHookSettingsTypeDef](./type_defs.md#fulfillmentcodehooksettingstypedef)
- `slotPriorities`:
  `Sequence`\[[SlotPriorityTypeDef](./type_defs.md#slotprioritytypedef)\]
- `intentConfirmationSetting`:
  [IntentConfirmationSettingTypeDef](./type_defs.md#intentconfirmationsettingtypedef)
- `intentClosingSetting`:
  [IntentClosingSettingTypeDef](./type_defs.md#intentclosingsettingtypedef)
- `inputContexts`:
  `Sequence`\[[InputContextTypeDef](./type_defs.md#inputcontexttypedef)\]
- `outputContexts`:
  `Sequence`\[[OutputContextTypeDef](./type_defs.md#outputcontexttypedef)\]
- `kendraConfiguration`:
  [KendraConfigurationTypeDef](./type_defs.md#kendraconfigurationtypedef)

Returns a `Coroutine` for
[UpdateIntentResponseTypeDef](./type_defs.md#updateintentresponsetypedef).

<a id="update\_resource\_policy"></a>

### update_resource_policy

Replaces the existing resource policy for a bot or bot alias with a new one.

Type annotations for
`session.create_client("lexv2-models").update_resource_policy` method.

Boto3 documentation:
[LexModelsV2.Client.update_resource_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_resource_policy)

Asynchronous method. Use `await update_resource_policy(...)` for a synchronous
call.

Arguments mapping described in
[UpdateResourcePolicyRequestRequestTypeDef](./type_defs.md#updateresourcepolicyrequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `policy`: `str` *(required)*
- `expectedRevisionId`: `str`

Returns a `Coroutine` for
[UpdateResourcePolicyResponseTypeDef](./type_defs.md#updateresourcepolicyresponsetypedef).

<a id="update\_slot"></a>

### update_slot

Updates the settings for a slot.

Type annotations for `session.create_client("lexv2-models").update_slot`
method.

Boto3 documentation:
[LexModelsV2.Client.update_slot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)

Asynchronous method. Use `await update_slot(...)` for a synchronous call.

Arguments mapping described in
[UpdateSlotRequestRequestTypeDef](./type_defs.md#updateslotrequestrequesttypedef).

Keyword-only arguments:

- `slotId`: `str` *(required)*
- `slotName`: `str` *(required)*
- `valueElicitationSetting`:
  [SlotValueElicitationSettingTypeDef](./type_defs.md#slotvalueelicitationsettingtypedef)
  *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `intentId`: `str` *(required)*
- `description`: `str`
- `slotTypeId`: `str`
- `obfuscationSetting`:
  [ObfuscationSettingTypeDef](./type_defs.md#obfuscationsettingtypedef)
- `multipleValuesSetting`:
  [MultipleValuesSettingTypeDef](./type_defs.md#multiplevaluessettingtypedef)

Returns a `Coroutine` for
[UpdateSlotResponseTypeDef](./type_defs.md#updateslotresponsetypedef).

<a id="update\_slot\_type"></a>

### update_slot_type

Updates the configuration of an existing slot type.

Type annotations for `session.create_client("lexv2-models").update_slot_type`
method.

Boto3 documentation:
[LexModelsV2.Client.update_slot_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)

Asynchronous method. Use `await update_slot_type(...)` for a synchronous call.

Arguments mapping described in
[UpdateSlotTypeRequestRequestTypeDef](./type_defs.md#updateslottyperequestrequesttypedef).

Keyword-only arguments:

- `slotTypeId`: `str` *(required)*
- `slotTypeName`: `str` *(required)*
- `botId`: `str` *(required)*
- `botVersion`: `str` *(required)*
- `localeId`: `str` *(required)*
- `description`: `str`
- `slotTypeValues`:
  `Sequence`\[[SlotTypeValueTypeDef](./type_defs.md#slottypevaluetypedef)\]
- `valueSelectionSetting`:
  [SlotValueSelectionSettingTypeDef](./type_defs.md#slotvalueselectionsettingtypedef)
- `parentSlotTypeSignature`: `str`
- `externalSourceSetting`:
  [ExternalSourceSettingTypeDef](./type_defs.md#externalsourcesettingtypedef)

Returns a `Coroutine` for
[UpdateSlotTypeResponseTypeDef](./type_defs.md#updateslottyperesponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("lexv2-models").__aenter__` method.

Boto3 documentation:
[LexModelsV2.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [LexModelsV2Client](#lexmodelsv2client).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("lexv2-models").__aexit__` method.

Boto3 documentation:
[LexModelsV2.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("lexv2-models").get_waiter` method
with overloads.

- `client.get_waiter("bot_alias_available")` ->
  [BotAliasAvailableWaiter](./waiters.md#botaliasavailablewaiter)
- `client.get_waiter("bot_available")` ->
  [BotAvailableWaiter](./waiters.md#botavailablewaiter)
- `client.get_waiter("bot_export_completed")` ->
  [BotExportCompletedWaiter](./waiters.md#botexportcompletedwaiter)
- `client.get_waiter("bot_import_completed")` ->
  [BotImportCompletedWaiter](./waiters.md#botimportcompletedwaiter)
- `client.get_waiter("bot_locale_built")` ->
  [BotLocaleBuiltWaiter](./waiters.md#botlocalebuiltwaiter)
- `client.get_waiter("bot_locale_created")` ->
  [BotLocaleCreatedWaiter](./waiters.md#botlocalecreatedwaiter)
- `client.get_waiter("bot_locale_express_testing_available")` ->
  [BotLocaleExpressTestingAvailableWaiter](./waiters.md#botlocaleexpresstestingavailablewaiter)
- `client.get_waiter("bot_version_available")` ->
  [BotVersionAvailableWaiter](./waiters.md#botversionavailablewaiter)

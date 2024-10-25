# SESV2Client

> [Index](../README.md) > [SESV2](./README.md) > SESV2Client

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## SESV2Client

Type annotations and code completion for `#!python session.create_client("sesv2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client)

```python
# SESV2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_sesv2.client import SESV2Client

session = get_session()
async with session.create_client("sesv2") as client:
    client: SESV2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sesv2").exceptions` structure.

```python
# SESV2Client.exceptions usage example

async with session.create_client("sesv2") as client:
    try:
        do_something(client)
    except (
            client.AccountSuspendedException,
        client.AlreadyExistsException,
        client.BadRequestException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.ConflictException,
        client.InternalServiceErrorException,
        client.InvalidNextTokenException,
        client.LimitExceededException,
        client.MailFromDomainNotVerifiedException,
        client.MessageRejected,
        client.NotFoundException,
        client.SendingPausedException,
        client.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# SESV2Client usage type checking example

from types_aiobotocore_sesv2.client import Exceptions

def handle_error(exc: Exceptions.AccountSuspendedException) -> None:
    ...
```


## Methods


### batch\_get\_metric\_data

Retrieves batches of metric data collected based on your sending activity.

Type annotations and code completion for `#!python session.create_client("sesv2").batch_get_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.batch_get_metric_data)

```python
# batch_get_metric_data method definition

await def batch_get_metric_data(
    self,
    *,
    Queries: Sequence[BatchGetMetricDataQueryTypeDef],  # (1)
) -> BatchGetMetricDataResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetMetricDataQueryTypeDef](./type_defs.md#batchgetmetricdataquerytypedef) 
2. See [:material-code-braces: BatchGetMetricDataResponseTypeDef](./type_defs.md#batchgetmetricdataresponsetypedef) 


```python
# batch_get_metric_data method usage example with argument unpacking

kwargs: BatchGetMetricDataRequestRequestTypeDef = {  # (1)
    "Queries": ...,
}

parent.batch_get_metric_data(**kwargs)
```

1. See [:material-code-braces: BatchGetMetricDataRequestRequestTypeDef](./type_defs.md#batchgetmetricdatarequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("sesv2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_export\_job

Cancels an export job.

Type annotations and code completion for `#!python session.create_client("sesv2").cancel_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.cancel_export_job)

```python
# cancel_export_job method definition

await def cancel_export_job(
    self,
    *,
    JobId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_export_job method usage example with argument unpacking

kwargs: CancelExportJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.cancel_export_job(**kwargs)
```

1. See [:material-code-braces: CancelExportJobRequestRequestTypeDef](./type_defs.md#cancelexportjobrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("sesv2").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_configuration\_set

Create a configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").create_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)

```python
# create_configuration_set method definition

await def create_configuration_set(
    self,
    *,
    ConfigurationSetName: str,
    TrackingOptions: TrackingOptionsTypeDef = ...,  # (1)
    DeliveryOptions: DeliveryOptionsTypeDef = ...,  # (2)
    ReputationOptions: ReputationOptionsTypeDef = ...,  # (3)
    SendingOptions: SendingOptionsTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    SuppressionOptions: SuppressionOptionsTypeDef = ...,  # (6)
    VdmOptions: VdmOptionsTypeDef = ...,  # (7)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsTypeDef](./type_defs.md#reputationoptionstypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: SuppressionOptionsTypeDef](./type_defs.md#suppressionoptionstypedef) 
7. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 


```python
# create_configuration_set method usage example with argument unpacking

kwargs: CreateConfigurationSetRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.create_configuration_set(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetRequestRequestTypeDef](./type_defs.md#createconfigurationsetrequestrequesttypedef) 

### create\_configuration\_set\_event\_destination

Create an event destination.

Type annotations and code completion for `#!python session.create_client("sesv2").create_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set_event_destination)

```python
# create_configuration_set_event_destination method definition

await def create_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 


```python
# create_configuration_set_event_destination method usage example with argument unpacking

kwargs: CreateConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
    "EventDestination": ...,
}

parent.create_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#createconfigurationseteventdestinationrequestrequesttypedef) 

### create\_contact

Creates a contact, which is an end-user who is receiving the email, and adds
them to a contact
list.

Type annotations and code completion for `#!python session.create_client("sesv2").create_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_contact)

```python
# create_contact method definition

await def create_contact(
    self,
    *,
    ContactListName: str,
    EmailAddress: str,
    TopicPreferences: Sequence[TopicPreferenceTypeDef] = ...,  # (1)
    UnsubscribeAll: bool = ...,
    AttributesData: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 


```python
# create_contact method usage example with argument unpacking

kwargs: CreateContactRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.create_contact(**kwargs)
```

1. See [:material-code-braces: CreateContactRequestRequestTypeDef](./type_defs.md#createcontactrequestrequesttypedef) 

### create\_contact\_list

Creates a contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").create_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_contact_list)

```python
# create_contact_list method definition

await def create_contact_list(
    self,
    *,
    ContactListName: str,
    Topics: Sequence[TopicTypeDef] = ...,  # (1)
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_contact_list method usage example with argument unpacking

kwargs: CreateContactListRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.create_contact_list(**kwargs)
```

1. See [:material-code-braces: CreateContactListRequestRequestTypeDef](./type_defs.md#createcontactlistrequestrequesttypedef) 

### create\_custom\_verification\_email\_template

Creates a new custom verification email template.

Type annotations and code completion for `#!python session.create_client("sesv2").create_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_custom_verification_email_template)

```python
# create_custom_verification_email_template method definition

await def create_custom_verification_email_template(
    self,
    *,
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
) -> Dict[str, Any]:
    ...
```



```python
# create_custom_verification_email_template method usage example with argument unpacking

kwargs: CreateCustomVerificationEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "FromEmailAddress": ...,
    "TemplateSubject": ...,
    "TemplateContent": ...,
    "SuccessRedirectionURL": ...,
    "FailureRedirectionURL": ...,
}

parent.create_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: CreateCustomVerificationEmailTemplateRequestRequestTypeDef](./type_defs.md#createcustomverificationemailtemplaterequestrequesttypedef) 

### create\_dedicated\_ip\_pool

Create a new pool of dedicated IP addresses.

Type annotations and code completion for `#!python session.create_client("sesv2").create_dedicated_ip_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_dedicated_ip_pool)

```python
# create_dedicated_ip_pool method definition

await def create_dedicated_ip_pool(
    self,
    *,
    PoolName: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    ScalingMode: ScalingModeType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 


```python
# create_dedicated_ip_pool method usage example with argument unpacking

kwargs: CreateDedicatedIpPoolRequestRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.create_dedicated_ip_pool(**kwargs)
```

1. See [:material-code-braces: CreateDedicatedIpPoolRequestRequestTypeDef](./type_defs.md#creatededicatedippoolrequestrequesttypedef) 

### create\_deliverability\_test\_report

Create a new predictive inbox placement test.

Type annotations and code completion for `#!python session.create_client("sesv2").create_deliverability_test_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_deliverability_test_report)

```python
# create_deliverability_test_report method definition

await def create_deliverability_test_report(
    self,
    *,
    FromEmailAddress: str,
    Content: EmailContentTypeDef,  # (1)
    ReportName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDeliverabilityTestReportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDeliverabilityTestReportResponseTypeDef](./type_defs.md#createdeliverabilitytestreportresponsetypedef) 


```python
# create_deliverability_test_report method usage example with argument unpacking

kwargs: CreateDeliverabilityTestReportRequestRequestTypeDef = {  # (1)
    "FromEmailAddress": ...,
    "Content": ...,
}

parent.create_deliverability_test_report(**kwargs)
```

1. See [:material-code-braces: CreateDeliverabilityTestReportRequestRequestTypeDef](./type_defs.md#createdeliverabilitytestreportrequestrequesttypedef) 

### create\_email\_identity

Starts the process of verifying an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").create_email_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_email_identity)

```python
# create_email_identity method definition

await def create_email_identity(
    self,
    *,
    EmailIdentity: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    DkimSigningAttributes: DkimSigningAttributesTypeDef = ...,  # (2)
    ConfigurationSetName: str = ...,
) -> CreateEmailIdentityResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: DkimSigningAttributesTypeDef](./type_defs.md#dkimsigningattributestypedef) 
3. See [:material-code-braces: CreateEmailIdentityResponseTypeDef](./type_defs.md#createemailidentityresponsetypedef) 


```python
# create_email_identity method usage example with argument unpacking

kwargs: CreateEmailIdentityRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.create_email_identity(**kwargs)
```

1. See [:material-code-braces: CreateEmailIdentityRequestRequestTypeDef](./type_defs.md#createemailidentityrequestrequesttypedef) 

### create\_email\_identity\_policy

Creates the specified sending authorization policy for the given identity (an
email address or a
domain).

Type annotations and code completion for `#!python session.create_client("sesv2").create_email_identity_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_email_identity_policy)

```python
# create_email_identity_policy method definition

await def create_email_identity_policy(
    self,
    *,
    EmailIdentity: str,
    PolicyName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# create_email_identity_policy method usage example with argument unpacking

kwargs: CreateEmailIdentityPolicyRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "PolicyName": ...,
    "Policy": ...,
}

parent.create_email_identity_policy(**kwargs)
```

1. See [:material-code-braces: CreateEmailIdentityPolicyRequestRequestTypeDef](./type_defs.md#createemailidentitypolicyrequestrequesttypedef) 

### create\_email\_template

Creates an email template.

Type annotations and code completion for `#!python session.create_client("sesv2").create_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_email_template)

```python
# create_email_template method definition

await def create_email_template(
    self,
    *,
    TemplateName: str,
    TemplateContent: EmailTemplateContentTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 


```python
# create_email_template method usage example with argument unpacking

kwargs: CreateEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "TemplateContent": ...,
}

parent.create_email_template(**kwargs)
```

1. See [:material-code-braces: CreateEmailTemplateRequestRequestTypeDef](./type_defs.md#createemailtemplaterequestrequesttypedef) 

### create\_export\_job

Creates an export job for a data source and destination.

Type annotations and code completion for `#!python session.create_client("sesv2").create_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_export_job)

```python
# create_export_job method definition

await def create_export_job(
    self,
    *,
    ExportDataSource: ExportDataSourceTypeDef,  # (1)
    ExportDestination: ExportDestinationTypeDef,  # (2)
) -> CreateExportJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExportDataSourceTypeDef](./type_defs.md#exportdatasourcetypedef) 
2. See [:material-code-braces: ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef) 
3. See [:material-code-braces: CreateExportJobResponseTypeDef](./type_defs.md#createexportjobresponsetypedef) 


```python
# create_export_job method usage example with argument unpacking

kwargs: CreateExportJobRequestRequestTypeDef = {  # (1)
    "ExportDataSource": ...,
    "ExportDestination": ...,
}

parent.create_export_job(**kwargs)
```

1. See [:material-code-braces: CreateExportJobRequestRequestTypeDef](./type_defs.md#createexportjobrequestrequesttypedef) 

### create\_import\_job

Creates an import job for a data destination.

Type annotations and code completion for `#!python session.create_client("sesv2").create_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_import_job)

```python
# create_import_job method definition

await def create_import_job(
    self,
    *,
    ImportDestination: ImportDestinationTypeDef,  # (1)
    ImportDataSource: ImportDataSourceTypeDef,  # (2)
) -> CreateImportJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ImportDestinationTypeDef](./type_defs.md#importdestinationtypedef) 
2. See [:material-code-braces: ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef) 
3. See [:material-code-braces: CreateImportJobResponseTypeDef](./type_defs.md#createimportjobresponsetypedef) 


```python
# create_import_job method usage example with argument unpacking

kwargs: CreateImportJobRequestRequestTypeDef = {  # (1)
    "ImportDestination": ...,
    "ImportDataSource": ...,
}

parent.create_import_job(**kwargs)
```

1. See [:material-code-braces: CreateImportJobRequestRequestTypeDef](./type_defs.md#createimportjobrequestrequesttypedef) 

### delete\_configuration\_set

Delete an existing configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_configuration_set)

```python
# delete_configuration_set method definition

await def delete_configuration_set(
    self,
    *,
    ConfigurationSetName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_configuration_set method usage example with argument unpacking

kwargs: DeleteConfigurationSetRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.delete_configuration_set(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetRequestRequestTypeDef](./type_defs.md#deleteconfigurationsetrequestrequesttypedef) 

### delete\_configuration\_set\_event\_destination

Delete an event destination.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_configuration_set_event_destination)

```python
# delete_configuration_set_event_destination method definition

await def delete_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestinationName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_configuration_set_event_destination method usage example with argument unpacking

kwargs: DeleteConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
}

parent.delete_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#deleteconfigurationseteventdestinationrequestrequesttypedef) 

### delete\_contact

Removes a contact from a contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_contact)

```python
# delete_contact method definition

await def delete_contact(
    self,
    *,
    ContactListName: str,
    EmailAddress: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_contact method usage example with argument unpacking

kwargs: DeleteContactRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.delete_contact(**kwargs)
```

1. See [:material-code-braces: DeleteContactRequestRequestTypeDef](./type_defs.md#deletecontactrequestrequesttypedef) 

### delete\_contact\_list

Deletes a contact list and all of the contacts on that list.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_contact_list)

```python
# delete_contact_list method definition

await def delete_contact_list(
    self,
    *,
    ContactListName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_contact_list method usage example with argument unpacking

kwargs: DeleteContactListRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.delete_contact_list(**kwargs)
```

1. See [:material-code-braces: DeleteContactListRequestRequestTypeDef](./type_defs.md#deletecontactlistrequestrequesttypedef) 

### delete\_custom\_verification\_email\_template

Deletes an existing custom verification email template.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_custom_verification_email_template)

```python
# delete_custom_verification_email_template method definition

await def delete_custom_verification_email_template(
    self,
    *,
    TemplateName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_custom_verification_email_template method usage example with argument unpacking

kwargs: DeleteCustomVerificationEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.delete_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: DeleteCustomVerificationEmailTemplateRequestRequestTypeDef](./type_defs.md#deletecustomverificationemailtemplaterequestrequesttypedef) 

### delete\_dedicated\_ip\_pool

Delete a dedicated IP pool.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_dedicated_ip_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_dedicated_ip_pool)

```python
# delete_dedicated_ip_pool method definition

await def delete_dedicated_ip_pool(
    self,
    *,
    PoolName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_dedicated_ip_pool method usage example with argument unpacking

kwargs: DeleteDedicatedIpPoolRequestRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.delete_dedicated_ip_pool(**kwargs)
```

1. See [:material-code-braces: DeleteDedicatedIpPoolRequestRequestTypeDef](./type_defs.md#deletededicatedippoolrequestrequesttypedef) 

### delete\_email\_identity

Deletes an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_email_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_email_identity)

```python
# delete_email_identity method definition

await def delete_email_identity(
    self,
    *,
    EmailIdentity: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_email_identity method usage example with argument unpacking

kwargs: DeleteEmailIdentityRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.delete_email_identity(**kwargs)
```

1. See [:material-code-braces: DeleteEmailIdentityRequestRequestTypeDef](./type_defs.md#deleteemailidentityrequestrequesttypedef) 

### delete\_email\_identity\_policy

Deletes the specified sending authorization policy for the given identity (an
email address or a
domain).

Type annotations and code completion for `#!python session.create_client("sesv2").delete_email_identity_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_email_identity_policy)

```python
# delete_email_identity_policy method definition

await def delete_email_identity_policy(
    self,
    *,
    EmailIdentity: str,
    PolicyName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_email_identity_policy method usage example with argument unpacking

kwargs: DeleteEmailIdentityPolicyRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "PolicyName": ...,
}

parent.delete_email_identity_policy(**kwargs)
```

1. See [:material-code-braces: DeleteEmailIdentityPolicyRequestRequestTypeDef](./type_defs.md#deleteemailidentitypolicyrequestrequesttypedef) 

### delete\_email\_template

Deletes an email template.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_email_template)

```python
# delete_email_template method definition

await def delete_email_template(
    self,
    *,
    TemplateName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_email_template method usage example with argument unpacking

kwargs: DeleteEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.delete_email_template(**kwargs)
```

1. See [:material-code-braces: DeleteEmailTemplateRequestRequestTypeDef](./type_defs.md#deleteemailtemplaterequestrequesttypedef) 

### delete\_suppressed\_destination

Removes an email address from the suppression list for your account.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_suppressed_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.delete_suppressed_destination)

```python
# delete_suppressed_destination method definition

await def delete_suppressed_destination(
    self,
    *,
    EmailAddress: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_suppressed_destination method usage example with argument unpacking

kwargs: DeleteSuppressedDestinationRequestRequestTypeDef = {  # (1)
    "EmailAddress": ...,
}

parent.delete_suppressed_destination(**kwargs)
```

1. See [:material-code-braces: DeleteSuppressedDestinationRequestRequestTypeDef](./type_defs.md#deletesuppresseddestinationrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("sesv2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.generate_presigned_url)

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


### get\_account

Obtain information about the email-sending status and capabilities of your
Amazon SES account in the current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("sesv2").get_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_account)

```python
# get_account method definition

await def get_account(
    self,
) -> GetAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountResponseTypeDef](./type_defs.md#getaccountresponsetypedef) 

### get\_blacklist\_reports

Retrieve a list of the blacklists that your dedicated IP addresses appear on.

Type annotations and code completion for `#!python session.create_client("sesv2").get_blacklist_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_blacklist_reports)

```python
# get_blacklist_reports method definition

await def get_blacklist_reports(
    self,
    *,
    BlacklistItemNames: Sequence[str],
) -> GetBlacklistReportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBlacklistReportsResponseTypeDef](./type_defs.md#getblacklistreportsresponsetypedef) 


```python
# get_blacklist_reports method usage example with argument unpacking

kwargs: GetBlacklistReportsRequestRequestTypeDef = {  # (1)
    "BlacklistItemNames": ...,
}

parent.get_blacklist_reports(**kwargs)
```

1. See [:material-code-braces: GetBlacklistReportsRequestRequestTypeDef](./type_defs.md#getblacklistreportsrequestrequesttypedef) 

### get\_configuration\_set

Get information about an existing configuration set, including the dedicated IP
pool that it's associated with, whether or not it's enabled for sending email,
and
more.

Type annotations and code completion for `#!python session.create_client("sesv2").get_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_configuration_set)

```python
# get_configuration_set method definition

await def get_configuration_set(
    self,
    *,
    ConfigurationSetName: str,
) -> GetConfigurationSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfigurationSetResponseTypeDef](./type_defs.md#getconfigurationsetresponsetypedef) 


```python
# get_configuration_set method usage example with argument unpacking

kwargs: GetConfigurationSetRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.get_configuration_set(**kwargs)
```

1. See [:material-code-braces: GetConfigurationSetRequestRequestTypeDef](./type_defs.md#getconfigurationsetrequestrequesttypedef) 

### get\_configuration\_set\_event\_destinations

Retrieve a list of event destinations that are associated with a configuration
set.

Type annotations and code completion for `#!python session.create_client("sesv2").get_configuration_set_event_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_configuration_set_event_destinations)

```python
# get_configuration_set_event_destinations method definition

await def get_configuration_set_event_destinations(
    self,
    *,
    ConfigurationSetName: str,
) -> GetConfigurationSetEventDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef) 


```python
# get_configuration_set_event_destinations method usage example with argument unpacking

kwargs: GetConfigurationSetEventDestinationsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.get_configuration_set_event_destinations(**kwargs)
```

1. See [:material-code-braces: GetConfigurationSetEventDestinationsRequestRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequestrequesttypedef) 

### get\_contact

Returns a contact from a contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").get_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_contact)

```python
# get_contact method definition

await def get_contact(
    self,
    *,
    ContactListName: str,
    EmailAddress: str,
) -> GetContactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactResponseTypeDef](./type_defs.md#getcontactresponsetypedef) 


```python
# get_contact method usage example with argument unpacking

kwargs: GetContactRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.get_contact(**kwargs)
```

1. See [:material-code-braces: GetContactRequestRequestTypeDef](./type_defs.md#getcontactrequestrequesttypedef) 

### get\_contact\_list

Returns contact list metadata.

Type annotations and code completion for `#!python session.create_client("sesv2").get_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_contact_list)

```python
# get_contact_list method definition

await def get_contact_list(
    self,
    *,
    ContactListName: str,
) -> GetContactListResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactListResponseTypeDef](./type_defs.md#getcontactlistresponsetypedef) 


```python
# get_contact_list method usage example with argument unpacking

kwargs: GetContactListRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.get_contact_list(**kwargs)
```

1. See [:material-code-braces: GetContactListRequestRequestTypeDef](./type_defs.md#getcontactlistrequestrequesttypedef) 

### get\_custom\_verification\_email\_template

Returns the custom email verification template for the template name you
specify.

Type annotations and code completion for `#!python session.create_client("sesv2").get_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_custom_verification_email_template)

```python
# get_custom_verification_email_template method definition

await def get_custom_verification_email_template(
    self,
    *,
    TemplateName: str,
) -> GetCustomVerificationEmailTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCustomVerificationEmailTemplateResponseTypeDef](./type_defs.md#getcustomverificationemailtemplateresponsetypedef) 


```python
# get_custom_verification_email_template method usage example with argument unpacking

kwargs: GetCustomVerificationEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.get_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: GetCustomVerificationEmailTemplateRequestRequestTypeDef](./type_defs.md#getcustomverificationemailtemplaterequestrequesttypedef) 

### get\_dedicated\_ip

Get information about a dedicated IP address, including the name of the
dedicated IP pool that it's associated with, as well information about the
automatic warm-up process for the
address.

Type annotations and code completion for `#!python session.create_client("sesv2").get_dedicated_ip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_dedicated_ip)

```python
# get_dedicated_ip method definition

await def get_dedicated_ip(
    self,
    *,
    Ip: str,
) -> GetDedicatedIpResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDedicatedIpResponseTypeDef](./type_defs.md#getdedicatedipresponsetypedef) 


```python
# get_dedicated_ip method usage example with argument unpacking

kwargs: GetDedicatedIpRequestRequestTypeDef = {  # (1)
    "Ip": ...,
}

parent.get_dedicated_ip(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpRequestRequestTypeDef](./type_defs.md#getdedicatediprequestrequesttypedef) 

### get\_dedicated\_ip\_pool

Retrieve information about the dedicated pool.

Type annotations and code completion for `#!python session.create_client("sesv2").get_dedicated_ip_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_dedicated_ip_pool)

```python
# get_dedicated_ip_pool method definition

await def get_dedicated_ip_pool(
    self,
    *,
    PoolName: str,
) -> GetDedicatedIpPoolResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDedicatedIpPoolResponseTypeDef](./type_defs.md#getdedicatedippoolresponsetypedef) 


```python
# get_dedicated_ip_pool method usage example with argument unpacking

kwargs: GetDedicatedIpPoolRequestRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.get_dedicated_ip_pool(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpPoolRequestRequestTypeDef](./type_defs.md#getdedicatedippoolrequestrequesttypedef) 

### get\_dedicated\_ips

List the dedicated IP addresses that are associated with your Amazon Web
Services
account.

Type annotations and code completion for `#!python session.create_client("sesv2").get_dedicated_ips` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_dedicated_ips)

```python
# get_dedicated_ips method definition

await def get_dedicated_ips(
    self,
    *,
    PoolName: str = ...,
    NextToken: str = ...,
    PageSize: int = ...,
) -> GetDedicatedIpsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef) 


```python
# get_dedicated_ips method usage example with argument unpacking

kwargs: GetDedicatedIpsRequestRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.get_dedicated_ips(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpsRequestRequestTypeDef](./type_defs.md#getdedicatedipsrequestrequesttypedef) 

### get\_deliverability\_dashboard\_options

Retrieve information about the status of the Deliverability dashboard for your
account.

Type annotations and code completion for `#!python session.create_client("sesv2").get_deliverability_dashboard_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_deliverability_dashboard_options)

```python
# get_deliverability_dashboard_options method definition

await def get_deliverability_dashboard_options(
    self,
) -> GetDeliverabilityDashboardOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeliverabilityDashboardOptionsResponseTypeDef](./type_defs.md#getdeliverabilitydashboardoptionsresponsetypedef) 

### get\_deliverability\_test\_report

Retrieve the results of a predictive inbox placement test.

Type annotations and code completion for `#!python session.create_client("sesv2").get_deliverability_test_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_deliverability_test_report)

```python
# get_deliverability_test_report method definition

await def get_deliverability_test_report(
    self,
    *,
    ReportId: str,
) -> GetDeliverabilityTestReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeliverabilityTestReportResponseTypeDef](./type_defs.md#getdeliverabilitytestreportresponsetypedef) 


```python
# get_deliverability_test_report method usage example with argument unpacking

kwargs: GetDeliverabilityTestReportRequestRequestTypeDef = {  # (1)
    "ReportId": ...,
}

parent.get_deliverability_test_report(**kwargs)
```

1. See [:material-code-braces: GetDeliverabilityTestReportRequestRequestTypeDef](./type_defs.md#getdeliverabilitytestreportrequestrequesttypedef) 

### get\_domain\_deliverability\_campaign

Retrieve all the deliverability data for a specific campaign.

Type annotations and code completion for `#!python session.create_client("sesv2").get_domain_deliverability_campaign` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_deliverability_campaign)

```python
# get_domain_deliverability_campaign method definition

await def get_domain_deliverability_campaign(
    self,
    *,
    CampaignId: str,
) -> GetDomainDeliverabilityCampaignResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainDeliverabilityCampaignResponseTypeDef](./type_defs.md#getdomaindeliverabilitycampaignresponsetypedef) 


```python
# get_domain_deliverability_campaign method usage example with argument unpacking

kwargs: GetDomainDeliverabilityCampaignRequestRequestTypeDef = {  # (1)
    "CampaignId": ...,
}

parent.get_domain_deliverability_campaign(**kwargs)
```

1. See [:material-code-braces: GetDomainDeliverabilityCampaignRequestRequestTypeDef](./type_defs.md#getdomaindeliverabilitycampaignrequestrequesttypedef) 

### get\_domain\_statistics\_report

Retrieve inbox placement and engagement rates for the domains that you use to
send
email.

Type annotations and code completion for `#!python session.create_client("sesv2").get_domain_statistics_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_statistics_report)

```python
# get_domain_statistics_report method definition

await def get_domain_statistics_report(
    self,
    *,
    Domain: str,
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
) -> GetDomainStatisticsReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainStatisticsReportResponseTypeDef](./type_defs.md#getdomainstatisticsreportresponsetypedef) 


```python
# get_domain_statistics_report method usage example with argument unpacking

kwargs: GetDomainStatisticsReportRequestRequestTypeDef = {  # (1)
    "Domain": ...,
    "StartDate": ...,
    "EndDate": ...,
}

parent.get_domain_statistics_report(**kwargs)
```

1. See [:material-code-braces: GetDomainStatisticsReportRequestRequestTypeDef](./type_defs.md#getdomainstatisticsreportrequestrequesttypedef) 

### get\_email\_identity

Provides information about a specific identity, including the identity's
verification status, sending authorization policies, its DKIM authentication
status, and its custom Mail-From
settings.

Type annotations and code completion for `#!python session.create_client("sesv2").get_email_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_email_identity)

```python
# get_email_identity method definition

await def get_email_identity(
    self,
    *,
    EmailIdentity: str,
) -> GetEmailIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEmailIdentityResponseTypeDef](./type_defs.md#getemailidentityresponsetypedef) 


```python
# get_email_identity method usage example with argument unpacking

kwargs: GetEmailIdentityRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.get_email_identity(**kwargs)
```

1. See [:material-code-braces: GetEmailIdentityRequestRequestTypeDef](./type_defs.md#getemailidentityrequestrequesttypedef) 

### get\_email\_identity\_policies

Returns the requested sending authorization policies for the given identity (an
email address or a
domain).

Type annotations and code completion for `#!python session.create_client("sesv2").get_email_identity_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_email_identity_policies)

```python
# get_email_identity_policies method definition

await def get_email_identity_policies(
    self,
    *,
    EmailIdentity: str,
) -> GetEmailIdentityPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEmailIdentityPoliciesResponseTypeDef](./type_defs.md#getemailidentitypoliciesresponsetypedef) 


```python
# get_email_identity_policies method usage example with argument unpacking

kwargs: GetEmailIdentityPoliciesRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.get_email_identity_policies(**kwargs)
```

1. See [:material-code-braces: GetEmailIdentityPoliciesRequestRequestTypeDef](./type_defs.md#getemailidentitypoliciesrequestrequesttypedef) 

### get\_email\_template

Displays the template object (which includes the subject line, HTML part and
text part) for the template you
specify.

Type annotations and code completion for `#!python session.create_client("sesv2").get_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_email_template)

```python
# get_email_template method definition

await def get_email_template(
    self,
    *,
    TemplateName: str,
) -> GetEmailTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEmailTemplateResponseTypeDef](./type_defs.md#getemailtemplateresponsetypedef) 


```python
# get_email_template method usage example with argument unpacking

kwargs: GetEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.get_email_template(**kwargs)
```

1. See [:material-code-braces: GetEmailTemplateRequestRequestTypeDef](./type_defs.md#getemailtemplaterequestrequesttypedef) 

### get\_export\_job

Provides information about an export job.

Type annotations and code completion for `#!python session.create_client("sesv2").get_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_export_job)

```python
# get_export_job method definition

await def get_export_job(
    self,
    *,
    JobId: str,
) -> GetExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExportJobResponseTypeDef](./type_defs.md#getexportjobresponsetypedef) 


```python
# get_export_job method usage example with argument unpacking

kwargs: GetExportJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_export_job(**kwargs)
```

1. See [:material-code-braces: GetExportJobRequestRequestTypeDef](./type_defs.md#getexportjobrequestrequesttypedef) 

### get\_import\_job

Provides information about an import job.

Type annotations and code completion for `#!python session.create_client("sesv2").get_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_import_job)

```python
# get_import_job method definition

await def get_import_job(
    self,
    *,
    JobId: str,
) -> GetImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImportJobResponseTypeDef](./type_defs.md#getimportjobresponsetypedef) 


```python
# get_import_job method usage example with argument unpacking

kwargs: GetImportJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_import_job(**kwargs)
```

1. See [:material-code-braces: GetImportJobRequestRequestTypeDef](./type_defs.md#getimportjobrequestrequesttypedef) 

### get\_message\_insights

Provides information about a specific message, including the from address, the
subject, the recipient address, email tags, as well as events associated with
the
message.

Type annotations and code completion for `#!python session.create_client("sesv2").get_message_insights` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_message_insights)

```python
# get_message_insights method definition

await def get_message_insights(
    self,
    *,
    MessageId: str,
) -> GetMessageInsightsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMessageInsightsResponseTypeDef](./type_defs.md#getmessageinsightsresponsetypedef) 


```python
# get_message_insights method usage example with argument unpacking

kwargs: GetMessageInsightsRequestRequestTypeDef = {  # (1)
    "MessageId": ...,
}

parent.get_message_insights(**kwargs)
```

1. See [:material-code-braces: GetMessageInsightsRequestRequestTypeDef](./type_defs.md#getmessageinsightsrequestrequesttypedef) 

### get\_suppressed\_destination

Retrieves information about a specific email address that's on the suppression
list for your
account.

Type annotations and code completion for `#!python session.create_client("sesv2").get_suppressed_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_suppressed_destination)

```python
# get_suppressed_destination method definition

await def get_suppressed_destination(
    self,
    *,
    EmailAddress: str,
) -> GetSuppressedDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSuppressedDestinationResponseTypeDef](./type_defs.md#getsuppresseddestinationresponsetypedef) 


```python
# get_suppressed_destination method usage example with argument unpacking

kwargs: GetSuppressedDestinationRequestRequestTypeDef = {  # (1)
    "EmailAddress": ...,
}

parent.get_suppressed_destination(**kwargs)
```

1. See [:material-code-braces: GetSuppressedDestinationRequestRequestTypeDef](./type_defs.md#getsuppresseddestinationrequestrequesttypedef) 

### list\_configuration\_sets

List all of the configuration sets associated with your account in the current
region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_configuration_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_configuration_sets)

```python
# list_configuration_sets method definition

await def list_configuration_sets(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListConfigurationSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef) 


```python
# list_configuration_sets method usage example with argument unpacking

kwargs: ListConfigurationSetsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_configuration_sets(**kwargs)
```

1. See [:material-code-braces: ListConfigurationSetsRequestRequestTypeDef](./type_defs.md#listconfigurationsetsrequestrequesttypedef) 

### list\_contact\_lists

Lists all of the contact lists available.

Type annotations and code completion for `#!python session.create_client("sesv2").list_contact_lists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_contact_lists)

```python
# list_contact_lists method definition

await def list_contact_lists(
    self,
    *,
    PageSize: int = ...,
    NextToken: str = ...,
) -> ListContactListsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContactListsResponseTypeDef](./type_defs.md#listcontactlistsresponsetypedef) 


```python
# list_contact_lists method usage example with argument unpacking

kwargs: ListContactListsRequestRequestTypeDef = {  # (1)
    "PageSize": ...,
}

parent.list_contact_lists(**kwargs)
```

1. See [:material-code-braces: ListContactListsRequestRequestTypeDef](./type_defs.md#listcontactlistsrequestrequesttypedef) 

### list\_contacts

Lists the contacts present in a specific contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").list_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_contacts)

```python
# list_contacts method definition

await def list_contacts(
    self,
    *,
    ContactListName: str,
    Filter: ListContactsFilterTypeDef = ...,  # (1)
    PageSize: int = ...,
    NextToken: str = ...,
) -> ListContactsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListContactsFilterTypeDef](./type_defs.md#listcontactsfiltertypedef) 
2. See [:material-code-braces: ListContactsResponseTypeDef](./type_defs.md#listcontactsresponsetypedef) 


```python
# list_contacts method usage example with argument unpacking

kwargs: ListContactsRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.list_contacts(**kwargs)
```

1. See [:material-code-braces: ListContactsRequestRequestTypeDef](./type_defs.md#listcontactsrequestrequesttypedef) 

### list\_custom\_verification\_email\_templates

Lists the existing custom verification email templates for your account in the
current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_custom_verification_email_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_custom_verification_email_templates)

```python
# list_custom_verification_email_templates method definition

await def list_custom_verification_email_templates(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListCustomVerificationEmailTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomVerificationEmailTemplatesResponseTypeDef](./type_defs.md#listcustomverificationemailtemplatesresponsetypedef) 


```python
# list_custom_verification_email_templates method usage example with argument unpacking

kwargs: ListCustomVerificationEmailTemplatesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_custom_verification_email_templates(**kwargs)
```

1. See [:material-code-braces: ListCustomVerificationEmailTemplatesRequestRequestTypeDef](./type_defs.md#listcustomverificationemailtemplatesrequestrequesttypedef) 

### list\_dedicated\_ip\_pools

List all of the dedicated IP pools that exist in your Amazon Web Services
account in the current
Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_dedicated_ip_pools` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_dedicated_ip_pools)

```python
# list_dedicated_ip_pools method definition

await def list_dedicated_ip_pools(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListDedicatedIpPoolsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDedicatedIpPoolsResponseTypeDef](./type_defs.md#listdedicatedippoolsresponsetypedef) 


```python
# list_dedicated_ip_pools method usage example with argument unpacking

kwargs: ListDedicatedIpPoolsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_dedicated_ip_pools(**kwargs)
```

1. See [:material-code-braces: ListDedicatedIpPoolsRequestRequestTypeDef](./type_defs.md#listdedicatedippoolsrequestrequesttypedef) 

### list\_deliverability\_test\_reports

Show a list of the predictive inbox placement tests that you've performed,
regardless of their
statuses.

Type annotations and code completion for `#!python session.create_client("sesv2").list_deliverability_test_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_deliverability_test_reports)

```python
# list_deliverability_test_reports method definition

await def list_deliverability_test_reports(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListDeliverabilityTestReportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeliverabilityTestReportsResponseTypeDef](./type_defs.md#listdeliverabilitytestreportsresponsetypedef) 


```python
# list_deliverability_test_reports method usage example with argument unpacking

kwargs: ListDeliverabilityTestReportsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_deliverability_test_reports(**kwargs)
```

1. See [:material-code-braces: ListDeliverabilityTestReportsRequestRequestTypeDef](./type_defs.md#listdeliverabilitytestreportsrequestrequesttypedef) 

### list\_domain\_deliverability\_campaigns

Retrieve deliverability data for all the campaigns that used a specific domain
to send email during a specified time
range.

Type annotations and code completion for `#!python session.create_client("sesv2").list_domain_deliverability_campaigns` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_domain_deliverability_campaigns)

```python
# list_domain_deliverability_campaigns method definition

await def list_domain_deliverability_campaigns(
    self,
    *,
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
    SubscribedDomain: str,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListDomainDeliverabilityCampaignsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainDeliverabilityCampaignsResponseTypeDef](./type_defs.md#listdomaindeliverabilitycampaignsresponsetypedef) 


```python
# list_domain_deliverability_campaigns method usage example with argument unpacking

kwargs: ListDomainDeliverabilityCampaignsRequestRequestTypeDef = {  # (1)
    "StartDate": ...,
    "EndDate": ...,
    "SubscribedDomain": ...,
}

parent.list_domain_deliverability_campaigns(**kwargs)
```

1. See [:material-code-braces: ListDomainDeliverabilityCampaignsRequestRequestTypeDef](./type_defs.md#listdomaindeliverabilitycampaignsrequestrequesttypedef) 

### list\_email\_identities

Returns a list of all of the email identities that are associated with your
Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("sesv2").list_email_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_email_identities)

```python
# list_email_identities method definition

await def list_email_identities(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListEmailIdentitiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEmailIdentitiesResponseTypeDef](./type_defs.md#listemailidentitiesresponsetypedef) 


```python
# list_email_identities method usage example with argument unpacking

kwargs: ListEmailIdentitiesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_email_identities(**kwargs)
```

1. See [:material-code-braces: ListEmailIdentitiesRequestRequestTypeDef](./type_defs.md#listemailidentitiesrequestrequesttypedef) 

### list\_email\_templates

Lists the email templates present in your Amazon SES account in the current
Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_email_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_email_templates)

```python
# list_email_templates method definition

await def list_email_templates(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListEmailTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEmailTemplatesResponseTypeDef](./type_defs.md#listemailtemplatesresponsetypedef) 


```python
# list_email_templates method usage example with argument unpacking

kwargs: ListEmailTemplatesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_email_templates(**kwargs)
```

1. See [:material-code-braces: ListEmailTemplatesRequestRequestTypeDef](./type_defs.md#listemailtemplatesrequestrequesttypedef) 

### list\_export\_jobs

Lists all of the export jobs.

Type annotations and code completion for `#!python session.create_client("sesv2").list_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_export_jobs)

```python
# list_export_jobs method definition

await def list_export_jobs(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
    ExportSourceType: ExportSourceTypeType = ...,  # (1)
    JobStatus: JobStatusType = ...,  # (2)
) -> ListExportJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: ListExportJobsResponseTypeDef](./type_defs.md#listexportjobsresponsetypedef) 


```python
# list_export_jobs method usage example with argument unpacking

kwargs: ListExportJobsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListExportJobsRequestRequestTypeDef](./type_defs.md#listexportjobsrequestrequesttypedef) 

### list\_import\_jobs

Lists all of the import jobs.

Type annotations and code completion for `#!python session.create_client("sesv2").list_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_import_jobs)

```python
# list_import_jobs method definition

await def list_import_jobs(
    self,
    *,
    ImportDestinationType: ImportDestinationTypeType = ...,  # (1)
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListImportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ImportDestinationTypeType](./literals.md#importdestinationtypetype) 
2. See [:material-code-braces: ListImportJobsResponseTypeDef](./type_defs.md#listimportjobsresponsetypedef) 


```python
# list_import_jobs method usage example with argument unpacking

kwargs: ListImportJobsRequestRequestTypeDef = {  # (1)
    "ImportDestinationType": ...,
}

parent.list_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListImportJobsRequestRequestTypeDef](./type_defs.md#listimportjobsrequestrequesttypedef) 

### list\_recommendations

Lists the recommendations present in your Amazon SES account in the current
Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_recommendations)

```python
# list_recommendations method definition

await def list_recommendations(
    self,
    *,
    Filter: Mapping[ListRecommendationsFilterKeyType, str] = ...,  # (1)
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListRecommendationsFilterKeyType](./literals.md#listrecommendationsfilterkeytype) 
2. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


```python
# list_recommendations method usage example with argument unpacking

kwargs: ListRecommendationsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_recommendations(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef) 

### list\_suppressed\_destinations

Retrieves a list of email addresses that are on the suppression list for your
account.

Type annotations and code completion for `#!python session.create_client("sesv2").list_suppressed_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_suppressed_destinations)

```python
# list_suppressed_destinations method definition

await def list_suppressed_destinations(
    self,
    *,
    Reasons: Sequence[SuppressionListReasonType] = ...,  # (1)
    StartDate: TimestampTypeDef = ...,
    EndDate: TimestampTypeDef = ...,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListSuppressedDestinationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
2. See [:material-code-braces: ListSuppressedDestinationsResponseTypeDef](./type_defs.md#listsuppresseddestinationsresponsetypedef) 


```python
# list_suppressed_destinations method usage example with argument unpacking

kwargs: ListSuppressedDestinationsRequestRequestTypeDef = {  # (1)
    "Reasons": ...,
}

parent.list_suppressed_destinations(**kwargs)
```

1. See [:material-code-braces: ListSuppressedDestinationsRequestRequestTypeDef](./type_defs.md#listsuppresseddestinationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieve a list of the tags (keys and values) that are associated with a
specified
resource.

Type annotations and code completion for `#!python session.create_client("sesv2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_tags_for_resource)

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

### put\_account\_dedicated\_ip\_warmup\_attributes

Enable or disable the automatic warm-up feature for dedicated IP addresses.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_dedicated_ip_warmup_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_account_dedicated_ip_warmup_attributes)

```python
# put_account_dedicated_ip_warmup_attributes method definition

await def put_account_dedicated_ip_warmup_attributes(
    self,
    *,
    AutoWarmupEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_account_dedicated_ip_warmup_attributes method usage example with argument unpacking

kwargs: PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef = {  # (1)
    "AutoWarmupEnabled": ...,
}

parent.put_account_dedicated_ip_warmup_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef](./type_defs.md#putaccountdedicatedipwarmupattributesrequestrequesttypedef) 

### put\_account\_details

Update your Amazon SES account details.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_account_details)

```python
# put_account_details method definition

await def put_account_details(
    self,
    *,
    MailType: MailTypeType,  # (1)
    WebsiteURL: str,
    ContactLanguage: ContactLanguageType = ...,  # (2)
    UseCaseDescription: str = ...,
    AdditionalContactEmailAddresses: Sequence[str] = ...,
    ProductionAccessEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MailTypeType](./literals.md#mailtypetype) 
2. See [:material-code-brackets: ContactLanguageType](./literals.md#contactlanguagetype) 


```python
# put_account_details method usage example with argument unpacking

kwargs: PutAccountDetailsRequestRequestTypeDef = {  # (1)
    "MailType": ...,
    "WebsiteURL": ...,
}

parent.put_account_details(**kwargs)
```

1. See [:material-code-braces: PutAccountDetailsRequestRequestTypeDef](./type_defs.md#putaccountdetailsrequestrequesttypedef) 

### put\_account\_sending\_attributes

Enable or disable the ability of your account to send email.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_sending_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_account_sending_attributes)

```python
# put_account_sending_attributes method definition

await def put_account_sending_attributes(
    self,
    *,
    SendingEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_account_sending_attributes method usage example with argument unpacking

kwargs: PutAccountSendingAttributesRequestRequestTypeDef = {  # (1)
    "SendingEnabled": ...,
}

parent.put_account_sending_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountSendingAttributesRequestRequestTypeDef](./type_defs.md#putaccountsendingattributesrequestrequesttypedef) 

### put\_account\_suppression\_attributes

Change the settings for the account-level suppression list.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_suppression_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_account_suppression_attributes)

```python
# put_account_suppression_attributes method definition

await def put_account_suppression_attributes(
    self,
    *,
    SuppressedReasons: Sequence[SuppressionListReasonType] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 


```python
# put_account_suppression_attributes method usage example with argument unpacking

kwargs: PutAccountSuppressionAttributesRequestRequestTypeDef = {  # (1)
    "SuppressedReasons": ...,
}

parent.put_account_suppression_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountSuppressionAttributesRequestRequestTypeDef](./type_defs.md#putaccountsuppressionattributesrequestrequesttypedef) 

### put\_account\_vdm\_attributes

Update your Amazon SES account VDM attributes.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_vdm_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_account_vdm_attributes)

```python
# put_account_vdm_attributes method definition

await def put_account_vdm_attributes(
    self,
    *,
    VdmAttributes: VdmAttributesTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: VdmAttributesTypeDef](./type_defs.md#vdmattributestypedef) 


```python
# put_account_vdm_attributes method usage example with argument unpacking

kwargs: PutAccountVdmAttributesRequestRequestTypeDef = {  # (1)
    "VdmAttributes": ...,
}

parent.put_account_vdm_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountVdmAttributesRequestRequestTypeDef](./type_defs.md#putaccountvdmattributesrequestrequesttypedef) 

### put\_configuration\_set\_delivery\_options

Associate a configuration set with a dedicated IP pool.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_delivery_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_delivery_options)

```python
# put_configuration_set_delivery_options method definition

await def put_configuration_set_delivery_options(
    self,
    *,
    ConfigurationSetName: str,
    TlsPolicy: TlsPolicyType = ...,  # (1)
    SendingPoolName: str = ...,
    MaxDeliverySeconds: int = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 


```python
# put_configuration_set_delivery_options method usage example with argument unpacking

kwargs: PutConfigurationSetDeliveryOptionsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_delivery_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetDeliveryOptionsRequestRequestTypeDef](./type_defs.md#putconfigurationsetdeliveryoptionsrequestrequesttypedef) 

### put\_configuration\_set\_reputation\_options

Enable or disable collection of reputation metrics for emails that you send
using a particular configuration set in a specific Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_reputation_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_reputation_options)

```python
# put_configuration_set_reputation_options method definition

await def put_configuration_set_reputation_options(
    self,
    *,
    ConfigurationSetName: str,
    ReputationMetricsEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_configuration_set_reputation_options method usage example with argument unpacking

kwargs: PutConfigurationSetReputationOptionsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_reputation_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetReputationOptionsRequestRequestTypeDef](./type_defs.md#putconfigurationsetreputationoptionsrequestrequesttypedef) 

### put\_configuration\_set\_sending\_options

Enable or disable email sending for messages that use a particular
configuration set in a specific Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_sending_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_sending_options)

```python
# put_configuration_set_sending_options method definition

await def put_configuration_set_sending_options(
    self,
    *,
    ConfigurationSetName: str,
    SendingEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_configuration_set_sending_options method usage example with argument unpacking

kwargs: PutConfigurationSetSendingOptionsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_sending_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetSendingOptionsRequestRequestTypeDef](./type_defs.md#putconfigurationsetsendingoptionsrequestrequesttypedef) 

### put\_configuration\_set\_suppression\_options

Specify the account suppression list preferences for a configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_suppression_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_suppression_options)

```python
# put_configuration_set_suppression_options method definition

await def put_configuration_set_suppression_options(
    self,
    *,
    ConfigurationSetName: str,
    SuppressedReasons: Sequence[SuppressionListReasonType] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 


```python
# put_configuration_set_suppression_options method usage example with argument unpacking

kwargs: PutConfigurationSetSuppressionOptionsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_suppression_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetSuppressionOptionsRequestRequestTypeDef](./type_defs.md#putconfigurationsetsuppressionoptionsrequestrequesttypedef) 

### put\_configuration\_set\_tracking\_options

Specify a custom domain to use for open and click tracking elements in email
that you
send.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_tracking_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_tracking_options)

```python
# put_configuration_set_tracking_options method definition

await def put_configuration_set_tracking_options(
    self,
    *,
    ConfigurationSetName: str,
    CustomRedirectDomain: str = ...,
    HttpsPolicy: HttpsPolicyType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: HttpsPolicyType](./literals.md#httpspolicytype) 


```python
# put_configuration_set_tracking_options method usage example with argument unpacking

kwargs: PutConfigurationSetTrackingOptionsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_tracking_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetTrackingOptionsRequestRequestTypeDef](./type_defs.md#putconfigurationsettrackingoptionsrequestrequesttypedef) 

### put\_configuration\_set\_vdm\_options

Specify VDM preferences for email that you send using the configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_vdm_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_configuration_set_vdm_options)

```python
# put_configuration_set_vdm_options method definition

await def put_configuration_set_vdm_options(
    self,
    *,
    ConfigurationSetName: str,
    VdmOptions: VdmOptionsTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 


```python
# put_configuration_set_vdm_options method usage example with argument unpacking

kwargs: PutConfigurationSetVdmOptionsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_vdm_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetVdmOptionsRequestRequestTypeDef](./type_defs.md#putconfigurationsetvdmoptionsrequestrequesttypedef) 

### put\_dedicated\_ip\_in\_pool

Move a dedicated IP address to an existing dedicated IP pool.

Type annotations and code completion for `#!python session.create_client("sesv2").put_dedicated_ip_in_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_in_pool)

```python
# put_dedicated_ip_in_pool method definition

await def put_dedicated_ip_in_pool(
    self,
    *,
    Ip: str,
    DestinationPoolName: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_dedicated_ip_in_pool method usage example with argument unpacking

kwargs: PutDedicatedIpInPoolRequestRequestTypeDef = {  # (1)
    "Ip": ...,
    "DestinationPoolName": ...,
}

parent.put_dedicated_ip_in_pool(**kwargs)
```

1. See [:material-code-braces: PutDedicatedIpInPoolRequestRequestTypeDef](./type_defs.md#putdedicatedipinpoolrequestrequesttypedef) 

### put\_dedicated\_ip\_pool\_scaling\_attributes

Used to convert a dedicated IP pool to a different scaling mode.

Type annotations and code completion for `#!python session.create_client("sesv2").put_dedicated_ip_pool_scaling_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_pool_scaling_attributes)

```python
# put_dedicated_ip_pool_scaling_attributes method definition

await def put_dedicated_ip_pool_scaling_attributes(
    self,
    *,
    PoolName: str,
    ScalingMode: ScalingModeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 


```python
# put_dedicated_ip_pool_scaling_attributes method usage example with argument unpacking

kwargs: PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef = {  # (1)
    "PoolName": ...,
    "ScalingMode": ...,
}

parent.put_dedicated_ip_pool_scaling_attributes(**kwargs)
```

1. See [:material-code-braces: PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef](./type_defs.md#putdedicatedippoolscalingattributesrequestrequesttypedef) 

### put\_dedicated\_ip\_warmup\_attributes

See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/sesv2-2019-09-27/PutDedicatedIpWarmupAttributes).

Type annotations and code completion for `#!python session.create_client("sesv2").put_dedicated_ip_warmup_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_warmup_attributes)

```python
# put_dedicated_ip_warmup_attributes method definition

await def put_dedicated_ip_warmup_attributes(
    self,
    *,
    Ip: str,
    WarmupPercentage: int,
) -> Dict[str, Any]:
    ...
```



```python
# put_dedicated_ip_warmup_attributes method usage example with argument unpacking

kwargs: PutDedicatedIpWarmupAttributesRequestRequestTypeDef = {  # (1)
    "Ip": ...,
    "WarmupPercentage": ...,
}

parent.put_dedicated_ip_warmup_attributes(**kwargs)
```

1. See [:material-code-braces: PutDedicatedIpWarmupAttributesRequestRequestTypeDef](./type_defs.md#putdedicatedipwarmupattributesrequestrequesttypedef) 

### put\_deliverability\_dashboard\_option

Enable or disable the Deliverability dashboard.

Type annotations and code completion for `#!python session.create_client("sesv2").put_deliverability_dashboard_option` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)

```python
# put_deliverability_dashboard_option method definition

await def put_deliverability_dashboard_option(
    self,
    *,
    DashboardEnabled: bool,
    SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DomainDeliverabilityTrackingOptionTypeDef](./type_defs.md#domaindeliverabilitytrackingoptiontypedef) [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 


```python
# put_deliverability_dashboard_option method usage example with argument unpacking

kwargs: PutDeliverabilityDashboardOptionRequestRequestTypeDef = {  # (1)
    "DashboardEnabled": ...,
}

parent.put_deliverability_dashboard_option(**kwargs)
```

1. See [:material-code-braces: PutDeliverabilityDashboardOptionRequestRequestTypeDef](./type_defs.md#putdeliverabilitydashboardoptionrequestrequesttypedef) 

### put\_email\_identity\_configuration\_set\_attributes

Used to associate a configuration set with an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_configuration_set_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_configuration_set_attributes)

```python
# put_email_identity_configuration_set_attributes method definition

await def put_email_identity_configuration_set_attributes(
    self,
    *,
    EmailIdentity: str,
    ConfigurationSetName: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_email_identity_configuration_set_attributes method usage example with argument unpacking

kwargs: PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_configuration_set_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef](./type_defs.md#putemailidentityconfigurationsetattributesrequestrequesttypedef) 

### put\_email\_identity\_dkim\_attributes

Used to enable or disable DKIM authentication for an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_dkim_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_dkim_attributes)

```python
# put_email_identity_dkim_attributes method definition

await def put_email_identity_dkim_attributes(
    self,
    *,
    EmailIdentity: str,
    SigningEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_email_identity_dkim_attributes method usage example with argument unpacking

kwargs: PutEmailIdentityDkimAttributesRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_dkim_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityDkimAttributesRequestRequestTypeDef](./type_defs.md#putemailidentitydkimattributesrequestrequesttypedef) 

### put\_email\_identity\_dkim\_signing\_attributes

Used to configure or change the DKIM authentication settings for an email
domain
identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_dkim_signing_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_dkim_signing_attributes)

```python
# put_email_identity_dkim_signing_attributes method definition

await def put_email_identity_dkim_signing_attributes(
    self,
    *,
    EmailIdentity: str,
    SigningAttributesOrigin: DkimSigningAttributesOriginType,  # (1)
    SigningAttributes: DkimSigningAttributesTypeDef = ...,  # (2)
) -> PutEmailIdentityDkimSigningAttributesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DkimSigningAttributesOriginType](./literals.md#dkimsigningattributesorigintype) 
2. See [:material-code-braces: DkimSigningAttributesTypeDef](./type_defs.md#dkimsigningattributestypedef) 
3. See [:material-code-braces: PutEmailIdentityDkimSigningAttributesResponseTypeDef](./type_defs.md#putemailidentitydkimsigningattributesresponsetypedef) 


```python
# put_email_identity_dkim_signing_attributes method usage example with argument unpacking

kwargs: PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "SigningAttributesOrigin": ...,
}

parent.put_email_identity_dkim_signing_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef](./type_defs.md#putemailidentitydkimsigningattributesrequestrequesttypedef) 

### put\_email\_identity\_feedback\_attributes

Used to enable or disable feedback forwarding for an identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_feedback_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_feedback_attributes)

```python
# put_email_identity_feedback_attributes method definition

await def put_email_identity_feedback_attributes(
    self,
    *,
    EmailIdentity: str,
    EmailForwardingEnabled: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_email_identity_feedback_attributes method usage example with argument unpacking

kwargs: PutEmailIdentityFeedbackAttributesRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_feedback_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityFeedbackAttributesRequestRequestTypeDef](./type_defs.md#putemailidentityfeedbackattributesrequestrequesttypedef) 

### put\_email\_identity\_mail\_from\_attributes

Used to enable or disable the custom Mail-From domain configuration for an
email
identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_mail_from_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_email_identity_mail_from_attributes)

```python
# put_email_identity_mail_from_attributes method definition

await def put_email_identity_mail_from_attributes(
    self,
    *,
    EmailIdentity: str,
    MailFromDomain: str = ...,
    BehaviorOnMxFailure: BehaviorOnMxFailureType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: BehaviorOnMxFailureType](./literals.md#behavioronmxfailuretype) 


```python
# put_email_identity_mail_from_attributes method usage example with argument unpacking

kwargs: PutEmailIdentityMailFromAttributesRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_mail_from_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityMailFromAttributesRequestRequestTypeDef](./type_defs.md#putemailidentitymailfromattributesrequestrequesttypedef) 

### put\_suppressed\_destination

Adds an email address to the suppression list for your account.

Type annotations and code completion for `#!python session.create_client("sesv2").put_suppressed_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_suppressed_destination)

```python
# put_suppressed_destination method definition

await def put_suppressed_destination(
    self,
    *,
    EmailAddress: str,
    Reason: SuppressionListReasonType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 


```python
# put_suppressed_destination method usage example with argument unpacking

kwargs: PutSuppressedDestinationRequestRequestTypeDef = {  # (1)
    "EmailAddress": ...,
    "Reason": ...,
}

parent.put_suppressed_destination(**kwargs)
```

1. See [:material-code-braces: PutSuppressedDestinationRequestRequestTypeDef](./type_defs.md#putsuppresseddestinationrequestrequesttypedef) 

### send\_bulk\_email

Composes an email message to multiple destinations.

Type annotations and code completion for `#!python session.create_client("sesv2").send_bulk_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.send_bulk_email)

```python
# send_bulk_email method definition

await def send_bulk_email(
    self,
    *,
    DefaultContent: BulkEmailContentTypeDef,  # (1)
    BulkEmailEntries: Sequence[BulkEmailEntryTypeDef],  # (2)
    FromEmailAddress: str = ...,
    FromEmailAddressIdentityArn: str = ...,
    ReplyToAddresses: Sequence[str] = ...,
    FeedbackForwardingEmailAddress: str = ...,
    FeedbackForwardingEmailAddressIdentityArn: str = ...,
    DefaultEmailTags: Sequence[MessageTagTypeDef] = ...,  # (3)
    ConfigurationSetName: str = ...,
) -> SendBulkEmailResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: BulkEmailContentTypeDef](./type_defs.md#bulkemailcontenttypedef) 
2. See [:material-code-braces: BulkEmailEntryTypeDef](./type_defs.md#bulkemailentrytypedef) 
3. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
4. See [:material-code-braces: SendBulkEmailResponseTypeDef](./type_defs.md#sendbulkemailresponsetypedef) 


```python
# send_bulk_email method usage example with argument unpacking

kwargs: SendBulkEmailRequestRequestTypeDef = {  # (1)
    "DefaultContent": ...,
    "BulkEmailEntries": ...,
}

parent.send_bulk_email(**kwargs)
```

1. See [:material-code-braces: SendBulkEmailRequestRequestTypeDef](./type_defs.md#sendbulkemailrequestrequesttypedef) 

### send\_custom\_verification\_email

Adds an email address to the list of identities for your Amazon SES account in
the current Amazon Web Services Region and attempts to verify
it.

Type annotations and code completion for `#!python session.create_client("sesv2").send_custom_verification_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.send_custom_verification_email)

```python
# send_custom_verification_email method definition

await def send_custom_verification_email(
    self,
    *,
    EmailAddress: str,
    TemplateName: str,
    ConfigurationSetName: str = ...,
) -> SendCustomVerificationEmailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendCustomVerificationEmailResponseTypeDef](./type_defs.md#sendcustomverificationemailresponsetypedef) 


```python
# send_custom_verification_email method usage example with argument unpacking

kwargs: SendCustomVerificationEmailRequestRequestTypeDef = {  # (1)
    "EmailAddress": ...,
    "TemplateName": ...,
}

parent.send_custom_verification_email(**kwargs)
```

1. See [:material-code-braces: SendCustomVerificationEmailRequestRequestTypeDef](./type_defs.md#sendcustomverificationemailrequestrequesttypedef) 

### send\_email

Sends an email message.

Type annotations and code completion for `#!python session.create_client("sesv2").send_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.send_email)

```python
# send_email method definition

await def send_email(
    self,
    *,
    Content: EmailContentTypeDef,  # (1)
    FromEmailAddress: str = ...,
    FromEmailAddressIdentityArn: str = ...,
    Destination: DestinationTypeDef = ...,  # (2)
    ReplyToAddresses: Sequence[str] = ...,
    FeedbackForwardingEmailAddress: str = ...,
    FeedbackForwardingEmailAddressIdentityArn: str = ...,
    EmailTags: Sequence[MessageTagTypeDef] = ...,  # (3)
    ConfigurationSetName: str = ...,
    ListManagementOptions: ListManagementOptionsTypeDef = ...,  # (4)
) -> SendEmailResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
4. See [:material-code-braces: ListManagementOptionsTypeDef](./type_defs.md#listmanagementoptionstypedef) 
5. See [:material-code-braces: SendEmailResponseTypeDef](./type_defs.md#sendemailresponsetypedef) 


```python
# send_email method usage example with argument unpacking

kwargs: SendEmailRequestRequestTypeDef = {  # (1)
    "Content": ...,
}

parent.send_email(**kwargs)
```

1. See [:material-code-braces: SendEmailRequestRequestTypeDef](./type_defs.md#sendemailrequestrequesttypedef) 

### tag\_resource

Add one or more tags (keys and values) to a specified resource.

Type annotations and code completion for `#!python session.create_client("sesv2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.tag_resource)

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

### test\_render\_email\_template

Creates a preview of the MIME content of an email when provided with a template
and a set of replacement
data.

Type annotations and code completion for `#!python session.create_client("sesv2").test_render_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.test_render_email_template)

```python
# test_render_email_template method definition

await def test_render_email_template(
    self,
    *,
    TemplateName: str,
    TemplateData: str,
) -> TestRenderEmailTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestRenderEmailTemplateResponseTypeDef](./type_defs.md#testrenderemailtemplateresponsetypedef) 


```python
# test_render_email_template method usage example with argument unpacking

kwargs: TestRenderEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "TemplateData": ...,
}

parent.test_render_email_template(**kwargs)
```

1. See [:material-code-braces: TestRenderEmailTemplateRequestRequestTypeDef](./type_defs.md#testrenderemailtemplaterequestrequesttypedef) 

### untag\_resource

Remove one or more tags (keys and values) from a specified resource.

Type annotations and code completion for `#!python session.create_client("sesv2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.untag_resource)

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

### update\_configuration\_set\_event\_destination

Update the configuration of an event destination for a configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").update_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_configuration_set_event_destination)

```python
# update_configuration_set_event_destination method definition

await def update_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 


```python
# update_configuration_set_event_destination method usage example with argument unpacking

kwargs: UpdateConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
    "EventDestination": ...,
}

parent.update_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#updateconfigurationseteventdestinationrequestrequesttypedef) 

### update\_contact

Updates a contact's preferences for a list.

Type annotations and code completion for `#!python session.create_client("sesv2").update_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_contact)

```python
# update_contact method definition

await def update_contact(
    self,
    *,
    ContactListName: str,
    EmailAddress: str,
    TopicPreferences: Sequence[TopicPreferenceTypeDef] = ...,  # (1)
    UnsubscribeAll: bool = ...,
    AttributesData: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 


```python
# update_contact method usage example with argument unpacking

kwargs: UpdateContactRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.update_contact(**kwargs)
```

1. See [:material-code-braces: UpdateContactRequestRequestTypeDef](./type_defs.md#updatecontactrequestrequesttypedef) 

### update\_contact\_list

Updates contact list metadata.

Type annotations and code completion for `#!python session.create_client("sesv2").update_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_contact_list)

```python
# update_contact_list method definition

await def update_contact_list(
    self,
    *,
    ContactListName: str,
    Topics: Sequence[TopicTypeDef] = ...,  # (1)
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 


```python
# update_contact_list method usage example with argument unpacking

kwargs: UpdateContactListRequestRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.update_contact_list(**kwargs)
```

1. See [:material-code-braces: UpdateContactListRequestRequestTypeDef](./type_defs.md#updatecontactlistrequestrequesttypedef) 

### update\_custom\_verification\_email\_template

Updates an existing custom verification email template.

Type annotations and code completion for `#!python session.create_client("sesv2").update_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_custom_verification_email_template)

```python
# update_custom_verification_email_template method definition

await def update_custom_verification_email_template(
    self,
    *,
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_custom_verification_email_template method usage example with argument unpacking

kwargs: UpdateCustomVerificationEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "FromEmailAddress": ...,
    "TemplateSubject": ...,
    "TemplateContent": ...,
    "SuccessRedirectionURL": ...,
    "FailureRedirectionURL": ...,
}

parent.update_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: UpdateCustomVerificationEmailTemplateRequestRequestTypeDef](./type_defs.md#updatecustomverificationemailtemplaterequestrequesttypedef) 

### update\_email\_identity\_policy

Updates the specified sending authorization policy for the given identity (an
email address or a
domain).

Type annotations and code completion for `#!python session.create_client("sesv2").update_email_identity_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_email_identity_policy)

```python
# update_email_identity_policy method definition

await def update_email_identity_policy(
    self,
    *,
    EmailIdentity: str,
    PolicyName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_email_identity_policy method usage example with argument unpacking

kwargs: UpdateEmailIdentityPolicyRequestRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "PolicyName": ...,
    "Policy": ...,
}

parent.update_email_identity_policy(**kwargs)
```

1. See [:material-code-braces: UpdateEmailIdentityPolicyRequestRequestTypeDef](./type_defs.md#updateemailidentitypolicyrequestrequesttypedef) 

### update\_email\_template

Updates an email template.

Type annotations and code completion for `#!python session.create_client("sesv2").update_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.update_email_template)

```python
# update_email_template method definition

await def update_email_template(
    self,
    *,
    TemplateName: str,
    TemplateContent: EmailTemplateContentTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 


```python
# update_email_template method usage example with argument unpacking

kwargs: UpdateEmailTemplateRequestRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "TemplateContent": ...,
}

parent.update_email_template(**kwargs)
```

1. See [:material-code-braces: UpdateEmailTemplateRequestRequestTypeDef](./type_defs.md#updateemailtemplaterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sesv2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SESV2Client":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sesv2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.__aexit__)

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






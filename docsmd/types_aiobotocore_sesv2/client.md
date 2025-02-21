# SESV2Client

> [Index](../README.md) > [SESV2](./README.md) > SESV2Client

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#sesv2)
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


### can\_paginate



Type annotations and code completion for `#!python session.create_client("sesv2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("sesv2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/generate_presigned_url.html)

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


### batch\_get\_metric\_data

Retrieves batches of metric data collected based on your sending activity.

Type annotations and code completion for `#!python session.create_client("sesv2").batch_get_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/batch_get_metric_data.html)

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

kwargs: BatchGetMetricDataRequestTypeDef = {  # (1)
    "Queries": ...,
}

parent.batch_get_metric_data(**kwargs)
```

1. See [:material-code-braces: BatchGetMetricDataRequestTypeDef](./type_defs.md#batchgetmetricdatarequesttypedef) 

### cancel\_export\_job

Cancels an export job.

Type annotations and code completion for `#!python session.create_client("sesv2").cancel_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/cancel_export_job.html)

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

kwargs: CancelExportJobRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.cancel_export_job(**kwargs)
```

1. See [:material-code-braces: CancelExportJobRequestTypeDef](./type_defs.md#cancelexportjobrequesttypedef) 

### create\_configuration\_set

Create a configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").create_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_configuration_set.html)

```python
# create_configuration_set method definition

await def create_configuration_set(
    self,
    *,
    ConfigurationSetName: str,
    TrackingOptions: TrackingOptionsTypeDef = ...,  # (1)
    DeliveryOptions: DeliveryOptionsTypeDef = ...,  # (2)
    ReputationOptions: ReputationOptionsUnionTypeDef = ...,  # (3)
    SendingOptions: SendingOptionsTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,  # (6)
    VdmOptions: VdmOptionsTypeDef = ...,  # (7)
    ArchivingOptions: ArchivingOptionsTypeDef = ...,  # (8)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsTypeDef](./type_defs.md#reputationoptionstypedef) [:material-code-braces: ReputationOptionsOutputTypeDef](./type_defs.md#reputationoptionsoutputtypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: SuppressionOptionsTypeDef](./type_defs.md#suppressionoptionstypedef) [:material-code-braces: SuppressionOptionsOutputTypeDef](./type_defs.md#suppressionoptionsoutputtypedef) 
7. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 
8. See [:material-code-braces: ArchivingOptionsTypeDef](./type_defs.md#archivingoptionstypedef) 


```python
# create_configuration_set method usage example with argument unpacking

kwargs: CreateConfigurationSetRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.create_configuration_set(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetRequestTypeDef](./type_defs.md#createconfigurationsetrequesttypedef) 

### create\_configuration\_set\_event\_destination

Create an event destination.

Type annotations and code completion for `#!python session.create_client("sesv2").create_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_configuration_set_event_destination.html)

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

kwargs: CreateConfigurationSetEventDestinationRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
    "EventDestination": ...,
}

parent.create_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetEventDestinationRequestTypeDef](./type_defs.md#createconfigurationseteventdestinationrequesttypedef) 

### create\_contact

Creates a contact, which is an end-user who is receiving the email, and adds
them to a contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").create_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_contact.html)

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

kwargs: CreateContactRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.create_contact(**kwargs)
```

1. See [:material-code-braces: CreateContactRequestTypeDef](./type_defs.md#createcontactrequesttypedef) 

### create\_contact\_list

Creates a contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").create_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_contact_list.html)

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

kwargs: CreateContactListRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.create_contact_list(**kwargs)
```

1. See [:material-code-braces: CreateContactListRequestTypeDef](./type_defs.md#createcontactlistrequesttypedef) 

### create\_custom\_verification\_email\_template

Creates a new custom verification email template.

Type annotations and code completion for `#!python session.create_client("sesv2").create_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_custom_verification_email_template.html)

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

kwargs: CreateCustomVerificationEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "FromEmailAddress": ...,
    "TemplateSubject": ...,
    "TemplateContent": ...,
    "SuccessRedirectionURL": ...,
    "FailureRedirectionURL": ...,
}

parent.create_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: CreateCustomVerificationEmailTemplateRequestTypeDef](./type_defs.md#createcustomverificationemailtemplaterequesttypedef) 

### create\_dedicated\_ip\_pool

Create a new pool of dedicated IP addresses.

Type annotations and code completion for `#!python session.create_client("sesv2").create_dedicated_ip_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_dedicated_ip_pool.html)

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

kwargs: CreateDedicatedIpPoolRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.create_dedicated_ip_pool(**kwargs)
```

1. See [:material-code-braces: CreateDedicatedIpPoolRequestTypeDef](./type_defs.md#creatededicatedippoolrequesttypedef) 

### create\_deliverability\_test\_report

Create a new predictive inbox placement test.

Type annotations and code completion for `#!python session.create_client("sesv2").create_deliverability_test_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_deliverability_test_report.html)

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

kwargs: CreateDeliverabilityTestReportRequestTypeDef = {  # (1)
    "FromEmailAddress": ...,
    "Content": ...,
}

parent.create_deliverability_test_report(**kwargs)
```

1. See [:material-code-braces: CreateDeliverabilityTestReportRequestTypeDef](./type_defs.md#createdeliverabilitytestreportrequesttypedef) 

### create\_email\_identity

Starts the process of verifying an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").create_email_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_email_identity.html)

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

kwargs: CreateEmailIdentityRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.create_email_identity(**kwargs)
```

1. See [:material-code-braces: CreateEmailIdentityRequestTypeDef](./type_defs.md#createemailidentityrequesttypedef) 

### create\_email\_identity\_policy

Creates the specified sending authorization policy for the given identity (an
email address or a domain).

Type annotations and code completion for `#!python session.create_client("sesv2").create_email_identity_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_email_identity_policy.html)

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

kwargs: CreateEmailIdentityPolicyRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "PolicyName": ...,
    "Policy": ...,
}

parent.create_email_identity_policy(**kwargs)
```

1. See [:material-code-braces: CreateEmailIdentityPolicyRequestTypeDef](./type_defs.md#createemailidentitypolicyrequesttypedef) 

### create\_email\_template

Creates an email template.

Type annotations and code completion for `#!python session.create_client("sesv2").create_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_email_template.html)

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

kwargs: CreateEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "TemplateContent": ...,
}

parent.create_email_template(**kwargs)
```

1. See [:material-code-braces: CreateEmailTemplateRequestTypeDef](./type_defs.md#createemailtemplaterequesttypedef) 

### create\_export\_job

Creates an export job for a data source and destination.

Type annotations and code completion for `#!python session.create_client("sesv2").create_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_export_job.html)

```python
# create_export_job method definition

await def create_export_job(
    self,
    *,
    ExportDataSource: ExportDataSourceUnionTypeDef,  # (1)
    ExportDestination: ExportDestinationTypeDef,  # (2)
) -> CreateExportJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExportDataSourceTypeDef](./type_defs.md#exportdatasourcetypedef) [:material-code-braces: ExportDataSourceOutputTypeDef](./type_defs.md#exportdatasourceoutputtypedef) 
2. See [:material-code-braces: ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef) 
3. See [:material-code-braces: CreateExportJobResponseTypeDef](./type_defs.md#createexportjobresponsetypedef) 


```python
# create_export_job method usage example with argument unpacking

kwargs: CreateExportJobRequestTypeDef = {  # (1)
    "ExportDataSource": ...,
    "ExportDestination": ...,
}

parent.create_export_job(**kwargs)
```

1. See [:material-code-braces: CreateExportJobRequestTypeDef](./type_defs.md#createexportjobrequesttypedef) 

### create\_import\_job

Creates an import job for a data destination.

Type annotations and code completion for `#!python session.create_client("sesv2").create_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_import_job.html)

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

kwargs: CreateImportJobRequestTypeDef = {  # (1)
    "ImportDestination": ...,
    "ImportDataSource": ...,
}

parent.create_import_job(**kwargs)
```

1. See [:material-code-braces: CreateImportJobRequestTypeDef](./type_defs.md#createimportjobrequesttypedef) 

### create\_multi\_region\_endpoint

Creates a multi-region endpoint (global-endpoint).

Type annotations and code completion for `#!python session.create_client("sesv2").create_multi_region_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/create_multi_region_endpoint.html)

```python
# create_multi_region_endpoint method definition

await def create_multi_region_endpoint(
    self,
    *,
    EndpointName: str,
    Details: DetailsTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateMultiRegionEndpointResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DetailsTypeDef](./type_defs.md#detailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateMultiRegionEndpointResponseTypeDef](./type_defs.md#createmultiregionendpointresponsetypedef) 


```python
# create_multi_region_endpoint method usage example with argument unpacking

kwargs: CreateMultiRegionEndpointRequestTypeDef = {  # (1)
    "EndpointName": ...,
    "Details": ...,
}

parent.create_multi_region_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateMultiRegionEndpointRequestTypeDef](./type_defs.md#createmultiregionendpointrequesttypedef) 

### delete\_configuration\_set

Delete an existing configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_configuration_set.html)

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

kwargs: DeleteConfigurationSetRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.delete_configuration_set(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetRequestTypeDef](./type_defs.md#deleteconfigurationsetrequesttypedef) 

### delete\_configuration\_set\_event\_destination

Delete an event destination.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_configuration_set_event_destination.html)

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

kwargs: DeleteConfigurationSetEventDestinationRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
}

parent.delete_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetEventDestinationRequestTypeDef](./type_defs.md#deleteconfigurationseteventdestinationrequesttypedef) 

### delete\_contact

Removes a contact from a contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_contact.html)

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

kwargs: DeleteContactRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.delete_contact(**kwargs)
```

1. See [:material-code-braces: DeleteContactRequestTypeDef](./type_defs.md#deletecontactrequesttypedef) 

### delete\_contact\_list

Deletes a contact list and all of the contacts on that list.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_contact_list.html)

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

kwargs: DeleteContactListRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.delete_contact_list(**kwargs)
```

1. See [:material-code-braces: DeleteContactListRequestTypeDef](./type_defs.md#deletecontactlistrequesttypedef) 

### delete\_custom\_verification\_email\_template

Deletes an existing custom verification email template.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_custom_verification_email_template.html)

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

kwargs: DeleteCustomVerificationEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.delete_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: DeleteCustomVerificationEmailTemplateRequestTypeDef](./type_defs.md#deletecustomverificationemailtemplaterequesttypedef) 

### delete\_dedicated\_ip\_pool

Delete a dedicated IP pool.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_dedicated_ip_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_dedicated_ip_pool.html)

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

kwargs: DeleteDedicatedIpPoolRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.delete_dedicated_ip_pool(**kwargs)
```

1. See [:material-code-braces: DeleteDedicatedIpPoolRequestTypeDef](./type_defs.md#deletededicatedippoolrequesttypedef) 

### delete\_email\_identity

Deletes an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_email_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_email_identity.html)

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

kwargs: DeleteEmailIdentityRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.delete_email_identity(**kwargs)
```

1. See [:material-code-braces: DeleteEmailIdentityRequestTypeDef](./type_defs.md#deleteemailidentityrequesttypedef) 

### delete\_email\_identity\_policy

Deletes the specified sending authorization policy for the given identity (an
email address or a domain).

Type annotations and code completion for `#!python session.create_client("sesv2").delete_email_identity_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_email_identity_policy.html)

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

kwargs: DeleteEmailIdentityPolicyRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "PolicyName": ...,
}

parent.delete_email_identity_policy(**kwargs)
```

1. See [:material-code-braces: DeleteEmailIdentityPolicyRequestTypeDef](./type_defs.md#deleteemailidentitypolicyrequesttypedef) 

### delete\_email\_template

Deletes an email template.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_email_template.html)

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

kwargs: DeleteEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.delete_email_template(**kwargs)
```

1. See [:material-code-braces: DeleteEmailTemplateRequestTypeDef](./type_defs.md#deleteemailtemplaterequesttypedef) 

### delete\_multi\_region\_endpoint

Deletes a multi-region endpoint (global-endpoint).

Type annotations and code completion for `#!python session.create_client("sesv2").delete_multi_region_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_multi_region_endpoint.html)

```python
# delete_multi_region_endpoint method definition

await def delete_multi_region_endpoint(
    self,
    *,
    EndpointName: str,
) -> DeleteMultiRegionEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMultiRegionEndpointResponseTypeDef](./type_defs.md#deletemultiregionendpointresponsetypedef) 


```python
# delete_multi_region_endpoint method usage example with argument unpacking

kwargs: DeleteMultiRegionEndpointRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.delete_multi_region_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteMultiRegionEndpointRequestTypeDef](./type_defs.md#deletemultiregionendpointrequesttypedef) 

### delete\_suppressed\_destination

Removes an email address from the suppression list for your account.

Type annotations and code completion for `#!python session.create_client("sesv2").delete_suppressed_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/delete_suppressed_destination.html)

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

kwargs: DeleteSuppressedDestinationRequestTypeDef = {  # (1)
    "EmailAddress": ...,
}

parent.delete_suppressed_destination(**kwargs)
```

1. See [:material-code-braces: DeleteSuppressedDestinationRequestTypeDef](./type_defs.md#deletesuppresseddestinationrequesttypedef) 

### get\_account

Obtain information about the email-sending status and capabilities of your
Amazon SES account in the current Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("sesv2").get_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_account.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_blacklist_reports.html)

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

kwargs: GetBlacklistReportsRequestTypeDef = {  # (1)
    "BlacklistItemNames": ...,
}

parent.get_blacklist_reports(**kwargs)
```

1. See [:material-code-braces: GetBlacklistReportsRequestTypeDef](./type_defs.md#getblacklistreportsrequesttypedef) 

### get\_configuration\_set

Get information about an existing configuration set, including the dedicated IP
pool that it's associated with, whether or not it's enabled for sending email,
and more.

Type annotations and code completion for `#!python session.create_client("sesv2").get_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_configuration_set.html)

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

kwargs: GetConfigurationSetRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.get_configuration_set(**kwargs)
```

1. See [:material-code-braces: GetConfigurationSetRequestTypeDef](./type_defs.md#getconfigurationsetrequesttypedef) 

### get\_configuration\_set\_event\_destinations

Retrieve a list of event destinations that are associated with a configuration
set.

Type annotations and code completion for `#!python session.create_client("sesv2").get_configuration_set_event_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_configuration_set_event_destinations.html)

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

kwargs: GetConfigurationSetEventDestinationsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.get_configuration_set_event_destinations(**kwargs)
```

1. See [:material-code-braces: GetConfigurationSetEventDestinationsRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequesttypedef) 

### get\_contact

Returns a contact from a contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").get_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_contact.html)

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

kwargs: GetContactRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.get_contact(**kwargs)
```

1. See [:material-code-braces: GetContactRequestTypeDef](./type_defs.md#getcontactrequesttypedef) 

### get\_contact\_list

Returns contact list metadata.

Type annotations and code completion for `#!python session.create_client("sesv2").get_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_contact_list.html)

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

kwargs: GetContactListRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.get_contact_list(**kwargs)
```

1. See [:material-code-braces: GetContactListRequestTypeDef](./type_defs.md#getcontactlistrequesttypedef) 

### get\_custom\_verification\_email\_template

Returns the custom email verification template for the template name you
specify.

Type annotations and code completion for `#!python session.create_client("sesv2").get_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_custom_verification_email_template.html)

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

kwargs: GetCustomVerificationEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.get_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: GetCustomVerificationEmailTemplateRequestTypeDef](./type_defs.md#getcustomverificationemailtemplaterequesttypedef) 

### get\_dedicated\_ip

Get information about a dedicated IP address, including the name of the
dedicated IP pool that it's associated with, as well information about the
automatic warm-up process for the address.

Type annotations and code completion for `#!python session.create_client("sesv2").get_dedicated_ip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_dedicated_ip.html)

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

kwargs: GetDedicatedIpRequestTypeDef = {  # (1)
    "Ip": ...,
}

parent.get_dedicated_ip(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpRequestTypeDef](./type_defs.md#getdedicatediprequesttypedef) 

### get\_dedicated\_ip\_pool

Retrieve information about the dedicated pool.

Type annotations and code completion for `#!python session.create_client("sesv2").get_dedicated_ip_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_dedicated_ip_pool.html)

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

kwargs: GetDedicatedIpPoolRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.get_dedicated_ip_pool(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpPoolRequestTypeDef](./type_defs.md#getdedicatedippoolrequesttypedef) 

### get\_dedicated\_ips

List the dedicated IP addresses that are associated with your Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("sesv2").get_dedicated_ips` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_dedicated_ips.html)

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

kwargs: GetDedicatedIpsRequestTypeDef = {  # (1)
    "PoolName": ...,
}

parent.get_dedicated_ips(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpsRequestTypeDef](./type_defs.md#getdedicatedipsrequesttypedef) 

### get\_deliverability\_dashboard\_options

Retrieve information about the status of the Deliverability dashboard for your
account.

Type annotations and code completion for `#!python session.create_client("sesv2").get_deliverability_dashboard_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_deliverability_dashboard_options.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_deliverability_test_report.html)

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

kwargs: GetDeliverabilityTestReportRequestTypeDef = {  # (1)
    "ReportId": ...,
}

parent.get_deliverability_test_report(**kwargs)
```

1. See [:material-code-braces: GetDeliverabilityTestReportRequestTypeDef](./type_defs.md#getdeliverabilitytestreportrequesttypedef) 

### get\_domain\_deliverability\_campaign

Retrieve all the deliverability data for a specific campaign.

Type annotations and code completion for `#!python session.create_client("sesv2").get_domain_deliverability_campaign` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_domain_deliverability_campaign.html)

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

kwargs: GetDomainDeliverabilityCampaignRequestTypeDef = {  # (1)
    "CampaignId": ...,
}

parent.get_domain_deliverability_campaign(**kwargs)
```

1. See [:material-code-braces: GetDomainDeliverabilityCampaignRequestTypeDef](./type_defs.md#getdomaindeliverabilitycampaignrequesttypedef) 

### get\_domain\_statistics\_report

Retrieve inbox placement and engagement rates for the domains that you use to
send email.

Type annotations and code completion for `#!python session.create_client("sesv2").get_domain_statistics_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_domain_statistics_report.html)

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

kwargs: GetDomainStatisticsReportRequestTypeDef = {  # (1)
    "Domain": ...,
    "StartDate": ...,
    "EndDate": ...,
}

parent.get_domain_statistics_report(**kwargs)
```

1. See [:material-code-braces: GetDomainStatisticsReportRequestTypeDef](./type_defs.md#getdomainstatisticsreportrequesttypedef) 

### get\_email\_identity

Provides information about a specific identity, including the identity's
verification status, sending authorization policies, its DKIM authentication
status, and its custom Mail-From settings.

Type annotations and code completion for `#!python session.create_client("sesv2").get_email_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_email_identity.html)

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

kwargs: GetEmailIdentityRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.get_email_identity(**kwargs)
```

1. See [:material-code-braces: GetEmailIdentityRequestTypeDef](./type_defs.md#getemailidentityrequesttypedef) 

### get\_email\_identity\_policies

Returns the requested sending authorization policies for the given identity (an
email address or a domain).

Type annotations and code completion for `#!python session.create_client("sesv2").get_email_identity_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_email_identity_policies.html)

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

kwargs: GetEmailIdentityPoliciesRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.get_email_identity_policies(**kwargs)
```

1. See [:material-code-braces: GetEmailIdentityPoliciesRequestTypeDef](./type_defs.md#getemailidentitypoliciesrequesttypedef) 

### get\_email\_template

Displays the template object (which includes the subject line, HTML part and
text part) for the template you specify.

Type annotations and code completion for `#!python session.create_client("sesv2").get_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_email_template.html)

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

kwargs: GetEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
}

parent.get_email_template(**kwargs)
```

1. See [:material-code-braces: GetEmailTemplateRequestTypeDef](./type_defs.md#getemailtemplaterequesttypedef) 

### get\_export\_job

Provides information about an export job.

Type annotations and code completion for `#!python session.create_client("sesv2").get_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_export_job.html)

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

kwargs: GetExportJobRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_export_job(**kwargs)
```

1. See [:material-code-braces: GetExportJobRequestTypeDef](./type_defs.md#getexportjobrequesttypedef) 

### get\_import\_job

Provides information about an import job.

Type annotations and code completion for `#!python session.create_client("sesv2").get_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_import_job.html)

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

kwargs: GetImportJobRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_import_job(**kwargs)
```

1. See [:material-code-braces: GetImportJobRequestTypeDef](./type_defs.md#getimportjobrequesttypedef) 

### get\_message\_insights

Provides information about a specific message, including the from address, the
subject, the recipient address, email tags, as well as events associated with
the message.

Type annotations and code completion for `#!python session.create_client("sesv2").get_message_insights` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_message_insights.html)

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

kwargs: GetMessageInsightsRequestTypeDef = {  # (1)
    "MessageId": ...,
}

parent.get_message_insights(**kwargs)
```

1. See [:material-code-braces: GetMessageInsightsRequestTypeDef](./type_defs.md#getmessageinsightsrequesttypedef) 

### get\_multi\_region\_endpoint

Displays the multi-region endpoint (global-endpoint) configuration.

Type annotations and code completion for `#!python session.create_client("sesv2").get_multi_region_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_multi_region_endpoint.html)

```python
# get_multi_region_endpoint method definition

await def get_multi_region_endpoint(
    self,
    *,
    EndpointName: str,
) -> GetMultiRegionEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMultiRegionEndpointResponseTypeDef](./type_defs.md#getmultiregionendpointresponsetypedef) 


```python
# get_multi_region_endpoint method usage example with argument unpacking

kwargs: GetMultiRegionEndpointRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.get_multi_region_endpoint(**kwargs)
```

1. See [:material-code-braces: GetMultiRegionEndpointRequestTypeDef](./type_defs.md#getmultiregionendpointrequesttypedef) 

### get\_suppressed\_destination

Retrieves information about a specific email address that's on the suppression
list for your account.

Type annotations and code completion for `#!python session.create_client("sesv2").get_suppressed_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/get_suppressed_destination.html)

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

kwargs: GetSuppressedDestinationRequestTypeDef = {  # (1)
    "EmailAddress": ...,
}

parent.get_suppressed_destination(**kwargs)
```

1. See [:material-code-braces: GetSuppressedDestinationRequestTypeDef](./type_defs.md#getsuppresseddestinationrequesttypedef) 

### list\_configuration\_sets

List all of the configuration sets associated with your account in the current
region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_configuration_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_configuration_sets.html)

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

kwargs: ListConfigurationSetsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_configuration_sets(**kwargs)
```

1. See [:material-code-braces: ListConfigurationSetsRequestTypeDef](./type_defs.md#listconfigurationsetsrequesttypedef) 

### list\_contact\_lists

Lists all of the contact lists available.

Type annotations and code completion for `#!python session.create_client("sesv2").list_contact_lists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_contact_lists.html)

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

kwargs: ListContactListsRequestTypeDef = {  # (1)
    "PageSize": ...,
}

parent.list_contact_lists(**kwargs)
```

1. See [:material-code-braces: ListContactListsRequestTypeDef](./type_defs.md#listcontactlistsrequesttypedef) 

### list\_contacts

Lists the contacts present in a specific contact list.

Type annotations and code completion for `#!python session.create_client("sesv2").list_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_contacts.html)

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

kwargs: ListContactsRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.list_contacts(**kwargs)
```

1. See [:material-code-braces: ListContactsRequestTypeDef](./type_defs.md#listcontactsrequesttypedef) 

### list\_custom\_verification\_email\_templates

Lists the existing custom verification email templates for your account in the
current Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_custom_verification_email_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_custom_verification_email_templates.html)

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

kwargs: ListCustomVerificationEmailTemplatesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_custom_verification_email_templates(**kwargs)
```

1. See [:material-code-braces: ListCustomVerificationEmailTemplatesRequestTypeDef](./type_defs.md#listcustomverificationemailtemplatesrequesttypedef) 

### list\_dedicated\_ip\_pools

List all of the dedicated IP pools that exist in your Amazon Web Services
account in the current Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_dedicated_ip_pools` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_dedicated_ip_pools.html)

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

kwargs: ListDedicatedIpPoolsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_dedicated_ip_pools(**kwargs)
```

1. See [:material-code-braces: ListDedicatedIpPoolsRequestTypeDef](./type_defs.md#listdedicatedippoolsrequesttypedef) 

### list\_deliverability\_test\_reports

Show a list of the predictive inbox placement tests that you've performed,
regardless of their statuses.

Type annotations and code completion for `#!python session.create_client("sesv2").list_deliverability_test_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_deliverability_test_reports.html)

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

kwargs: ListDeliverabilityTestReportsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_deliverability_test_reports(**kwargs)
```

1. See [:material-code-braces: ListDeliverabilityTestReportsRequestTypeDef](./type_defs.md#listdeliverabilitytestreportsrequesttypedef) 

### list\_domain\_deliverability\_campaigns

Retrieve deliverability data for all the campaigns that used a specific domain
to send email during a specified time range.

Type annotations and code completion for `#!python session.create_client("sesv2").list_domain_deliverability_campaigns` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_domain_deliverability_campaigns.html)

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

kwargs: ListDomainDeliverabilityCampaignsRequestTypeDef = {  # (1)
    "StartDate": ...,
    "EndDate": ...,
    "SubscribedDomain": ...,
}

parent.list_domain_deliverability_campaigns(**kwargs)
```

1. See [:material-code-braces: ListDomainDeliverabilityCampaignsRequestTypeDef](./type_defs.md#listdomaindeliverabilitycampaignsrequesttypedef) 

### list\_email\_identities

Returns a list of all of the email identities that are associated with your
Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("sesv2").list_email_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_email_identities.html)

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

kwargs: ListEmailIdentitiesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_email_identities(**kwargs)
```

1. See [:material-code-braces: ListEmailIdentitiesRequestTypeDef](./type_defs.md#listemailidentitiesrequesttypedef) 

### list\_email\_templates

Lists the email templates present in your Amazon SES account in the current
Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_email_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_email_templates.html)

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

kwargs: ListEmailTemplatesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_email_templates(**kwargs)
```

1. See [:material-code-braces: ListEmailTemplatesRequestTypeDef](./type_defs.md#listemailtemplatesrequesttypedef) 

### list\_export\_jobs

Lists all of the export jobs.

Type annotations and code completion for `#!python session.create_client("sesv2").list_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_export_jobs.html)

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

kwargs: ListExportJobsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListExportJobsRequestTypeDef](./type_defs.md#listexportjobsrequesttypedef) 

### list\_import\_jobs

Lists all of the import jobs.

Type annotations and code completion for `#!python session.create_client("sesv2").list_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_import_jobs.html)

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

kwargs: ListImportJobsRequestTypeDef = {  # (1)
    "ImportDestinationType": ...,
}

parent.list_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListImportJobsRequestTypeDef](./type_defs.md#listimportjobsrequesttypedef) 

### list\_multi\_region\_endpoints

List the multi-region endpoints (global-endpoints).

Type annotations and code completion for `#!python session.create_client("sesv2").list_multi_region_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_multi_region_endpoints.html)

```python
# list_multi_region_endpoints method definition

await def list_multi_region_endpoints(
    self,
    *,
    NextToken: str = ...,
    PageSize: int = ...,
) -> ListMultiRegionEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMultiRegionEndpointsResponseTypeDef](./type_defs.md#listmultiregionendpointsresponsetypedef) 


```python
# list_multi_region_endpoints method usage example with argument unpacking

kwargs: ListMultiRegionEndpointsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_multi_region_endpoints(**kwargs)
```

1. See [:material-code-braces: ListMultiRegionEndpointsRequestTypeDef](./type_defs.md#listmultiregionendpointsrequesttypedef) 

### list\_recommendations

Lists the recommendations present in your Amazon SES account in the current
Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("sesv2").list_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_recommendations.html)

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

kwargs: ListRecommendationsRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_recommendations(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestTypeDef](./type_defs.md#listrecommendationsrequesttypedef) 

### list\_suppressed\_destinations

Retrieves a list of email addresses that are on the suppression list for your
account.

Type annotations and code completion for `#!python session.create_client("sesv2").list_suppressed_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_suppressed_destinations.html)

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

kwargs: ListSuppressedDestinationsRequestTypeDef = {  # (1)
    "Reasons": ...,
}

parent.list_suppressed_destinations(**kwargs)
```

1. See [:material-code-braces: ListSuppressedDestinationsRequestTypeDef](./type_defs.md#listsuppresseddestinationsrequesttypedef) 

### list\_tags\_for\_resource

Retrieve a list of the tags (keys and values) that are associated with a
specified resource.

Type annotations and code completion for `#!python session.create_client("sesv2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### put\_account\_dedicated\_ip\_warmup\_attributes

Enable or disable the automatic warm-up feature for dedicated IP addresses.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_dedicated_ip_warmup_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_account_dedicated_ip_warmup_attributes.html)

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

kwargs: PutAccountDedicatedIpWarmupAttributesRequestTypeDef = {  # (1)
    "AutoWarmupEnabled": ...,
}

parent.put_account_dedicated_ip_warmup_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountDedicatedIpWarmupAttributesRequestTypeDef](./type_defs.md#putaccountdedicatedipwarmupattributesrequesttypedef) 

### put\_account\_details

Update your Amazon SES account details.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_account_details.html)

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

kwargs: PutAccountDetailsRequestTypeDef = {  # (1)
    "MailType": ...,
    "WebsiteURL": ...,
}

parent.put_account_details(**kwargs)
```

1. See [:material-code-braces: PutAccountDetailsRequestTypeDef](./type_defs.md#putaccountdetailsrequesttypedef) 

### put\_account\_sending\_attributes

Enable or disable the ability of your account to send email.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_sending_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_account_sending_attributes.html)

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

kwargs: PutAccountSendingAttributesRequestTypeDef = {  # (1)
    "SendingEnabled": ...,
}

parent.put_account_sending_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountSendingAttributesRequestTypeDef](./type_defs.md#putaccountsendingattributesrequesttypedef) 

### put\_account\_suppression\_attributes

Change the settings for the account-level suppression list.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_suppression_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_account_suppression_attributes.html)

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

kwargs: PutAccountSuppressionAttributesRequestTypeDef = {  # (1)
    "SuppressedReasons": ...,
}

parent.put_account_suppression_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountSuppressionAttributesRequestTypeDef](./type_defs.md#putaccountsuppressionattributesrequesttypedef) 

### put\_account\_vdm\_attributes

Update your Amazon SES account VDM attributes.

Type annotations and code completion for `#!python session.create_client("sesv2").put_account_vdm_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_account_vdm_attributes.html)

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

kwargs: PutAccountVdmAttributesRequestTypeDef = {  # (1)
    "VdmAttributes": ...,
}

parent.put_account_vdm_attributes(**kwargs)
```

1. See [:material-code-braces: PutAccountVdmAttributesRequestTypeDef](./type_defs.md#putaccountvdmattributesrequesttypedef) 

### put\_configuration\_set\_archiving\_options

Associate the configuration set with a MailManager archive.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_archiving_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_configuration_set_archiving_options.html)

```python
# put_configuration_set_archiving_options method definition

await def put_configuration_set_archiving_options(
    self,
    *,
    ConfigurationSetName: str,
    ArchiveArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_configuration_set_archiving_options method usage example with argument unpacking

kwargs: PutConfigurationSetArchivingOptionsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_archiving_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetArchivingOptionsRequestTypeDef](./type_defs.md#putconfigurationsetarchivingoptionsrequesttypedef) 

### put\_configuration\_set\_delivery\_options

Associate a configuration set with a dedicated IP pool.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_delivery_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_configuration_set_delivery_options.html)

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

kwargs: PutConfigurationSetDeliveryOptionsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_delivery_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetDeliveryOptionsRequestTypeDef](./type_defs.md#putconfigurationsetdeliveryoptionsrequesttypedef) 

### put\_configuration\_set\_reputation\_options

Enable or disable collection of reputation metrics for emails that you send
using a particular configuration set in a specific Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_reputation_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_configuration_set_reputation_options.html)

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

kwargs: PutConfigurationSetReputationOptionsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_reputation_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetReputationOptionsRequestTypeDef](./type_defs.md#putconfigurationsetreputationoptionsrequesttypedef) 

### put\_configuration\_set\_sending\_options

Enable or disable email sending for messages that use a particular
configuration set in a specific Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_sending_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_configuration_set_sending_options.html)

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

kwargs: PutConfigurationSetSendingOptionsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_sending_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetSendingOptionsRequestTypeDef](./type_defs.md#putconfigurationsetsendingoptionsrequesttypedef) 

### put\_configuration\_set\_suppression\_options

Specify the account suppression list preferences for a configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_suppression_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_configuration_set_suppression_options.html)

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

kwargs: PutConfigurationSetSuppressionOptionsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_suppression_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetSuppressionOptionsRequestTypeDef](./type_defs.md#putconfigurationsetsuppressionoptionsrequesttypedef) 

### put\_configuration\_set\_tracking\_options

Specify a custom domain to use for open and click tracking elements in email
that you send.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_tracking_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_configuration_set_tracking_options.html)

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

kwargs: PutConfigurationSetTrackingOptionsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_tracking_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetTrackingOptionsRequestTypeDef](./type_defs.md#putconfigurationsettrackingoptionsrequesttypedef) 

### put\_configuration\_set\_vdm\_options

Specify VDM preferences for email that you send using the configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").put_configuration_set_vdm_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_configuration_set_vdm_options.html)

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

kwargs: PutConfigurationSetVdmOptionsRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.put_configuration_set_vdm_options(**kwargs)
```

1. See [:material-code-braces: PutConfigurationSetVdmOptionsRequestTypeDef](./type_defs.md#putconfigurationsetvdmoptionsrequesttypedef) 

### put\_dedicated\_ip\_in\_pool

Move a dedicated IP address to an existing dedicated IP pool.

Type annotations and code completion for `#!python session.create_client("sesv2").put_dedicated_ip_in_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_dedicated_ip_in_pool.html)

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

kwargs: PutDedicatedIpInPoolRequestTypeDef = {  # (1)
    "Ip": ...,
    "DestinationPoolName": ...,
}

parent.put_dedicated_ip_in_pool(**kwargs)
```

1. See [:material-code-braces: PutDedicatedIpInPoolRequestTypeDef](./type_defs.md#putdedicatedipinpoolrequesttypedef) 

### put\_dedicated\_ip\_pool\_scaling\_attributes

Used to convert a dedicated IP pool to a different scaling mode.

Type annotations and code completion for `#!python session.create_client("sesv2").put_dedicated_ip_pool_scaling_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_dedicated_ip_pool_scaling_attributes.html)

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

kwargs: PutDedicatedIpPoolScalingAttributesRequestTypeDef = {  # (1)
    "PoolName": ...,
    "ScalingMode": ...,
}

parent.put_dedicated_ip_pool_scaling_attributes(**kwargs)
```

1. See [:material-code-braces: PutDedicatedIpPoolScalingAttributesRequestTypeDef](./type_defs.md#putdedicatedippoolscalingattributesrequesttypedef) 

### put\_dedicated\_ip\_warmup\_attributes

<p/>.

Type annotations and code completion for `#!python session.create_client("sesv2").put_dedicated_ip_warmup_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_dedicated_ip_warmup_attributes.html)

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

kwargs: PutDedicatedIpWarmupAttributesRequestTypeDef = {  # (1)
    "Ip": ...,
    "WarmupPercentage": ...,
}

parent.put_dedicated_ip_warmup_attributes(**kwargs)
```

1. See [:material-code-braces: PutDedicatedIpWarmupAttributesRequestTypeDef](./type_defs.md#putdedicatedipwarmupattributesrequesttypedef) 

### put\_deliverability\_dashboard\_option

Enable or disable the Deliverability dashboard.

Type annotations and code completion for `#!python session.create_client("sesv2").put_deliverability_dashboard_option` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_deliverability_dashboard_option.html)

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

kwargs: PutDeliverabilityDashboardOptionRequestTypeDef = {  # (1)
    "DashboardEnabled": ...,
}

parent.put_deliverability_dashboard_option(**kwargs)
```

1. See [:material-code-braces: PutDeliverabilityDashboardOptionRequestTypeDef](./type_defs.md#putdeliverabilitydashboardoptionrequesttypedef) 

### put\_email\_identity\_configuration\_set\_attributes

Used to associate a configuration set with an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_configuration_set_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_email_identity_configuration_set_attributes.html)

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

kwargs: PutEmailIdentityConfigurationSetAttributesRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_configuration_set_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityConfigurationSetAttributesRequestTypeDef](./type_defs.md#putemailidentityconfigurationsetattributesrequesttypedef) 

### put\_email\_identity\_dkim\_attributes

Used to enable or disable DKIM authentication for an email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_dkim_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_email_identity_dkim_attributes.html)

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

kwargs: PutEmailIdentityDkimAttributesRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_dkim_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityDkimAttributesRequestTypeDef](./type_defs.md#putemailidentitydkimattributesrequesttypedef) 

### put\_email\_identity\_dkim\_signing\_attributes

Used to configure or change the DKIM authentication settings for an email
domain identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_dkim_signing_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_email_identity_dkim_signing_attributes.html)

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

kwargs: PutEmailIdentityDkimSigningAttributesRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "SigningAttributesOrigin": ...,
}

parent.put_email_identity_dkim_signing_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityDkimSigningAttributesRequestTypeDef](./type_defs.md#putemailidentitydkimsigningattributesrequesttypedef) 

### put\_email\_identity\_feedback\_attributes

Used to enable or disable feedback forwarding for an identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_feedback_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_email_identity_feedback_attributes.html)

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

kwargs: PutEmailIdentityFeedbackAttributesRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_feedback_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityFeedbackAttributesRequestTypeDef](./type_defs.md#putemailidentityfeedbackattributesrequesttypedef) 

### put\_email\_identity\_mail\_from\_attributes

Used to enable or disable the custom Mail-From domain configuration for an
email identity.

Type annotations and code completion for `#!python session.create_client("sesv2").put_email_identity_mail_from_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_email_identity_mail_from_attributes.html)

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

kwargs: PutEmailIdentityMailFromAttributesRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
}

parent.put_email_identity_mail_from_attributes(**kwargs)
```

1. See [:material-code-braces: PutEmailIdentityMailFromAttributesRequestTypeDef](./type_defs.md#putemailidentitymailfromattributesrequesttypedef) 

### put\_suppressed\_destination

Adds an email address to the suppression list for your account.

Type annotations and code completion for `#!python session.create_client("sesv2").put_suppressed_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/put_suppressed_destination.html)

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

kwargs: PutSuppressedDestinationRequestTypeDef = {  # (1)
    "EmailAddress": ...,
    "Reason": ...,
}

parent.put_suppressed_destination(**kwargs)
```

1. See [:material-code-braces: PutSuppressedDestinationRequestTypeDef](./type_defs.md#putsuppresseddestinationrequesttypedef) 

### send\_bulk\_email

Composes an email message to multiple destinations.

Type annotations and code completion for `#!python session.create_client("sesv2").send_bulk_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/send_bulk_email.html)

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
    EndpointId: str = ...,
) -> SendBulkEmailResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: BulkEmailContentTypeDef](./type_defs.md#bulkemailcontenttypedef) 
2. See [:material-code-braces: BulkEmailEntryTypeDef](./type_defs.md#bulkemailentrytypedef) 
3. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
4. See [:material-code-braces: SendBulkEmailResponseTypeDef](./type_defs.md#sendbulkemailresponsetypedef) 


```python
# send_bulk_email method usage example with argument unpacking

kwargs: SendBulkEmailRequestTypeDef = {  # (1)
    "DefaultContent": ...,
    "BulkEmailEntries": ...,
}

parent.send_bulk_email(**kwargs)
```

1. See [:material-code-braces: SendBulkEmailRequestTypeDef](./type_defs.md#sendbulkemailrequesttypedef) 

### send\_custom\_verification\_email

Adds an email address to the list of identities for your Amazon SES account in
the current Amazon Web Services Region and attempts to verify it.

Type annotations and code completion for `#!python session.create_client("sesv2").send_custom_verification_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/send_custom_verification_email.html)

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

kwargs: SendCustomVerificationEmailRequestTypeDef = {  # (1)
    "EmailAddress": ...,
    "TemplateName": ...,
}

parent.send_custom_verification_email(**kwargs)
```

1. See [:material-code-braces: SendCustomVerificationEmailRequestTypeDef](./type_defs.md#sendcustomverificationemailrequesttypedef) 

### send\_email

Sends an email message.

Type annotations and code completion for `#!python session.create_client("sesv2").send_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/send_email.html)

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
    EndpointId: str = ...,
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

kwargs: SendEmailRequestTypeDef = {  # (1)
    "Content": ...,
}

parent.send_email(**kwargs)
```

1. See [:material-code-braces: SendEmailRequestTypeDef](./type_defs.md#sendemailrequesttypedef) 

### tag\_resource

Add one or more tags (keys and values) to a specified resource.

Type annotations and code completion for `#!python session.create_client("sesv2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/tag_resource.html)

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### test\_render\_email\_template

Creates a preview of the MIME content of an email when provided with a template
and a set of replacement data.

Type annotations and code completion for `#!python session.create_client("sesv2").test_render_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/test_render_email_template.html)

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

kwargs: TestRenderEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "TemplateData": ...,
}

parent.test_render_email_template(**kwargs)
```

1. See [:material-code-braces: TestRenderEmailTemplateRequestTypeDef](./type_defs.md#testrenderemailtemplaterequesttypedef) 

### untag\_resource

Remove one or more tags (keys and values) from a specified resource.

Type annotations and code completion for `#!python session.create_client("sesv2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/untag_resource.html)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_configuration\_set\_event\_destination

Update the configuration of an event destination for a configuration set.

Type annotations and code completion for `#!python session.create_client("sesv2").update_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/update_configuration_set_event_destination.html)

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

kwargs: UpdateConfigurationSetEventDestinationRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
    "EventDestination": ...,
}

parent.update_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationSetEventDestinationRequestTypeDef](./type_defs.md#updateconfigurationseteventdestinationrequesttypedef) 

### update\_contact

Updates a contact's preferences for a list.

Type annotations and code completion for `#!python session.create_client("sesv2").update_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/update_contact.html)

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

kwargs: UpdateContactRequestTypeDef = {  # (1)
    "ContactListName": ...,
    "EmailAddress": ...,
}

parent.update_contact(**kwargs)
```

1. See [:material-code-braces: UpdateContactRequestTypeDef](./type_defs.md#updatecontactrequesttypedef) 

### update\_contact\_list

Updates contact list metadata.

Type annotations and code completion for `#!python session.create_client("sesv2").update_contact_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/update_contact_list.html)

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

kwargs: UpdateContactListRequestTypeDef = {  # (1)
    "ContactListName": ...,
}

parent.update_contact_list(**kwargs)
```

1. See [:material-code-braces: UpdateContactListRequestTypeDef](./type_defs.md#updatecontactlistrequesttypedef) 

### update\_custom\_verification\_email\_template

Updates an existing custom verification email template.

Type annotations and code completion for `#!python session.create_client("sesv2").update_custom_verification_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/update_custom_verification_email_template.html)

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

kwargs: UpdateCustomVerificationEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "FromEmailAddress": ...,
    "TemplateSubject": ...,
    "TemplateContent": ...,
    "SuccessRedirectionURL": ...,
    "FailureRedirectionURL": ...,
}

parent.update_custom_verification_email_template(**kwargs)
```

1. See [:material-code-braces: UpdateCustomVerificationEmailTemplateRequestTypeDef](./type_defs.md#updatecustomverificationemailtemplaterequesttypedef) 

### update\_email\_identity\_policy

Updates the specified sending authorization policy for the given identity (an
email address or a domain).

Type annotations and code completion for `#!python session.create_client("sesv2").update_email_identity_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/update_email_identity_policy.html)

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

kwargs: UpdateEmailIdentityPolicyRequestTypeDef = {  # (1)
    "EmailIdentity": ...,
    "PolicyName": ...,
    "Policy": ...,
}

parent.update_email_identity_policy(**kwargs)
```

1. See [:material-code-braces: UpdateEmailIdentityPolicyRequestTypeDef](./type_defs.md#updateemailidentitypolicyrequesttypedef) 

### update\_email\_template

Updates an email template.

Type annotations and code completion for `#!python session.create_client("sesv2").update_email_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/client/update_email_template.html)

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

kwargs: UpdateEmailTemplateRequestTypeDef = {  # (1)
    "TemplateName": ...,
    "TemplateContent": ...,
}

parent.update_email_template(**kwargs)
```

1. See [:material-code-braces: UpdateEmailTemplateRequestTypeDef](./type_defs.md#updateemailtemplaterequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sesv2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sesv2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("sesv2").get_paginator` method with overloads.

- `client.get_paginator("list_multi_region_endpoints")` -> [ListMultiRegionEndpointsPaginator](./paginators.md#listmultiregionendpointspaginator)




<a id="sagemakerclient-for-aiobotocore-sagemaker-module"></a>

# SageMakerClient for aiobotocore SageMaker module

> [Index](..) > [SageMaker](.) > SageMakerClient

Auto-generated documentation for
[SageMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
type annotations stubs module
[types-aiobotocore-sagemaker](https://pypi.org/project/types-aiobotocore-sagemaker/).

- [SageMakerClient for aiobotocore SageMaker module](#sagemakerclient-for-aiobotocore-sagemaker-module)
  - [SageMakerClient](#sagemakerclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_association](#add_association)
    - [add_tags](#add_tags)
    - [associate_trial_component](#associate_trial_component)
    - [batch_describe_model_package](#batch_describe_model_package)
    - [can_paginate](#can_paginate)
    - [create_action](#create_action)
    - [create_algorithm](#create_algorithm)
    - [create_app](#create_app)
    - [create_app_image_config](#create_app_image_config)
    - [create_artifact](#create_artifact)
    - [create_auto_ml_job](#create_auto_ml_job)
    - [create_code_repository](#create_code_repository)
    - [create_compilation_job](#create_compilation_job)
    - [create_context](#create_context)
    - [create_data_quality_job_definition](#create_data_quality_job_definition)
    - [create_device_fleet](#create_device_fleet)
    - [create_domain](#create_domain)
    - [create_edge_packaging_job](#create_edge_packaging_job)
    - [create_endpoint](#create_endpoint)
    - [create_endpoint_config](#create_endpoint_config)
    - [create_experiment](#create_experiment)
    - [create_feature_group](#create_feature_group)
    - [create_flow_definition](#create_flow_definition)
    - [create_human_task_ui](#create_human_task_ui)
    - [create_hyper_parameter_tuning_job](#create_hyper_parameter_tuning_job)
    - [create_image](#create_image)
    - [create_image_version](#create_image_version)
    - [create_inference_recommendations_job](#create_inference_recommendations_job)
    - [create_labeling_job](#create_labeling_job)
    - [create_model](#create_model)
    - [create_model_bias_job_definition](#create_model_bias_job_definition)
    - [create_model_explainability_job_definition](#create_model_explainability_job_definition)
    - [create_model_package](#create_model_package)
    - [create_model_package_group](#create_model_package_group)
    - [create_model_quality_job_definition](#create_model_quality_job_definition)
    - [create_monitoring_schedule](#create_monitoring_schedule)
    - [create_notebook_instance](#create_notebook_instance)
    - [create_notebook_instance_lifecycle_config](#create_notebook_instance_lifecycle_config)
    - [create_pipeline](#create_pipeline)
    - [create_presigned_domain_url](#create_presigned_domain_url)
    - [create_presigned_notebook_instance_url](#create_presigned_notebook_instance_url)
    - [create_processing_job](#create_processing_job)
    - [create_project](#create_project)
    - [create_studio_lifecycle_config](#create_studio_lifecycle_config)
    - [create_training_job](#create_training_job)
    - [create_transform_job](#create_transform_job)
    - [create_trial](#create_trial)
    - [create_trial_component](#create_trial_component)
    - [create_user_profile](#create_user_profile)
    - [create_workforce](#create_workforce)
    - [create_workteam](#create_workteam)
    - [delete_action](#delete_action)
    - [delete_algorithm](#delete_algorithm)
    - [delete_app](#delete_app)
    - [delete_app_image_config](#delete_app_image_config)
    - [delete_artifact](#delete_artifact)
    - [delete_association](#delete_association)
    - [delete_code_repository](#delete_code_repository)
    - [delete_context](#delete_context)
    - [delete_data_quality_job_definition](#delete_data_quality_job_definition)
    - [delete_device_fleet](#delete_device_fleet)
    - [delete_domain](#delete_domain)
    - [delete_endpoint](#delete_endpoint)
    - [delete_endpoint_config](#delete_endpoint_config)
    - [delete_experiment](#delete_experiment)
    - [delete_feature_group](#delete_feature_group)
    - [delete_flow_definition](#delete_flow_definition)
    - [delete_human_task_ui](#delete_human_task_ui)
    - [delete_image](#delete_image)
    - [delete_image_version](#delete_image_version)
    - [delete_model](#delete_model)
    - [delete_model_bias_job_definition](#delete_model_bias_job_definition)
    - [delete_model_explainability_job_definition](#delete_model_explainability_job_definition)
    - [delete_model_package](#delete_model_package)
    - [delete_model_package_group](#delete_model_package_group)
    - [delete_model_package_group_policy](#delete_model_package_group_policy)
    - [delete_model_quality_job_definition](#delete_model_quality_job_definition)
    - [delete_monitoring_schedule](#delete_monitoring_schedule)
    - [delete_notebook_instance](#delete_notebook_instance)
    - [delete_notebook_instance_lifecycle_config](#delete_notebook_instance_lifecycle_config)
    - [delete_pipeline](#delete_pipeline)
    - [delete_project](#delete_project)
    - [delete_studio_lifecycle_config](#delete_studio_lifecycle_config)
    - [delete_tags](#delete_tags)
    - [delete_trial](#delete_trial)
    - [delete_trial_component](#delete_trial_component)
    - [delete_user_profile](#delete_user_profile)
    - [delete_workforce](#delete_workforce)
    - [delete_workteam](#delete_workteam)
    - [deregister_devices](#deregister_devices)
    - [describe_action](#describe_action)
    - [describe_algorithm](#describe_algorithm)
    - [describe_app](#describe_app)
    - [describe_app_image_config](#describe_app_image_config)
    - [describe_artifact](#describe_artifact)
    - [describe_auto_ml_job](#describe_auto_ml_job)
    - [describe_code_repository](#describe_code_repository)
    - [describe_compilation_job](#describe_compilation_job)
    - [describe_context](#describe_context)
    - [describe_data_quality_job_definition](#describe_data_quality_job_definition)
    - [describe_device](#describe_device)
    - [describe_device_fleet](#describe_device_fleet)
    - [describe_domain](#describe_domain)
    - [describe_edge_packaging_job](#describe_edge_packaging_job)
    - [describe_endpoint](#describe_endpoint)
    - [describe_endpoint_config](#describe_endpoint_config)
    - [describe_experiment](#describe_experiment)
    - [describe_feature_group](#describe_feature_group)
    - [describe_flow_definition](#describe_flow_definition)
    - [describe_human_task_ui](#describe_human_task_ui)
    - [describe_hyper_parameter_tuning_job](#describe_hyper_parameter_tuning_job)
    - [describe_image](#describe_image)
    - [describe_image_version](#describe_image_version)
    - [describe_inference_recommendations_job](#describe_inference_recommendations_job)
    - [describe_labeling_job](#describe_labeling_job)
    - [describe_lineage_group](#describe_lineage_group)
    - [describe_model](#describe_model)
    - [describe_model_bias_job_definition](#describe_model_bias_job_definition)
    - [describe_model_explainability_job_definition](#describe_model_explainability_job_definition)
    - [describe_model_package](#describe_model_package)
    - [describe_model_package_group](#describe_model_package_group)
    - [describe_model_quality_job_definition](#describe_model_quality_job_definition)
    - [describe_monitoring_schedule](#describe_monitoring_schedule)
    - [describe_notebook_instance](#describe_notebook_instance)
    - [describe_notebook_instance_lifecycle_config](#describe_notebook_instance_lifecycle_config)
    - [describe_pipeline](#describe_pipeline)
    - [describe_pipeline_definition_for_execution](#describe_pipeline_definition_for_execution)
    - [describe_pipeline_execution](#describe_pipeline_execution)
    - [describe_processing_job](#describe_processing_job)
    - [describe_project](#describe_project)
    - [describe_studio_lifecycle_config](#describe_studio_lifecycle_config)
    - [describe_subscribed_workteam](#describe_subscribed_workteam)
    - [describe_training_job](#describe_training_job)
    - [describe_transform_job](#describe_transform_job)
    - [describe_trial](#describe_trial)
    - [describe_trial_component](#describe_trial_component)
    - [describe_user_profile](#describe_user_profile)
    - [describe_workforce](#describe_workforce)
    - [describe_workteam](#describe_workteam)
    - [disable_sagemaker_servicecatalog_portfolio](#disable_sagemaker_servicecatalog_portfolio)
    - [disassociate_trial_component](#disassociate_trial_component)
    - [enable_sagemaker_servicecatalog_portfolio](#enable_sagemaker_servicecatalog_portfolio)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_device_fleet_report](#get_device_fleet_report)
    - [get_lineage_group_policy](#get_lineage_group_policy)
    - [get_model_package_group_policy](#get_model_package_group_policy)
    - [get_sagemaker_servicecatalog_portfolio_status](#get_sagemaker_servicecatalog_portfolio_status)
    - [get_search_suggestions](#get_search_suggestions)
    - [list_actions](#list_actions)
    - [list_algorithms](#list_algorithms)
    - [list_app_image_configs](#list_app_image_configs)
    - [list_apps](#list_apps)
    - [list_artifacts](#list_artifacts)
    - [list_associations](#list_associations)
    - [list_auto_ml_jobs](#list_auto_ml_jobs)
    - [list_candidates_for_auto_ml_job](#list_candidates_for_auto_ml_job)
    - [list_code_repositories](#list_code_repositories)
    - [list_compilation_jobs](#list_compilation_jobs)
    - [list_contexts](#list_contexts)
    - [list_data_quality_job_definitions](#list_data_quality_job_definitions)
    - [list_device_fleets](#list_device_fleets)
    - [list_devices](#list_devices)
    - [list_domains](#list_domains)
    - [list_edge_packaging_jobs](#list_edge_packaging_jobs)
    - [list_endpoint_configs](#list_endpoint_configs)
    - [list_endpoints](#list_endpoints)
    - [list_experiments](#list_experiments)
    - [list_feature_groups](#list_feature_groups)
    - [list_flow_definitions](#list_flow_definitions)
    - [list_human_task_uis](#list_human_task_uis)
    - [list_hyper_parameter_tuning_jobs](#list_hyper_parameter_tuning_jobs)
    - [list_image_versions](#list_image_versions)
    - [list_images](#list_images)
    - [list_inference_recommendations_jobs](#list_inference_recommendations_jobs)
    - [list_labeling_jobs](#list_labeling_jobs)
    - [list_labeling_jobs_for_workteam](#list_labeling_jobs_for_workteam)
    - [list_lineage_groups](#list_lineage_groups)
    - [list_model_bias_job_definitions](#list_model_bias_job_definitions)
    - [list_model_explainability_job_definitions](#list_model_explainability_job_definitions)
    - [list_model_metadata](#list_model_metadata)
    - [list_model_package_groups](#list_model_package_groups)
    - [list_model_packages](#list_model_packages)
    - [list_model_quality_job_definitions](#list_model_quality_job_definitions)
    - [list_models](#list_models)
    - [list_monitoring_executions](#list_monitoring_executions)
    - [list_monitoring_schedules](#list_monitoring_schedules)
    - [list_notebook_instance_lifecycle_configs](#list_notebook_instance_lifecycle_configs)
    - [list_notebook_instances](#list_notebook_instances)
    - [list_pipeline_execution_steps](#list_pipeline_execution_steps)
    - [list_pipeline_executions](#list_pipeline_executions)
    - [list_pipeline_parameters_for_execution](#list_pipeline_parameters_for_execution)
    - [list_pipelines](#list_pipelines)
    - [list_processing_jobs](#list_processing_jobs)
    - [list_projects](#list_projects)
    - [list_studio_lifecycle_configs](#list_studio_lifecycle_configs)
    - [list_subscribed_workteams](#list_subscribed_workteams)
    - [list_tags](#list_tags)
    - [list_training_jobs](#list_training_jobs)
    - [list_training_jobs_for_hyper_parameter_tuning_job](#list_training_jobs_for_hyper_parameter_tuning_job)
    - [list_transform_jobs](#list_transform_jobs)
    - [list_trial_components](#list_trial_components)
    - [list_trials](#list_trials)
    - [list_user_profiles](#list_user_profiles)
    - [list_workforces](#list_workforces)
    - [list_workteams](#list_workteams)
    - [put_model_package_group_policy](#put_model_package_group_policy)
    - [query_lineage](#query_lineage)
    - [register_devices](#register_devices)
    - [render_ui_template](#render_ui_template)
    - [retry_pipeline_execution](#retry_pipeline_execution)
    - [search](#search)
    - [send_pipeline_execution_step_failure](#send_pipeline_execution_step_failure)
    - [send_pipeline_execution_step_success](#send_pipeline_execution_step_success)
    - [start_monitoring_schedule](#start_monitoring_schedule)
    - [start_notebook_instance](#start_notebook_instance)
    - [start_pipeline_execution](#start_pipeline_execution)
    - [stop_auto_ml_job](#stop_auto_ml_job)
    - [stop_compilation_job](#stop_compilation_job)
    - [stop_edge_packaging_job](#stop_edge_packaging_job)
    - [stop_hyper_parameter_tuning_job](#stop_hyper_parameter_tuning_job)
    - [stop_inference_recommendations_job](#stop_inference_recommendations_job)
    - [stop_labeling_job](#stop_labeling_job)
    - [stop_monitoring_schedule](#stop_monitoring_schedule)
    - [stop_notebook_instance](#stop_notebook_instance)
    - [stop_pipeline_execution](#stop_pipeline_execution)
    - [stop_processing_job](#stop_processing_job)
    - [stop_training_job](#stop_training_job)
    - [stop_transform_job](#stop_transform_job)
    - [update_action](#update_action)
    - [update_app_image_config](#update_app_image_config)
    - [update_artifact](#update_artifact)
    - [update_code_repository](#update_code_repository)
    - [update_context](#update_context)
    - [update_device_fleet](#update_device_fleet)
    - [update_devices](#update_devices)
    - [update_domain](#update_domain)
    - [update_endpoint](#update_endpoint)
    - [update_endpoint_weights_and_capacities](#update_endpoint_weights_and_capacities)
    - [update_experiment](#update_experiment)
    - [update_image](#update_image)
    - [update_model_package](#update_model_package)
    - [update_monitoring_schedule](#update_monitoring_schedule)
    - [update_notebook_instance](#update_notebook_instance)
    - [update_notebook_instance_lifecycle_config](#update_notebook_instance_lifecycle_config)
    - [update_pipeline](#update_pipeline)
    - [update_pipeline_execution](#update_pipeline_execution)
    - [update_project](#update_project)
    - [update_training_job](#update_training_job)
    - [update_trial](#update_trial)
    - [update_trial_component](#update_trial_component)
    - [update_user_profile](#update_user_profile)
    - [update_workforce](#update_workforce)
    - [update_workteam](#update_workteam)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="sagemakerclient"></a>

## SageMakerClient

Type annotations for `aiobotocore.create_client("sagemaker")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_sagemaker.client import SageMakerClient

def get_sagemaker_client() -> SageMakerClient:
    return Session().client("sagemaker")
```

Boto3 documentation:
[SageMaker.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sagemaker.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.ResourceInUse`
- `Exceptions.ResourceLimitExceeded`
- `Exceptions.ResourceNotFound`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SageMakerClient exceptions.

Type annotations for `aiobotocore.create_client("sagemaker").exceptions`
method.

Boto3 documentation:
[SageMaker.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add_association"></a>

### add_association

Creates an *association* between the source and the destination.

Type annotations for `aiobotocore.create_client("sagemaker").add_association`
method.

Boto3 documentation:
[SageMaker.Client.add_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.add_association)

Asynchronous method. Use `await add_association(...)` for a synchronous call.

Arguments mapping described in
[AddAssociationRequestRequestTypeDef](./type_defs.md#addassociationrequestrequesttypedef).

Keyword-only arguments:

- `SourceArn`: `str` *(required)*
- `DestinationArn`: `str` *(required)*
- `AssociationType`:
  [AssociationEdgeTypeType](./literals.md#associationedgetypetype)

Returns a `Coroutine` for
[AddAssociationResponseTypeDef](./type_defs.md#addassociationresponsetypedef).

<a id="add_tags"></a>

### add_tags

Adds or overwrites one or more tags for the specified Amazon SageMaker
resource.

Type annotations for `aiobotocore.create_client("sagemaker").add_tags` method.

Boto3 documentation:
[SageMaker.Client.add_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.add_tags)

Asynchronous method. Use `await add_tags(...)` for a synchronous call.

Arguments mapping described in
[AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for
[AddTagsOutputTypeDef](./type_defs.md#addtagsoutputtypedef).

<a id="associate_trial_component"></a>

### associate_trial_component

Associates a trial component with a trial.

Type annotations for
`aiobotocore.create_client("sagemaker").associate_trial_component` method.

Boto3 documentation:
[SageMaker.Client.associate_trial_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.associate_trial_component)

Asynchronous method. Use `await associate_trial_component(...)` for a
synchronous call.

Arguments mapping described in
[AssociateTrialComponentRequestRequestTypeDef](./type_defs.md#associatetrialcomponentrequestrequesttypedef).

Keyword-only arguments:

- `TrialComponentName`: `str` *(required)*
- `TrialName`: `str` *(required)*

Returns a `Coroutine` for
[AssociateTrialComponentResponseTypeDef](./type_defs.md#associatetrialcomponentresponsetypedef).

<a id="batch_describe_model_package"></a>

### batch_describe_model_package

This action batch describes a list of versioned model packages See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/sagemaker-2017-07-24/BatchDescribeModelPackage).

Type annotations for
`aiobotocore.create_client("sagemaker").batch_describe_model_package` method.

Boto3 documentation:
[SageMaker.Client.batch_describe_model_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.batch_describe_model_package)

Asynchronous method. Use `await batch_describe_model_package(...)` for a
synchronous call.

Arguments mapping described in
[BatchDescribeModelPackageInputRequestTypeDef](./type_defs.md#batchdescribemodelpackageinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageArnList`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[BatchDescribeModelPackageOutputTypeDef](./type_defs.md#batchdescribemodelpackageoutputtypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("sagemaker").can_paginate`
method.

Boto3 documentation:
[SageMaker.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_action"></a>

### create_action

Creates an *action*.

Type annotations for `aiobotocore.create_client("sagemaker").create_action`
method.

Boto3 documentation:
[SageMaker.Client.create_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_action)

Asynchronous method. Use `await create_action(...)` for a synchronous call.

Arguments mapping described in
[CreateActionRequestRequestTypeDef](./type_defs.md#createactionrequestrequesttypedef).

Keyword-only arguments:

- `ActionName`: `str` *(required)*
- `Source`: [ActionSourceTypeDef](./type_defs.md#actionsourcetypedef)
  *(required)*
- `ActionType`: `str` *(required)*
- `Description`: `str`
- `Status`: [ActionStatusType](./literals.md#actionstatustype)
- `Properties`: `Mapping`\[`str`, `str`\]
- `MetadataProperties`:
  [MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateActionResponseTypeDef](./type_defs.md#createactionresponsetypedef).

<a id="create_algorithm"></a>

### create_algorithm

Create a machine learning algorithm that you can use in Amazon SageMaker and
list in the Amazon Web Services Marketplace.

Type annotations for `aiobotocore.create_client("sagemaker").create_algorithm`
method.

Boto3 documentation:
[SageMaker.Client.create_algorithm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_algorithm)

Asynchronous method. Use `await create_algorithm(...)` for a synchronous call.

Arguments mapping described in
[CreateAlgorithmInputRequestTypeDef](./type_defs.md#createalgorithminputrequesttypedef).

Keyword-only arguments:

- `AlgorithmName`: `str` *(required)*
- `TrainingSpecification`:
  [TrainingSpecificationTypeDef](./type_defs.md#trainingspecificationtypedef)
  *(required)*
- `AlgorithmDescription`: `str`
- `InferenceSpecification`:
  [InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef)
- `ValidationSpecification`:
  [AlgorithmValidationSpecificationTypeDef](./type_defs.md#algorithmvalidationspecificationtypedef)
- `CertifyForMarketplace`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateAlgorithmOutputTypeDef](./type_defs.md#createalgorithmoutputtypedef).

<a id="create_app"></a>

### create_app

Creates a running app for the specified UserProfile.

Type annotations for `aiobotocore.create_client("sagemaker").create_app`
method.

Boto3 documentation:
[SageMaker.Client.create_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app)

Asynchronous method. Use `await create_app(...)` for a synchronous call.

Arguments mapping described in
[CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*
- `AppType`: [AppTypeType](./literals.md#apptypetype) *(required)*
- `AppName`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ResourceSpec`: [ResourceSpecTypeDef](./type_defs.md#resourcespectypedef)

Returns a `Coroutine` for
[CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef).

<a id="create_app_image_config"></a>

### create_app_image_config

Creates a configuration for running a SageMaker image as a KernelGateway app.

Type annotations for
`aiobotocore.create_client("sagemaker").create_app_image_config` method.

Boto3 documentation:
[SageMaker.Client.create_app_image_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app_image_config)

Asynchronous method. Use `await create_app_image_config(...)` for a synchronous
call.

Arguments mapping described in
[CreateAppImageConfigRequestRequestTypeDef](./type_defs.md#createappimageconfigrequestrequesttypedef).

Keyword-only arguments:

- `AppImageConfigName`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `KernelGatewayImageConfig`:
  [KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef)

Returns a `Coroutine` for
[CreateAppImageConfigResponseTypeDef](./type_defs.md#createappimageconfigresponsetypedef).

<a id="create_artifact"></a>

### create_artifact

Creates an *artifact*.

Type annotations for `aiobotocore.create_client("sagemaker").create_artifact`
method.

Boto3 documentation:
[SageMaker.Client.create_artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_artifact)

Asynchronous method. Use `await create_artifact(...)` for a synchronous call.

Arguments mapping described in
[CreateArtifactRequestRequestTypeDef](./type_defs.md#createartifactrequestrequesttypedef).

Keyword-only arguments:

- `Source`: [ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef)
  *(required)*
- `ArtifactType`: `str` *(required)*
- `ArtifactName`: `str`
- `Properties`: `Mapping`\[`str`, `str`\]
- `MetadataProperties`:
  [MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateArtifactResponseTypeDef](./type_defs.md#createartifactresponsetypedef).

<a id="create_auto_ml_job"></a>

### create_auto_ml_job

Creates an Autopilot job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_auto_ml_job` method.

Boto3 documentation:
[SageMaker.Client.create_auto_ml_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job)

Asynchronous method. Use `await create_auto_ml_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateAutoMLJobRequestRequestTypeDef](./type_defs.md#createautomljobrequestrequesttypedef).

Keyword-only arguments:

- `AutoMLJobName`: `str` *(required)*
- `InputDataConfig`:
  `Sequence`\[[AutoMLChannelTypeDef](./type_defs.md#automlchanneltypedef)\]
  *(required)*
- `OutputDataConfig`:
  [AutoMLOutputDataConfigTypeDef](./type_defs.md#automloutputdataconfigtypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `ProblemType`: [ProblemTypeType](./literals.md#problemtypetype)
- `AutoMLJobObjective`:
  [AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef)
- `AutoMLJobConfig`:
  [AutoMLJobConfigTypeDef](./type_defs.md#automljobconfigtypedef)
- `GenerateCandidateDefinitionsOnly`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ModelDeployConfig`:
  [ModelDeployConfigTypeDef](./type_defs.md#modeldeployconfigtypedef)

Returns a `Coroutine` for
[CreateAutoMLJobResponseTypeDef](./type_defs.md#createautomljobresponsetypedef).

<a id="create_code_repository"></a>

### create_code_repository

Creates a Git repository as a resource in your Amazon SageMaker account.

Type annotations for
`aiobotocore.create_client("sagemaker").create_code_repository` method.

Boto3 documentation:
[SageMaker.Client.create_code_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_code_repository)

Asynchronous method. Use `await create_code_repository(...)` for a synchronous
call.

Arguments mapping described in
[CreateCodeRepositoryInputRequestTypeDef](./type_defs.md#createcoderepositoryinputrequesttypedef).

Keyword-only arguments:

- `CodeRepositoryName`: `str` *(required)*
- `GitConfig`: [GitConfigTypeDef](./type_defs.md#gitconfigtypedef) *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateCodeRepositoryOutputTypeDef](./type_defs.md#createcoderepositoryoutputtypedef).

<a id="create_compilation_job"></a>

### create_compilation_job

.

Type annotations for
`aiobotocore.create_client("sagemaker").create_compilation_job` method.

Boto3 documentation:
[SageMaker.Client.create_compilation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_compilation_job)

Asynchronous method. Use `await create_compilation_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateCompilationJobRequestRequestTypeDef](./type_defs.md#createcompilationjobrequestrequesttypedef).

Keyword-only arguments:

- `CompilationJobName`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `OutputConfig`: [OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
  *(required)*
- `StoppingCondition`:
  [StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef)
  *(required)*
- `ModelPackageVersionArn`: `str`
- `InputConfig`: [InputConfigTypeDef](./type_defs.md#inputconfigtypedef)
- `VpcConfig`: [NeoVpcConfigTypeDef](./type_defs.md#neovpcconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateCompilationJobResponseTypeDef](./type_defs.md#createcompilationjobresponsetypedef).

<a id="create_context"></a>

### create_context

Creates a *context*.

Type annotations for `aiobotocore.create_client("sagemaker").create_context`
method.

Boto3 documentation:
[SageMaker.Client.create_context](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_context)

Asynchronous method. Use `await create_context(...)` for a synchronous call.

Arguments mapping described in
[CreateContextRequestRequestTypeDef](./type_defs.md#createcontextrequestrequesttypedef).

Keyword-only arguments:

- `ContextName`: `str` *(required)*
- `Source`: [ContextSourceTypeDef](./type_defs.md#contextsourcetypedef)
  *(required)*
- `ContextType`: `str` *(required)*
- `Description`: `str`
- `Properties`: `Mapping`\[`str`, `str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateContextResponseTypeDef](./type_defs.md#createcontextresponsetypedef).

<a id="create_data_quality_job_definition"></a>

### create_data_quality_job_definition

Creates a definition for a job that monitors data quality and drift.

Type annotations for
`aiobotocore.create_client("sagemaker").create_data_quality_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.create_data_quality_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_data_quality_job_definition)

Asynchronous method. Use `await create_data_quality_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[CreateDataQualityJobDefinitionRequestRequestTypeDef](./type_defs.md#createdataqualityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*
- `DataQualityAppSpecification`:
  [DataQualityAppSpecificationTypeDef](./type_defs.md#dataqualityappspecificationtypedef)
  *(required)*
- `DataQualityJobInput`:
  [DataQualityJobInputTypeDef](./type_defs.md#dataqualityjobinputtypedef)
  *(required)*
- `DataQualityJobOutputConfig`:
  [MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef)
  *(required)*
- `JobResources`:
  [MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `DataQualityBaselineConfig`:
  [DataQualityBaselineConfigTypeDef](./type_defs.md#dataqualitybaselineconfigtypedef)
- `NetworkConfig`:
  [MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef)
- `StoppingCondition`:
  [MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDataQualityJobDefinitionResponseTypeDef](./type_defs.md#createdataqualityjobdefinitionresponsetypedef).

<a id="create_device_fleet"></a>

### create_device_fleet

Creates a device fleet.

Type annotations for
`aiobotocore.create_client("sagemaker").create_device_fleet` method.

Boto3 documentation:
[SageMaker.Client.create_device_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_device_fleet)

Asynchronous method. Use `await create_device_fleet(...)` for a synchronous
call.

Arguments mapping described in
[CreateDeviceFleetRequestRequestTypeDef](./type_defs.md#createdevicefleetrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*
- `OutputConfig`:
  [EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef)
  *(required)*
- `RoleArn`: `str`
- `Description`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `EnableIotRoleAlias`: `bool`

<a id="create_domain"></a>

### create_domain

Creates a `Domain` used by Amazon SageMaker Studio.

Type annotations for `aiobotocore.create_client("sagemaker").create_domain`
method.

Boto3 documentation:
[SageMaker.Client.create_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_domain)

Asynchronous method. Use `await create_domain(...)` for a synchronous call.

Arguments mapping described in
[CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*
- `AuthMode`: [AuthModeType](./literals.md#authmodetype) *(required)*
- `DefaultUserSettings`:
  [UserSettingsTypeDef](./type_defs.md#usersettingstypedef) *(required)*
- `SubnetIds`: `Sequence`\[`str`\] *(required)*
- `VpcId`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `AppNetworkAccessType`:
  [AppNetworkAccessTypeType](./literals.md#appnetworkaccesstypetype)
- `HomeEfsFileSystemKmsKeyId`: `str`
- `KmsKeyId`: `str`
- `AppSecurityGroupManagement`:
  [AppSecurityGroupManagementType](./literals.md#appsecuritygroupmanagementtype)
- `DomainSettings`:
  [DomainSettingsTypeDef](./type_defs.md#domainsettingstypedef)

Returns a `Coroutine` for
[CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef).

<a id="create_edge_packaging_job"></a>

### create_edge_packaging_job

Starts a SageMaker Edge Manager model packaging job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_edge_packaging_job` method.

Boto3 documentation:
[SageMaker.Client.create_edge_packaging_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_edge_packaging_job)

Asynchronous method. Use `await create_edge_packaging_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateEdgePackagingJobRequestRequestTypeDef](./type_defs.md#createedgepackagingjobrequestrequesttypedef).

Keyword-only arguments:

- `EdgePackagingJobName`: `str` *(required)*
- `CompilationJobName`: `str` *(required)*
- `ModelName`: `str` *(required)*
- `ModelVersion`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `OutputConfig`:
  [EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef)
  *(required)*
- `ResourceKey`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="create_endpoint"></a>

### create_endpoint

.

Type annotations for `aiobotocore.create_client("sagemaker").create_endpoint`
method.

Boto3 documentation:
[SageMaker.Client.create_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint)

Asynchronous method. Use `await create_endpoint(...)` for a synchronous call.

Arguments mapping described in
[CreateEndpointInputRequestTypeDef](./type_defs.md#createendpointinputrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str` *(required)*
- `EndpointConfigName`: `str` *(required)*
- `DeploymentConfig`:
  [DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateEndpointOutputTypeDef](./type_defs.md#createendpointoutputtypedef).

<a id="create_endpoint_config"></a>

### create_endpoint_config

.

Type annotations for
`aiobotocore.create_client("sagemaker").create_endpoint_config` method.

Boto3 documentation:
[SageMaker.Client.create_endpoint_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint_config)

Asynchronous method. Use `await create_endpoint_config(...)` for a synchronous
call.

Arguments mapping described in
[CreateEndpointConfigInputRequestTypeDef](./type_defs.md#createendpointconfiginputrequesttypedef).

Keyword-only arguments:

- `EndpointConfigName`: `str` *(required)*
- `ProductionVariants`:
  `Sequence`\[[ProductionVariantTypeDef](./type_defs.md#productionvarianttypedef)\]
  *(required)*
- `DataCaptureConfig`:
  [DataCaptureConfigTypeDef](./type_defs.md#datacaptureconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `KmsKeyId`: `str`
- `AsyncInferenceConfig`:
  [AsyncInferenceConfigTypeDef](./type_defs.md#asyncinferenceconfigtypedef)

Returns a `Coroutine` for
[CreateEndpointConfigOutputTypeDef](./type_defs.md#createendpointconfigoutputtypedef).

<a id="create_experiment"></a>

### create_experiment

Creates an SageMaker *experiment*.

Type annotations for `aiobotocore.create_client("sagemaker").create_experiment`
method.

Boto3 documentation:
[SageMaker.Client.create_experiment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_experiment)

Asynchronous method. Use `await create_experiment(...)` for a synchronous call.

Arguments mapping described in
[CreateExperimentRequestRequestTypeDef](./type_defs.md#createexperimentrequestrequesttypedef).

Keyword-only arguments:

- `ExperimentName`: `str` *(required)*
- `DisplayName`: `str`
- `Description`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateExperimentResponseTypeDef](./type_defs.md#createexperimentresponsetypedef).

<a id="create_feature_group"></a>

### create_feature_group

Create a new `FeatureGroup`.

Type annotations for
`aiobotocore.create_client("sagemaker").create_feature_group` method.

Boto3 documentation:
[SageMaker.Client.create_feature_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_feature_group)

Asynchronous method. Use `await create_feature_group(...)` for a synchronous
call.

Arguments mapping described in
[CreateFeatureGroupRequestRequestTypeDef](./type_defs.md#createfeaturegrouprequestrequesttypedef).

Keyword-only arguments:

- `FeatureGroupName`: `str` *(required)*
- `RecordIdentifierFeatureName`: `str` *(required)*
- `EventTimeFeatureName`: `str` *(required)*
- `FeatureDefinitions`:
  `Sequence`\[[FeatureDefinitionTypeDef](./type_defs.md#featuredefinitiontypedef)\]
  *(required)*
- `OnlineStoreConfig`:
  [OnlineStoreConfigTypeDef](./type_defs.md#onlinestoreconfigtypedef)
- `OfflineStoreConfig`:
  [OfflineStoreConfigTypeDef](./type_defs.md#offlinestoreconfigtypedef)
- `RoleArn`: `str`
- `Description`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateFeatureGroupResponseTypeDef](./type_defs.md#createfeaturegroupresponsetypedef).

<a id="create_flow_definition"></a>

### create_flow_definition

Creates a flow definition.

Type annotations for
`aiobotocore.create_client("sagemaker").create_flow_definition` method.

Boto3 documentation:
[SageMaker.Client.create_flow_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_flow_definition)

Asynchronous method. Use `await create_flow_definition(...)` for a synchronous
call.

Arguments mapping described in
[CreateFlowDefinitionRequestRequestTypeDef](./type_defs.md#createflowdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `FlowDefinitionName`: `str` *(required)*
- `HumanLoopConfig`:
  [HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) *(required)*
- `OutputConfig`:
  [FlowDefinitionOutputConfigTypeDef](./type_defs.md#flowdefinitionoutputconfigtypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `HumanLoopRequestSource`:
  [HumanLoopRequestSourceTypeDef](./type_defs.md#humanlooprequestsourcetypedef)
- `HumanLoopActivationConfig`:
  [HumanLoopActivationConfigTypeDef](./type_defs.md#humanloopactivationconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateFlowDefinitionResponseTypeDef](./type_defs.md#createflowdefinitionresponsetypedef).

<a id="create_human_task_ui"></a>

### create_human_task_ui

Defines the settings you will use for the human review workflow user interface.

Type annotations for
`aiobotocore.create_client("sagemaker").create_human_task_ui` method.

Boto3 documentation:
[SageMaker.Client.create_human_task_ui](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_human_task_ui)

Asynchronous method. Use `await create_human_task_ui(...)` for a synchronous
call.

Arguments mapping described in
[CreateHumanTaskUiRequestRequestTypeDef](./type_defs.md#createhumantaskuirequestrequesttypedef).

Keyword-only arguments:

- `HumanTaskUiName`: `str` *(required)*
- `UiTemplate`: [UiTemplateTypeDef](./type_defs.md#uitemplatetypedef)
  *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateHumanTaskUiResponseTypeDef](./type_defs.md#createhumantaskuiresponsetypedef).

<a id="create_hyper_parameter_tuning_job"></a>

### create_hyper_parameter_tuning_job

Starts a hyperparameter tuning job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_hyper_parameter_tuning_job`
method.

Boto3 documentation:
[SageMaker.Client.create_hyper_parameter_tuning_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hyper_parameter_tuning_job)

Asynchronous method. Use `await create_hyper_parameter_tuning_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateHyperParameterTuningJobRequestRequestTypeDef](./type_defs.md#createhyperparametertuningjobrequestrequesttypedef).

Keyword-only arguments:

- `HyperParameterTuningJobName`: `str` *(required)*
- `HyperParameterTuningJobConfig`:
  [HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef)
  *(required)*
- `TrainingJobDefinition`:
  [HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef)
- `TrainingJobDefinitions`:
  `Sequence`\[[HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef)\]
- `WarmStartConfig`:
  [HyperParameterTuningJobWarmStartConfigTypeDef](./type_defs.md#hyperparametertuningjobwarmstartconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateHyperParameterTuningJobResponseTypeDef](./type_defs.md#createhyperparametertuningjobresponsetypedef).

<a id="create_image"></a>

### create_image

Creates a custom SageMaker image.

Type annotations for `aiobotocore.create_client("sagemaker").create_image`
method.

Boto3 documentation:
[SageMaker.Client.create_image](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_image)

Asynchronous method. Use `await create_image(...)` for a synchronous call.

Arguments mapping described in
[CreateImageRequestRequestTypeDef](./type_defs.md#createimagerequestrequesttypedef).

Keyword-only arguments:

- `ImageName`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `Description`: `str`
- `DisplayName`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateImageResponseTypeDef](./type_defs.md#createimageresponsetypedef).

<a id="create_image_version"></a>

### create_image_version

Creates a version of the SageMaker image specified by `ImageName`.

Type annotations for
`aiobotocore.create_client("sagemaker").create_image_version` method.

Boto3 documentation:
[SageMaker.Client.create_image_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_image_version)

Asynchronous method. Use `await create_image_version(...)` for a synchronous
call.

Arguments mapping described in
[CreateImageVersionRequestRequestTypeDef](./type_defs.md#createimageversionrequestrequesttypedef).

Keyword-only arguments:

- `BaseImage`: `str` *(required)*
- `ClientToken`: `str` *(required)*
- `ImageName`: `str` *(required)*

Returns a `Coroutine` for
[CreateImageVersionResponseTypeDef](./type_defs.md#createimageversionresponsetypedef).

<a id="create_inference_recommendations_job"></a>

### create_inference_recommendations_job

Starts a recommendation job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_inference_recommendations_job`
method.

Boto3 documentation:
[SageMaker.Client.create_inference_recommendations_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_recommendations_job)

Asynchronous method. Use `await create_inference_recommendations_job(...)` for
a synchronous call.

Arguments mapping described in
[CreateInferenceRecommendationsJobRequestRequestTypeDef](./type_defs.md#createinferencerecommendationsjobrequestrequesttypedef).

Keyword-only arguments:

- `JobName`: `str` *(required)*
- `JobType`:
  [RecommendationJobTypeType](./literals.md#recommendationjobtypetype)
  *(required)*
- `RoleArn`: `str` *(required)*
- `InputConfig`:
  [RecommendationJobInputConfigTypeDef](./type_defs.md#recommendationjobinputconfigtypedef)
  *(required)*
- `JobDescription`: `str`
- `StoppingConditions`:
  [RecommendationJobStoppingConditionsTypeDef](./type_defs.md#recommendationjobstoppingconditionstypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateInferenceRecommendationsJobResponseTypeDef](./type_defs.md#createinferencerecommendationsjobresponsetypedef).

<a id="create_labeling_job"></a>

### create_labeling_job

.

Type annotations for
`aiobotocore.create_client("sagemaker").create_labeling_job` method.

Boto3 documentation:
[SageMaker.Client.create_labeling_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_labeling_job)

Asynchronous method. Use `await create_labeling_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateLabelingJobRequestRequestTypeDef](./type_defs.md#createlabelingjobrequestrequesttypedef).

Keyword-only arguments:

- `LabelingJobName`: `str` *(required)*
- `LabelAttributeName`: `str` *(required)*
- `InputConfig`:
  [LabelingJobInputConfigTypeDef](./type_defs.md#labelingjobinputconfigtypedef)
  *(required)*
- `OutputConfig`:
  [LabelingJobOutputConfigTypeDef](./type_defs.md#labelingjoboutputconfigtypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `HumanTaskConfig`:
  [HumanTaskConfigTypeDef](./type_defs.md#humantaskconfigtypedef) *(required)*
- `LabelCategoryConfigS3Uri`: `str`
- `StoppingConditions`:
  [LabelingJobStoppingConditionsTypeDef](./type_defs.md#labelingjobstoppingconditionstypedef)
- `LabelingJobAlgorithmsConfig`:
  [LabelingJobAlgorithmsConfigTypeDef](./type_defs.md#labelingjobalgorithmsconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateLabelingJobResponseTypeDef](./type_defs.md#createlabelingjobresponsetypedef).

<a id="create_model"></a>

### create_model

Creates a model in Amazon SageMaker.

Type annotations for `aiobotocore.create_client("sagemaker").create_model`
method.

Boto3 documentation:
[SageMaker.Client.create_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model)

Asynchronous method. Use `await create_model(...)` for a synchronous call.

Arguments mapping described in
[CreateModelInputRequestTypeDef](./type_defs.md#createmodelinputrequesttypedef).

Keyword-only arguments:

- `ModelName`: `str` *(required)*
- `ExecutionRoleArn`: `str` *(required)*
- `PrimaryContainer`:
  [ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef)
- `Containers`:
  `Sequence`\[[ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef)\]
- `InferenceExecutionConfig`:
  [InferenceExecutionConfigTypeDef](./type_defs.md#inferenceexecutionconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `VpcConfig`: [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- `EnableNetworkIsolation`: `bool`

Returns a `Coroutine` for
[CreateModelOutputTypeDef](./type_defs.md#createmodeloutputtypedef).

<a id="create_model_bias_job_definition"></a>

### create_model_bias_job_definition

Creates the definition for a model bias job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_model_bias_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.create_model_bias_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_bias_job_definition)

Asynchronous method. Use `await create_model_bias_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[CreateModelBiasJobDefinitionRequestRequestTypeDef](./type_defs.md#createmodelbiasjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*
- `ModelBiasAppSpecification`:
  [ModelBiasAppSpecificationTypeDef](./type_defs.md#modelbiasappspecificationtypedef)
  *(required)*
- `ModelBiasJobInput`:
  [ModelBiasJobInputTypeDef](./type_defs.md#modelbiasjobinputtypedef)
  *(required)*
- `ModelBiasJobOutputConfig`:
  [MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef)
  *(required)*
- `JobResources`:
  [MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `ModelBiasBaselineConfig`:
  [ModelBiasBaselineConfigTypeDef](./type_defs.md#modelbiasbaselineconfigtypedef)
- `NetworkConfig`:
  [MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef)
- `StoppingCondition`:
  [MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateModelBiasJobDefinitionResponseTypeDef](./type_defs.md#createmodelbiasjobdefinitionresponsetypedef).

<a id="create_model_explainability_job_definition"></a>

### create_model_explainability_job_definition

Creates the definition for a model explainability job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_model_explainability_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.create_model_explainability_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_explainability_job_definition)

Asynchronous method. Use
`await create_model_explainability_job_definition(...)` for a synchronous call.

Arguments mapping described in
[CreateModelExplainabilityJobDefinitionRequestRequestTypeDef](./type_defs.md#createmodelexplainabilityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*
- `ModelExplainabilityAppSpecification`:
  [ModelExplainabilityAppSpecificationTypeDef](./type_defs.md#modelexplainabilityappspecificationtypedef)
  *(required)*
- `ModelExplainabilityJobInput`:
  [ModelExplainabilityJobInputTypeDef](./type_defs.md#modelexplainabilityjobinputtypedef)
  *(required)*
- `ModelExplainabilityJobOutputConfig`:
  [MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef)
  *(required)*
- `JobResources`:
  [MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `ModelExplainabilityBaselineConfig`:
  [ModelExplainabilityBaselineConfigTypeDef](./type_defs.md#modelexplainabilitybaselineconfigtypedef)
- `NetworkConfig`:
  [MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef)
- `StoppingCondition`:
  [MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateModelExplainabilityJobDefinitionResponseTypeDef](./type_defs.md#createmodelexplainabilityjobdefinitionresponsetypedef).

<a id="create_model_package"></a>

### create_model_package

Creates a model package that you can use to create Amazon SageMaker models or
list on Amazon Web Services Marketplace, or a versioned model that is part of a
model group.

Type annotations for
`aiobotocore.create_client("sagemaker").create_model_package` method.

Boto3 documentation:
[SageMaker.Client.create_model_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_package)

Asynchronous method. Use `await create_model_package(...)` for a synchronous
call.

Arguments mapping described in
[CreateModelPackageInputRequestTypeDef](./type_defs.md#createmodelpackageinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageName`: `str`
- `ModelPackageGroupName`: `str`
- `ModelPackageDescription`: `str`
- `InferenceSpecification`:
  [InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef)
- `ValidationSpecification`:
  [ModelPackageValidationSpecificationTypeDef](./type_defs.md#modelpackagevalidationspecificationtypedef)
- `SourceAlgorithmSpecification`:
  [SourceAlgorithmSpecificationTypeDef](./type_defs.md#sourcealgorithmspecificationtypedef)
- `CertifyForMarketplace`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ModelApprovalStatus`:
  [ModelApprovalStatusType](./literals.md#modelapprovalstatustype)
- `MetadataProperties`:
  [MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef)
- `ModelMetrics`: [ModelMetricsTypeDef](./type_defs.md#modelmetricstypedef)
- `ClientToken`: `str`
- `CustomerMetadataProperties`: `Mapping`\[`str`, `str`\]
- `DriftCheckBaselines`:
  [DriftCheckBaselinesTypeDef](./type_defs.md#driftcheckbaselinestypedef)
- `Domain`: `str`
- `Task`: `str`
- `SamplePayloadUrl`: `str`
- `AdditionalInferenceSpecifications`:
  `Sequence`\[[AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef)\]

Returns a `Coroutine` for
[CreateModelPackageOutputTypeDef](./type_defs.md#createmodelpackageoutputtypedef).

<a id="create_model_package_group"></a>

### create_model_package_group

Creates a model group.

Type annotations for
`aiobotocore.create_client("sagemaker").create_model_package_group` method.

Boto3 documentation:
[SageMaker.Client.create_model_package_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_package_group)

Asynchronous method. Use `await create_model_package_group(...)` for a
synchronous call.

Arguments mapping described in
[CreateModelPackageGroupInputRequestTypeDef](./type_defs.md#createmodelpackagegroupinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageGroupName`: `str` *(required)*
- `ModelPackageGroupDescription`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateModelPackageGroupOutputTypeDef](./type_defs.md#createmodelpackagegroupoutputtypedef).

<a id="create_model_quality_job_definition"></a>

### create_model_quality_job_definition

Creates a definition for a job that monitors model quality and drift.

Type annotations for
`aiobotocore.create_client("sagemaker").create_model_quality_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.create_model_quality_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_quality_job_definition)

Asynchronous method. Use `await create_model_quality_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[CreateModelQualityJobDefinitionRequestRequestTypeDef](./type_defs.md#createmodelqualityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*
- `ModelQualityAppSpecification`:
  [ModelQualityAppSpecificationTypeDef](./type_defs.md#modelqualityappspecificationtypedef)
  *(required)*
- `ModelQualityJobInput`:
  [ModelQualityJobInputTypeDef](./type_defs.md#modelqualityjobinputtypedef)
  *(required)*
- `ModelQualityJobOutputConfig`:
  [MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef)
  *(required)*
- `JobResources`:
  [MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `ModelQualityBaselineConfig`:
  [ModelQualityBaselineConfigTypeDef](./type_defs.md#modelqualitybaselineconfigtypedef)
- `NetworkConfig`:
  [MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef)
- `StoppingCondition`:
  [MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateModelQualityJobDefinitionResponseTypeDef](./type_defs.md#createmodelqualityjobdefinitionresponsetypedef).

<a id="create_monitoring_schedule"></a>

### create_monitoring_schedule

Creates a schedule that regularly starts Amazon SageMaker Processing Jobs to
monitor the data captured for an Amazon SageMaker Endoint.

Type annotations for
`aiobotocore.create_client("sagemaker").create_monitoring_schedule` method.

Boto3 documentation:
[SageMaker.Client.create_monitoring_schedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_monitoring_schedule)

Asynchronous method. Use `await create_monitoring_schedule(...)` for a
synchronous call.

Arguments mapping described in
[CreateMonitoringScheduleRequestRequestTypeDef](./type_defs.md#createmonitoringschedulerequestrequesttypedef).

Keyword-only arguments:

- `MonitoringScheduleName`: `str` *(required)*
- `MonitoringScheduleConfig`:
  [MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef)
  *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateMonitoringScheduleResponseTypeDef](./type_defs.md#createmonitoringscheduleresponsetypedef).

<a id="create_notebook_instance"></a>

### create_notebook_instance

Creates an Amazon SageMaker notebook instance.

Type annotations for
`aiobotocore.create_client("sagemaker").create_notebook_instance` method.

Boto3 documentation:
[SageMaker.Client.create_notebook_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_notebook_instance)

Asynchronous method. Use `await create_notebook_instance(...)` for a
synchronous call.

Arguments mapping described in
[CreateNotebookInstanceInputRequestTypeDef](./type_defs.md#createnotebookinstanceinputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceName`: `str` *(required)*
- `InstanceType`: [InstanceTypeType](./literals.md#instancetypetype)
  *(required)*
- `RoleArn`: `str` *(required)*
- `SubnetId`: `str`
- `SecurityGroupIds`: `Sequence`\[`str`\]
- `KmsKeyId`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `LifecycleConfigName`: `str`
- `DirectInternetAccess`:
  [DirectInternetAccessType](./literals.md#directinternetaccesstype)
- `VolumeSizeInGB`: `int`
- `AcceleratorTypes`:
  `Sequence`\[[NotebookInstanceAcceleratorTypeType](./literals.md#notebookinstanceacceleratortypetype)\]
- `DefaultCodeRepository`: `str`
- `AdditionalCodeRepositories`: `Sequence`\[`str`\]
- `RootAccess`: [RootAccessType](./literals.md#rootaccesstype)
- `PlatformIdentifier`: `str`

Returns a `Coroutine` for
[CreateNotebookInstanceOutputTypeDef](./type_defs.md#createnotebookinstanceoutputtypedef).

<a id="create_notebook_instance_lifecycle_config"></a>

### create_notebook_instance_lifecycle_config

Creates a lifecycle configuration that you can associate with a notebook
instance.

Type annotations for
`aiobotocore.create_client("sagemaker").create_notebook_instance_lifecycle_config`
method.

Boto3 documentation:
[SageMaker.Client.create_notebook_instance_lifecycle_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_notebook_instance_lifecycle_config)

Asynchronous method. Use `await create_notebook_instance_lifecycle_config(...)`
for a synchronous call.

Arguments mapping described in
[CreateNotebookInstanceLifecycleConfigInputRequestTypeDef](./type_defs.md#createnotebookinstancelifecycleconfiginputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceLifecycleConfigName`: `str` *(required)*
- `OnCreate`:
  `Sequence`\[[NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef)\]
- `OnStart`:
  `Sequence`\[[NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef)\]

Returns a `Coroutine` for
[CreateNotebookInstanceLifecycleConfigOutputTypeDef](./type_defs.md#createnotebookinstancelifecycleconfigoutputtypedef).

<a id="create_pipeline"></a>

### create_pipeline

Creates a pipeline using a JSON pipeline definition.

Type annotations for `aiobotocore.create_client("sagemaker").create_pipeline`
method.

Boto3 documentation:
[SageMaker.Client.create_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_pipeline)

Asynchronous method. Use `await create_pipeline(...)` for a synchronous call.

Arguments mapping described in
[CreatePipelineRequestRequestTypeDef](./type_defs.md#createpipelinerequestrequesttypedef).

Keyword-only arguments:

- `PipelineName`: `str` *(required)*
- `PipelineDefinition`: `str` *(required)*
- `ClientRequestToken`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `PipelineDisplayName`: `str`
- `PipelineDescription`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef).

<a id="create_presigned_domain_url"></a>

### create_presigned_domain_url

Creates a URL for a specified UserProfile in a Domain.

Type annotations for
`aiobotocore.create_client("sagemaker").create_presigned_domain_url` method.

Boto3 documentation:
[SageMaker.Client.create_presigned_domain_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_presigned_domain_url)

Asynchronous method. Use `await create_presigned_domain_url(...)` for a
synchronous call.

Arguments mapping described in
[CreatePresignedDomainUrlRequestRequestTypeDef](./type_defs.md#createpresigneddomainurlrequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*
- `SessionExpirationDurationInSeconds`: `int`
- `ExpiresInSeconds`: `int`

Returns a `Coroutine` for
[CreatePresignedDomainUrlResponseTypeDef](./type_defs.md#createpresigneddomainurlresponsetypedef).

<a id="create_presigned_notebook_instance_url"></a>

### create_presigned_notebook_instance_url

Returns a URL that you can use to connect to the Jupyter server from a notebook
instance.

Type annotations for
`aiobotocore.create_client("sagemaker").create_presigned_notebook_instance_url`
method.

Boto3 documentation:
[SageMaker.Client.create_presigned_notebook_instance_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_presigned_notebook_instance_url)

Asynchronous method. Use `await create_presigned_notebook_instance_url(...)`
for a synchronous call.

Arguments mapping described in
[CreatePresignedNotebookInstanceUrlInputRequestTypeDef](./type_defs.md#createpresignednotebookinstanceurlinputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceName`: `str` *(required)*
- `SessionExpirationDurationInSeconds`: `int`

Returns a `Coroutine` for
[CreatePresignedNotebookInstanceUrlOutputTypeDef](./type_defs.md#createpresignednotebookinstanceurloutputtypedef).

<a id="create_processing_job"></a>

### create_processing_job

Creates a processing job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_processing_job` method.

Boto3 documentation:
[SageMaker.Client.create_processing_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_processing_job)

Asynchronous method. Use `await create_processing_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateProcessingJobRequestRequestTypeDef](./type_defs.md#createprocessingjobrequestrequesttypedef).

Keyword-only arguments:

- `ProcessingJobName`: `str` *(required)*
- `ProcessingResources`:
  [ProcessingResourcesTypeDef](./type_defs.md#processingresourcestypedef)
  *(required)*
- `AppSpecification`:
  [AppSpecificationTypeDef](./type_defs.md#appspecificationtypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `ProcessingInputs`:
  `Sequence`\[[ProcessingInputTypeDef](./type_defs.md#processinginputtypedef)\]
- `ProcessingOutputConfig`:
  [ProcessingOutputConfigTypeDef](./type_defs.md#processingoutputconfigtypedef)
- `StoppingCondition`:
  [ProcessingStoppingConditionTypeDef](./type_defs.md#processingstoppingconditiontypedef)
- `Environment`: `Mapping`\[`str`, `str`\]
- `NetworkConfig`: [NetworkConfigTypeDef](./type_defs.md#networkconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ExperimentConfig`:
  [ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef)

Returns a `Coroutine` for
[CreateProcessingJobResponseTypeDef](./type_defs.md#createprocessingjobresponsetypedef).

<a id="create_project"></a>

### create_project

Creates a machine learning (ML) project that can contain one or more templates
that set up an ML pipeline from training to deploying an approved model.

Type annotations for `aiobotocore.create_client("sagemaker").create_project`
method.

Boto3 documentation:
[SageMaker.Client.create_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_project)

Asynchronous method. Use `await create_project(...)` for a synchronous call.

Arguments mapping described in
[CreateProjectInputRequestTypeDef](./type_defs.md#createprojectinputrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ServiceCatalogProvisioningDetails`:
  [ServiceCatalogProvisioningDetailsTypeDef](./type_defs.md#servicecatalogprovisioningdetailstypedef)
  *(required)*
- `ProjectDescription`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateProjectOutputTypeDef](./type_defs.md#createprojectoutputtypedef).

<a id="create_studio_lifecycle_config"></a>

### create_studio_lifecycle_config

Creates a new Studio Lifecycle Configuration.

Type annotations for
`aiobotocore.create_client("sagemaker").create_studio_lifecycle_config` method.

Boto3 documentation:
[SageMaker.Client.create_studio_lifecycle_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_studio_lifecycle_config)

Asynchronous method. Use `await create_studio_lifecycle_config(...)` for a
synchronous call.

Arguments mapping described in
[CreateStudioLifecycleConfigRequestRequestTypeDef](./type_defs.md#createstudiolifecycleconfigrequestrequesttypedef).

Keyword-only arguments:

- `StudioLifecycleConfigName`: `str` *(required)*
- `StudioLifecycleConfigContent`: `str` *(required)*
- `StudioLifecycleConfigAppType`:
  [StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype)
  *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateStudioLifecycleConfigResponseTypeDef](./type_defs.md#createstudiolifecycleconfigresponsetypedef).

<a id="create_training_job"></a>

### create_training_job

Starts a model training job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_training_job` method.

Boto3 documentation:
[SageMaker.Client.create_training_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_training_job)

Asynchronous method. Use `await create_training_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateTrainingJobRequestRequestTypeDef](./type_defs.md#createtrainingjobrequestrequesttypedef).

Keyword-only arguments:

- `TrainingJobName`: `str` *(required)*
- `AlgorithmSpecification`:
  [AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `OutputDataConfig`:
  [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
  *(required)*
- `ResourceConfig`:
  [ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) *(required)*
- `StoppingCondition`:
  [StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef)
  *(required)*
- `HyperParameters`: `Mapping`\[`str`, `str`\]
- `InputDataConfig`:
  `Sequence`\[[ChannelTypeDef](./type_defs.md#channeltypedef)\]
- `VpcConfig`: [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `EnableNetworkIsolation`: `bool`
- `EnableInterContainerTrafficEncryption`: `bool`
- `EnableManagedSpotTraining`: `bool`
- `CheckpointConfig`:
  [CheckpointConfigTypeDef](./type_defs.md#checkpointconfigtypedef)
- `DebugHookConfig`:
  [DebugHookConfigTypeDef](./type_defs.md#debughookconfigtypedef)
- `DebugRuleConfigurations`:
  `Sequence`\[[DebugRuleConfigurationTypeDef](./type_defs.md#debugruleconfigurationtypedef)\]
- `TensorBoardOutputConfig`:
  [TensorBoardOutputConfigTypeDef](./type_defs.md#tensorboardoutputconfigtypedef)
- `ExperimentConfig`:
  [ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef)
- `ProfilerConfig`:
  [ProfilerConfigTypeDef](./type_defs.md#profilerconfigtypedef)
- `ProfilerRuleConfigurations`:
  `Sequence`\[[ProfilerRuleConfigurationTypeDef](./type_defs.md#profilerruleconfigurationtypedef)\]
- `Environment`: `Mapping`\[`str`, `str`\]
- `RetryStrategy`: [RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef)

Returns a `Coroutine` for
[CreateTrainingJobResponseTypeDef](./type_defs.md#createtrainingjobresponsetypedef).

<a id="create_transform_job"></a>

### create_transform_job

Starts a transform job.

Type annotations for
`aiobotocore.create_client("sagemaker").create_transform_job` method.

Boto3 documentation:
[SageMaker.Client.create_transform_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_transform_job)

Asynchronous method. Use `await create_transform_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateTransformJobRequestRequestTypeDef](./type_defs.md#createtransformjobrequestrequesttypedef).

Keyword-only arguments:

- `TransformJobName`: `str` *(required)*
- `ModelName`: `str` *(required)*
- `TransformInput`:
  [TransformInputTypeDef](./type_defs.md#transforminputtypedef) *(required)*
- `TransformOutput`:
  [TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) *(required)*
- `TransformResources`:
  [TransformResourcesTypeDef](./type_defs.md#transformresourcestypedef)
  *(required)*
- `MaxConcurrentTransforms`: `int`
- `ModelClientConfig`:
  [ModelClientConfigTypeDef](./type_defs.md#modelclientconfigtypedef)
- `MaxPayloadInMB`: `int`
- `BatchStrategy`: [BatchStrategyType](./literals.md#batchstrategytype)
- `Environment`: `Mapping`\[`str`, `str`\]
- `DataProcessing`:
  [DataProcessingTypeDef](./type_defs.md#dataprocessingtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ExperimentConfig`:
  [ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef)

Returns a `Coroutine` for
[CreateTransformJobResponseTypeDef](./type_defs.md#createtransformjobresponsetypedef).

<a id="create_trial"></a>

### create_trial

Creates an SageMaker *trial*.

Type annotations for `aiobotocore.create_client("sagemaker").create_trial`
method.

Boto3 documentation:
[SageMaker.Client.create_trial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial)

Asynchronous method. Use `await create_trial(...)` for a synchronous call.

Arguments mapping described in
[CreateTrialRequestRequestTypeDef](./type_defs.md#createtrialrequestrequesttypedef).

Keyword-only arguments:

- `TrialName`: `str` *(required)*
- `ExperimentName`: `str` *(required)*
- `DisplayName`: `str`
- `MetadataProperties`:
  [MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateTrialResponseTypeDef](./type_defs.md#createtrialresponsetypedef).

<a id="create_trial_component"></a>

### create_trial_component

Creates a *trial component* , which is a stage of a machine learning *trial*.

Type annotations for
`aiobotocore.create_client("sagemaker").create_trial_component` method.

Boto3 documentation:
[SageMaker.Client.create_trial_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial_component)

Asynchronous method. Use `await create_trial_component(...)` for a synchronous
call.

Arguments mapping described in
[CreateTrialComponentRequestRequestTypeDef](./type_defs.md#createtrialcomponentrequestrequesttypedef).

Keyword-only arguments:

- `TrialComponentName`: `str` *(required)*
- `DisplayName`: `str`
- `Status`:
  [TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef)
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `Parameters`: `Mapping`\[`str`,
  [TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef)\]
- `InputArtifacts`: `Mapping`\[`str`,
  [TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef)\]
- `OutputArtifacts`: `Mapping`\[`str`,
  [TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef)\]
- `MetadataProperties`:
  [MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateTrialComponentResponseTypeDef](./type_defs.md#createtrialcomponentresponsetypedef).

<a id="create_user_profile"></a>

### create_user_profile

Creates a user profile.

Type annotations for
`aiobotocore.create_client("sagemaker").create_user_profile` method.

Boto3 documentation:
[SageMaker.Client.create_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_user_profile)

Asynchronous method. Use `await create_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[CreateUserProfileRequestRequestTypeDef](./type_defs.md#createuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*
- `SingleSignOnUserIdentifier`: `str`
- `SingleSignOnUserValue`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `UserSettings`: [UserSettingsTypeDef](./type_defs.md#usersettingstypedef)

Returns a `Coroutine` for
[CreateUserProfileResponseTypeDef](./type_defs.md#createuserprofileresponsetypedef).

<a id="create_workforce"></a>

### create_workforce

Use this operation to create a workforce.

Type annotations for `aiobotocore.create_client("sagemaker").create_workforce`
method.

Boto3 documentation:
[SageMaker.Client.create_workforce](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workforce)

Asynchronous method. Use `await create_workforce(...)` for a synchronous call.

Arguments mapping described in
[CreateWorkforceRequestRequestTypeDef](./type_defs.md#createworkforcerequestrequesttypedef).

Keyword-only arguments:

- `WorkforceName`: `str` *(required)*
- `CognitoConfig`: [CognitoConfigTypeDef](./type_defs.md#cognitoconfigtypedef)
- `OidcConfig`: [OidcConfigTypeDef](./type_defs.md#oidcconfigtypedef)
- `SourceIpConfig`:
  [SourceIpConfigTypeDef](./type_defs.md#sourceipconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateWorkforceResponseTypeDef](./type_defs.md#createworkforceresponsetypedef).

<a id="create_workteam"></a>

### create_workteam

Creates a new work team for labeling your data.

Type annotations for `aiobotocore.create_client("sagemaker").create_workteam`
method.

Boto3 documentation:
[SageMaker.Client.create_workteam](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workteam)

Asynchronous method. Use `await create_workteam(...)` for a synchronous call.

Arguments mapping described in
[CreateWorkteamRequestRequestTypeDef](./type_defs.md#createworkteamrequestrequesttypedef).

Keyword-only arguments:

- `WorkteamName`: `str` *(required)*
- `MemberDefinitions`:
  `Sequence`\[[MemberDefinitionTypeDef](./type_defs.md#memberdefinitiontypedef)\]
  *(required)*
- `Description`: `str` *(required)*
- `WorkforceName`: `str`
- `NotificationConfiguration`:
  [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateWorkteamResponseTypeDef](./type_defs.md#createworkteamresponsetypedef).

<a id="delete_action"></a>

### delete_action

Deletes an action.

Type annotations for `aiobotocore.create_client("sagemaker").delete_action`
method.

Boto3 documentation:
[SageMaker.Client.delete_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_action)

Asynchronous method. Use `await delete_action(...)` for a synchronous call.

Arguments mapping described in
[DeleteActionRequestRequestTypeDef](./type_defs.md#deleteactionrequestrequesttypedef).

Keyword-only arguments:

- `ActionName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteActionResponseTypeDef](./type_defs.md#deleteactionresponsetypedef).

<a id="delete_algorithm"></a>

### delete_algorithm

Removes the specified algorithm from your account.

Type annotations for `aiobotocore.create_client("sagemaker").delete_algorithm`
method.

Boto3 documentation:
[SageMaker.Client.delete_algorithm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_algorithm)

Asynchronous method. Use `await delete_algorithm(...)` for a synchronous call.

Arguments mapping described in
[DeleteAlgorithmInputRequestTypeDef](./type_defs.md#deletealgorithminputrequesttypedef).

Keyword-only arguments:

- `AlgorithmName`: `str` *(required)*

<a id="delete_app"></a>

### delete_app

Used to stop and delete an app.

Type annotations for `aiobotocore.create_client("sagemaker").delete_app`
method.

Boto3 documentation:
[SageMaker.Client.delete_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app)

Asynchronous method. Use `await delete_app(...)` for a synchronous call.

Arguments mapping described in
[DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*
- `AppType`: [AppTypeType](./literals.md#apptypetype) *(required)*
- `AppName`: `str` *(required)*

<a id="delete_app_image_config"></a>

### delete_app_image_config

Deletes an AppImageConfig.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_app_image_config` method.

Boto3 documentation:
[SageMaker.Client.delete_app_image_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app_image_config)

Asynchronous method. Use `await delete_app_image_config(...)` for a synchronous
call.

Arguments mapping described in
[DeleteAppImageConfigRequestRequestTypeDef](./type_defs.md#deleteappimageconfigrequestrequesttypedef).

Keyword-only arguments:

- `AppImageConfigName`: `str` *(required)*

<a id="delete_artifact"></a>

### delete_artifact

Deletes an artifact.

Type annotations for `aiobotocore.create_client("sagemaker").delete_artifact`
method.

Boto3 documentation:
[SageMaker.Client.delete_artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_artifact)

Asynchronous method. Use `await delete_artifact(...)` for a synchronous call.

Arguments mapping described in
[DeleteArtifactRequestRequestTypeDef](./type_defs.md#deleteartifactrequestrequesttypedef).

Keyword-only arguments:

- `ArtifactArn`: `str`
- `Source`: [ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef)

Returns a `Coroutine` for
[DeleteArtifactResponseTypeDef](./type_defs.md#deleteartifactresponsetypedef).

<a id="delete_association"></a>

### delete_association

Deletes an association.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_association` method.

Boto3 documentation:
[SageMaker.Client.delete_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_association)

Asynchronous method. Use `await delete_association(...)` for a synchronous
call.

Arguments mapping described in
[DeleteAssociationRequestRequestTypeDef](./type_defs.md#deleteassociationrequestrequesttypedef).

Keyword-only arguments:

- `SourceArn`: `str` *(required)*
- `DestinationArn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteAssociationResponseTypeDef](./type_defs.md#deleteassociationresponsetypedef).

<a id="delete_code_repository"></a>

### delete_code_repository

Deletes the specified Git repository from your account.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_code_repository` method.

Boto3 documentation:
[SageMaker.Client.delete_code_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_code_repository)

Asynchronous method. Use `await delete_code_repository(...)` for a synchronous
call.

Arguments mapping described in
[DeleteCodeRepositoryInputRequestTypeDef](./type_defs.md#deletecoderepositoryinputrequesttypedef).

Keyword-only arguments:

- `CodeRepositoryName`: `str` *(required)*

<a id="delete_context"></a>

### delete_context

Deletes an context.

Type annotations for `aiobotocore.create_client("sagemaker").delete_context`
method.

Boto3 documentation:
[SageMaker.Client.delete_context](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_context)

Asynchronous method. Use `await delete_context(...)` for a synchronous call.

Arguments mapping described in
[DeleteContextRequestRequestTypeDef](./type_defs.md#deletecontextrequestrequesttypedef).

Keyword-only arguments:

- `ContextName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteContextResponseTypeDef](./type_defs.md#deletecontextresponsetypedef).

<a id="delete_data_quality_job_definition"></a>

### delete_data_quality_job_definition

Deletes a data quality monitoring job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_data_quality_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.delete_data_quality_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_data_quality_job_definition)

Asynchronous method. Use `await delete_data_quality_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDataQualityJobDefinitionRequestRequestTypeDef](./type_defs.md#deletedataqualityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

<a id="delete_device_fleet"></a>

### delete_device_fleet

Deletes a fleet.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_device_fleet` method.

Boto3 documentation:
[SageMaker.Client.delete_device_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_device_fleet)

Asynchronous method. Use `await delete_device_fleet(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDeviceFleetRequestRequestTypeDef](./type_defs.md#deletedevicefleetrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*

<a id="delete_domain"></a>

### delete_domain

Used to delete a domain.

Type annotations for `aiobotocore.create_client("sagemaker").delete_domain`
method.

Boto3 documentation:
[SageMaker.Client.delete_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_domain)

Asynchronous method. Use `await delete_domain(...)` for a synchronous call.

Arguments mapping described in
[DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `RetentionPolicy`:
  [RetentionPolicyTypeDef](./type_defs.md#retentionpolicytypedef)

<a id="delete_endpoint"></a>

### delete_endpoint

Deletes an endpoint.

Type annotations for `aiobotocore.create_client("sagemaker").delete_endpoint`
method.

Boto3 documentation:
[SageMaker.Client.delete_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_endpoint)

Asynchronous method. Use `await delete_endpoint(...)` for a synchronous call.

Arguments mapping described in
[DeleteEndpointInputRequestTypeDef](./type_defs.md#deleteendpointinputrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str` *(required)*

<a id="delete_endpoint_config"></a>

### delete_endpoint_config

Deletes an endpoint configuration.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_endpoint_config` method.

Boto3 documentation:
[SageMaker.Client.delete_endpoint_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_endpoint_config)

Asynchronous method. Use `await delete_endpoint_config(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEndpointConfigInputRequestTypeDef](./type_defs.md#deleteendpointconfiginputrequesttypedef).

Keyword-only arguments:

- `EndpointConfigName`: `str` *(required)*

<a id="delete_experiment"></a>

### delete_experiment

Deletes an SageMaker experiment.

Type annotations for `aiobotocore.create_client("sagemaker").delete_experiment`
method.

Boto3 documentation:
[SageMaker.Client.delete_experiment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_experiment)

Asynchronous method. Use `await delete_experiment(...)` for a synchronous call.

Arguments mapping described in
[DeleteExperimentRequestRequestTypeDef](./type_defs.md#deleteexperimentrequestrequesttypedef).

Keyword-only arguments:

- `ExperimentName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteExperimentResponseTypeDef](./type_defs.md#deleteexperimentresponsetypedef).

<a id="delete_feature_group"></a>

### delete_feature_group

Delete the `FeatureGroup` and any data that was written to the `OnlineStore` of
the `FeatureGroup`.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_feature_group` method.

Boto3 documentation:
[SageMaker.Client.delete_feature_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_feature_group)

Asynchronous method. Use `await delete_feature_group(...)` for a synchronous
call.

Arguments mapping described in
[DeleteFeatureGroupRequestRequestTypeDef](./type_defs.md#deletefeaturegrouprequestrequesttypedef).

Keyword-only arguments:

- `FeatureGroupName`: `str` *(required)*

<a id="delete_flow_definition"></a>

### delete_flow_definition

Deletes the specified flow definition.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_flow_definition` method.

Boto3 documentation:
[SageMaker.Client.delete_flow_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_flow_definition)

Asynchronous method. Use `await delete_flow_definition(...)` for a synchronous
call.

Arguments mapping described in
[DeleteFlowDefinitionRequestRequestTypeDef](./type_defs.md#deleteflowdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `FlowDefinitionName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_human_task_ui"></a>

### delete_human_task_ui

Use this operation to delete a human task user interface (worker task
template).

Type annotations for
`aiobotocore.create_client("sagemaker").delete_human_task_ui` method.

Boto3 documentation:
[SageMaker.Client.delete_human_task_ui](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_human_task_ui)

Asynchronous method. Use `await delete_human_task_ui(...)` for a synchronous
call.

Arguments mapping described in
[DeleteHumanTaskUiRequestRequestTypeDef](./type_defs.md#deletehumantaskuirequestrequesttypedef).

Keyword-only arguments:

- `HumanTaskUiName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_image"></a>

### delete_image

Deletes a SageMaker image and all versions of the image.

Type annotations for `aiobotocore.create_client("sagemaker").delete_image`
method.

Boto3 documentation:
[SageMaker.Client.delete_image](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_image)

Asynchronous method. Use `await delete_image(...)` for a synchronous call.

Arguments mapping described in
[DeleteImageRequestRequestTypeDef](./type_defs.md#deleteimagerequestrequesttypedef).

Keyword-only arguments:

- `ImageName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_image_version"></a>

### delete_image_version

Deletes a version of a SageMaker image.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_image_version` method.

Boto3 documentation:
[SageMaker.Client.delete_image_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_image_version)

Asynchronous method. Use `await delete_image_version(...)` for a synchronous
call.

Arguments mapping described in
[DeleteImageVersionRequestRequestTypeDef](./type_defs.md#deleteimageversionrequestrequesttypedef).

Keyword-only arguments:

- `ImageName`: `str` *(required)*
- `Version`: `int` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_model"></a>

### delete_model

Deletes a model.

Type annotations for `aiobotocore.create_client("sagemaker").delete_model`
method.

Boto3 documentation:
[SageMaker.Client.delete_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_model)

Asynchronous method. Use `await delete_model(...)` for a synchronous call.

Arguments mapping described in
[DeleteModelInputRequestTypeDef](./type_defs.md#deletemodelinputrequesttypedef).

Keyword-only arguments:

- `ModelName`: `str` *(required)*

<a id="delete_model_bias_job_definition"></a>

### delete_model_bias_job_definition

Deletes an Amazon SageMaker model bias job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_model_bias_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.delete_model_bias_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_model_bias_job_definition)

Asynchronous method. Use `await delete_model_bias_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[DeleteModelBiasJobDefinitionRequestRequestTypeDef](./type_defs.md#deletemodelbiasjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

<a id="delete_model_explainability_job_definition"></a>

### delete_model_explainability_job_definition

Deletes an Amazon SageMaker model explainability job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_model_explainability_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.delete_model_explainability_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_model_explainability_job_definition)

Asynchronous method. Use
`await delete_model_explainability_job_definition(...)` for a synchronous call.

Arguments mapping described in
[DeleteModelExplainabilityJobDefinitionRequestRequestTypeDef](./type_defs.md#deletemodelexplainabilityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

<a id="delete_model_package"></a>

### delete_model_package

Deletes a model package.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_model_package` method.

Boto3 documentation:
[SageMaker.Client.delete_model_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_model_package)

Asynchronous method. Use `await delete_model_package(...)` for a synchronous
call.

Arguments mapping described in
[DeleteModelPackageInputRequestTypeDef](./type_defs.md#deletemodelpackageinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageName`: `str` *(required)*

<a id="delete_model_package_group"></a>

### delete_model_package_group

Deletes the specified model group.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_model_package_group` method.

Boto3 documentation:
[SageMaker.Client.delete_model_package_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_model_package_group)

Asynchronous method. Use `await delete_model_package_group(...)` for a
synchronous call.

Arguments mapping described in
[DeleteModelPackageGroupInputRequestTypeDef](./type_defs.md#deletemodelpackagegroupinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageGroupName`: `str` *(required)*

<a id="delete_model_package_group_policy"></a>

### delete_model_package_group_policy

Deletes a model group resource policy.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_model_package_group_policy`
method.

Boto3 documentation:
[SageMaker.Client.delete_model_package_group_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_model_package_group_policy)

Asynchronous method. Use `await delete_model_package_group_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteModelPackageGroupPolicyInputRequestTypeDef](./type_defs.md#deletemodelpackagegrouppolicyinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageGroupName`: `str` *(required)*

<a id="delete_model_quality_job_definition"></a>

### delete_model_quality_job_definition

Deletes the secified model quality monitoring job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_model_quality_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.delete_model_quality_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_model_quality_job_definition)

Asynchronous method. Use `await delete_model_quality_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[DeleteModelQualityJobDefinitionRequestRequestTypeDef](./type_defs.md#deletemodelqualityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

<a id="delete_monitoring_schedule"></a>

### delete_monitoring_schedule

Deletes a monitoring schedule.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_monitoring_schedule` method.

Boto3 documentation:
[SageMaker.Client.delete_monitoring_schedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_monitoring_schedule)

Asynchronous method. Use `await delete_monitoring_schedule(...)` for a
synchronous call.

Arguments mapping described in
[DeleteMonitoringScheduleRequestRequestTypeDef](./type_defs.md#deletemonitoringschedulerequestrequesttypedef).

Keyword-only arguments:

- `MonitoringScheduleName`: `str` *(required)*

<a id="delete_notebook_instance"></a>

### delete_notebook_instance

Deletes an Amazon SageMaker notebook instance.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_notebook_instance` method.

Boto3 documentation:
[SageMaker.Client.delete_notebook_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_notebook_instance)

Asynchronous method. Use `await delete_notebook_instance(...)` for a
synchronous call.

Arguments mapping described in
[DeleteNotebookInstanceInputRequestTypeDef](./type_defs.md#deletenotebookinstanceinputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceName`: `str` *(required)*

<a id="delete_notebook_instance_lifecycle_config"></a>

### delete_notebook_instance_lifecycle_config

Deletes a notebook instance lifecycle configuration.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_notebook_instance_lifecycle_config`
method.

Boto3 documentation:
[SageMaker.Client.delete_notebook_instance_lifecycle_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_notebook_instance_lifecycle_config)

Asynchronous method. Use `await delete_notebook_instance_lifecycle_config(...)`
for a synchronous call.

Arguments mapping described in
[DeleteNotebookInstanceLifecycleConfigInputRequestTypeDef](./type_defs.md#deletenotebookinstancelifecycleconfiginputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceLifecycleConfigName`: `str` *(required)*

<a id="delete_pipeline"></a>

### delete_pipeline

Deletes a pipeline if there are no running instances of the pipeline.

Type annotations for `aiobotocore.create_client("sagemaker").delete_pipeline`
method.

Boto3 documentation:
[SageMaker.Client.delete_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_pipeline)

Asynchronous method. Use `await delete_pipeline(...)` for a synchronous call.

Arguments mapping described in
[DeletePipelineRequestRequestTypeDef](./type_defs.md#deletepipelinerequestrequesttypedef).

Keyword-only arguments:

- `PipelineName`: `str` *(required)*
- `ClientRequestToken`: `str` *(required)*

Returns a `Coroutine` for
[DeletePipelineResponseTypeDef](./type_defs.md#deletepipelineresponsetypedef).

<a id="delete_project"></a>

### delete_project

Delete the specified project.

Type annotations for `aiobotocore.create_client("sagemaker").delete_project`
method.

Boto3 documentation:
[SageMaker.Client.delete_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_project)

Asynchronous method. Use `await delete_project(...)` for a synchronous call.

Arguments mapping described in
[DeleteProjectInputRequestTypeDef](./type_defs.md#deleteprojectinputrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*

<a id="delete_studio_lifecycle_config"></a>

### delete_studio_lifecycle_config

Deletes the Studio Lifecycle Configuration.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_studio_lifecycle_config` method.

Boto3 documentation:
[SageMaker.Client.delete_studio_lifecycle_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_studio_lifecycle_config)

Asynchronous method. Use `await delete_studio_lifecycle_config(...)` for a
synchronous call.

Arguments mapping described in
[DeleteStudioLifecycleConfigRequestRequestTypeDef](./type_defs.md#deletestudiolifecycleconfigrequestrequesttypedef).

Keyword-only arguments:

- `StudioLifecycleConfigName`: `str` *(required)*

<a id="delete_tags"></a>

### delete_tags

Deletes the specified tags from an Amazon SageMaker resource.

Type annotations for `aiobotocore.create_client("sagemaker").delete_tags`
method.

Boto3 documentation:
[SageMaker.Client.delete_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_tags)

Asynchronous method. Use `await delete_tags(...)` for a synchronous call.

Arguments mapping described in
[DeleteTagsInputRequestTypeDef](./type_defs.md#deletetagsinputrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_trial"></a>

### delete_trial

Deletes the specified trial.

Type annotations for `aiobotocore.create_client("sagemaker").delete_trial`
method.

Boto3 documentation:
[SageMaker.Client.delete_trial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_trial)

Asynchronous method. Use `await delete_trial(...)` for a synchronous call.

Arguments mapping described in
[DeleteTrialRequestRequestTypeDef](./type_defs.md#deletetrialrequestrequesttypedef).

Keyword-only arguments:

- `TrialName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteTrialResponseTypeDef](./type_defs.md#deletetrialresponsetypedef).

<a id="delete_trial_component"></a>

### delete_trial_component

Deletes the specified trial component.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_trial_component` method.

Boto3 documentation:
[SageMaker.Client.delete_trial_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_trial_component)

Asynchronous method. Use `await delete_trial_component(...)` for a synchronous
call.

Arguments mapping described in
[DeleteTrialComponentRequestRequestTypeDef](./type_defs.md#deletetrialcomponentrequestrequesttypedef).

Keyword-only arguments:

- `TrialComponentName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteTrialComponentResponseTypeDef](./type_defs.md#deletetrialcomponentresponsetypedef).

<a id="delete_user_profile"></a>

### delete_user_profile

Deletes a user profile.

Type annotations for
`aiobotocore.create_client("sagemaker").delete_user_profile` method.

Boto3 documentation:
[SageMaker.Client.delete_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_user_profile)

Asynchronous method. Use `await delete_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[DeleteUserProfileRequestRequestTypeDef](./type_defs.md#deleteuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*

<a id="delete_workforce"></a>

### delete_workforce

Use this operation to delete a workforce.

Type annotations for `aiobotocore.create_client("sagemaker").delete_workforce`
method.

Boto3 documentation:
[SageMaker.Client.delete_workforce](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_workforce)

Asynchronous method. Use `await delete_workforce(...)` for a synchronous call.

Arguments mapping described in
[DeleteWorkforceRequestRequestTypeDef](./type_defs.md#deleteworkforcerequestrequesttypedef).

Keyword-only arguments:

- `WorkforceName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_workteam"></a>

### delete_workteam

Deletes an existing work team.

Type annotations for `aiobotocore.create_client("sagemaker").delete_workteam`
method.

Boto3 documentation:
[SageMaker.Client.delete_workteam](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_workteam)

Asynchronous method. Use `await delete_workteam(...)` for a synchronous call.

Arguments mapping described in
[DeleteWorkteamRequestRequestTypeDef](./type_defs.md#deleteworkteamrequestrequesttypedef).

Keyword-only arguments:

- `WorkteamName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteWorkteamResponseTypeDef](./type_defs.md#deleteworkteamresponsetypedef).

<a id="deregister_devices"></a>

### deregister_devices

Deregisters the specified devices.

Type annotations for
`aiobotocore.create_client("sagemaker").deregister_devices` method.

Boto3 documentation:
[SageMaker.Client.deregister_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.deregister_devices)

Asynchronous method. Use `await deregister_devices(...)` for a synchronous
call.

Arguments mapping described in
[DeregisterDevicesRequestRequestTypeDef](./type_defs.md#deregisterdevicesrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*
- `DeviceNames`: `Sequence`\[`str`\] *(required)*

<a id="describe_action"></a>

### describe_action

Describes an action.

Type annotations for `aiobotocore.create_client("sagemaker").describe_action`
method.

Boto3 documentation:
[SageMaker.Client.describe_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_action)

Asynchronous method. Use `await describe_action(...)` for a synchronous call.

Arguments mapping described in
[DescribeActionRequestRequestTypeDef](./type_defs.md#describeactionrequestrequesttypedef).

Keyword-only arguments:

- `ActionName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeActionResponseTypeDef](./type_defs.md#describeactionresponsetypedef).

<a id="describe_algorithm"></a>

### describe_algorithm

Returns a description of the specified algorithm that is in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_algorithm` method.

Boto3 documentation:
[SageMaker.Client.describe_algorithm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_algorithm)

Asynchronous method. Use `await describe_algorithm(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAlgorithmInputRequestTypeDef](./type_defs.md#describealgorithminputrequesttypedef).

Keyword-only arguments:

- `AlgorithmName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAlgorithmOutputTypeDef](./type_defs.md#describealgorithmoutputtypedef).

<a id="describe_app"></a>

### describe_app

Describes the app.

Type annotations for `aiobotocore.create_client("sagemaker").describe_app`
method.

Boto3 documentation:
[SageMaker.Client.describe_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_app)

Asynchronous method. Use `await describe_app(...)` for a synchronous call.

Arguments mapping described in
[DescribeAppRequestRequestTypeDef](./type_defs.md#describeapprequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*
- `AppType`: [AppTypeType](./literals.md#apptypetype) *(required)*
- `AppName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAppResponseTypeDef](./type_defs.md#describeappresponsetypedef).

<a id="describe_app_image_config"></a>

### describe_app_image_config

Describes an AppImageConfig.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_app_image_config` method.

Boto3 documentation:
[SageMaker.Client.describe_app_image_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_app_image_config)

Asynchronous method. Use `await describe_app_image_config(...)` for a
synchronous call.

Arguments mapping described in
[DescribeAppImageConfigRequestRequestTypeDef](./type_defs.md#describeappimageconfigrequestrequesttypedef).

Keyword-only arguments:

- `AppImageConfigName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAppImageConfigResponseTypeDef](./type_defs.md#describeappimageconfigresponsetypedef).

<a id="describe_artifact"></a>

### describe_artifact

Describes an artifact.

Type annotations for `aiobotocore.create_client("sagemaker").describe_artifact`
method.

Boto3 documentation:
[SageMaker.Client.describe_artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_artifact)

Asynchronous method. Use `await describe_artifact(...)` for a synchronous call.

Arguments mapping described in
[DescribeArtifactRequestRequestTypeDef](./type_defs.md#describeartifactrequestrequesttypedef).

Keyword-only arguments:

- `ArtifactArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeArtifactResponseTypeDef](./type_defs.md#describeartifactresponsetypedef).

<a id="describe_auto_ml_job"></a>

### describe_auto_ml_job

Returns information about an Amazon SageMaker AutoML job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_auto_ml_job` method.

Boto3 documentation:
[SageMaker.Client.describe_auto_ml_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_auto_ml_job)

Asynchronous method. Use `await describe_auto_ml_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAutoMLJobRequestRequestTypeDef](./type_defs.md#describeautomljobrequestrequesttypedef).

Keyword-only arguments:

- `AutoMLJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAutoMLJobResponseTypeDef](./type_defs.md#describeautomljobresponsetypedef).

<a id="describe_code_repository"></a>

### describe_code_repository

Gets details about the specified Git repository.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_code_repository` method.

Boto3 documentation:
[SageMaker.Client.describe_code_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_code_repository)

Asynchronous method. Use `await describe_code_repository(...)` for a
synchronous call.

Arguments mapping described in
[DescribeCodeRepositoryInputRequestTypeDef](./type_defs.md#describecoderepositoryinputrequesttypedef).

Keyword-only arguments:

- `CodeRepositoryName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeCodeRepositoryOutputTypeDef](./type_defs.md#describecoderepositoryoutputtypedef).

<a id="describe_compilation_job"></a>

### describe_compilation_job

.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_compilation_job` method.

Boto3 documentation:
[SageMaker.Client.describe_compilation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_compilation_job)

Asynchronous method. Use `await describe_compilation_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeCompilationJobRequestRequestTypeDef](./type_defs.md#describecompilationjobrequestrequesttypedef).

Keyword-only arguments:

- `CompilationJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeCompilationJobResponseTypeDef](./type_defs.md#describecompilationjobresponsetypedef).

<a id="describe_context"></a>

### describe_context

Describes a context.

Type annotations for `aiobotocore.create_client("sagemaker").describe_context`
method.

Boto3 documentation:
[SageMaker.Client.describe_context](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_context)

Asynchronous method. Use `await describe_context(...)` for a synchronous call.

Arguments mapping described in
[DescribeContextRequestRequestTypeDef](./type_defs.md#describecontextrequestrequesttypedef).

Keyword-only arguments:

- `ContextName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeContextResponseTypeDef](./type_defs.md#describecontextresponsetypedef).

<a id="describe_data_quality_job_definition"></a>

### describe_data_quality_job_definition

Gets the details of a data quality monitoring job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_data_quality_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.describe_data_quality_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_data_quality_job_definition)

Asynchronous method. Use `await describe_data_quality_job_definition(...)` for
a synchronous call.

Arguments mapping described in
[DescribeDataQualityJobDefinitionRequestRequestTypeDef](./type_defs.md#describedataqualityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDataQualityJobDefinitionResponseTypeDef](./type_defs.md#describedataqualityjobdefinitionresponsetypedef).

<a id="describe_device"></a>

### describe_device

Describes the device.

Type annotations for `aiobotocore.create_client("sagemaker").describe_device`
method.

Boto3 documentation:
[SageMaker.Client.describe_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_device)

Asynchronous method. Use `await describe_device(...)` for a synchronous call.

Arguments mapping described in
[DescribeDeviceRequestRequestTypeDef](./type_defs.md#describedevicerequestrequesttypedef).

Keyword-only arguments:

- `DeviceName`: `str` *(required)*
- `DeviceFleetName`: `str` *(required)*
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeDeviceResponseTypeDef](./type_defs.md#describedeviceresponsetypedef).

<a id="describe_device_fleet"></a>

### describe_device_fleet

A description of the fleet the device belongs to.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_device_fleet` method.

Boto3 documentation:
[SageMaker.Client.describe_device_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_device_fleet)

Asynchronous method. Use `await describe_device_fleet(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDeviceFleetRequestRequestTypeDef](./type_defs.md#describedevicefleetrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDeviceFleetResponseTypeDef](./type_defs.md#describedevicefleetresponsetypedef).

<a id="describe_domain"></a>

### describe_domain

The description of the domain.

Type annotations for `aiobotocore.create_client("sagemaker").describe_domain`
method.

Boto3 documentation:
[SageMaker.Client.describe_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_domain)

Asynchronous method. Use `await describe_domain(...)` for a synchronous call.

Arguments mapping described in
[DescribeDomainRequestRequestTypeDef](./type_defs.md#describedomainrequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDomainResponseTypeDef](./type_defs.md#describedomainresponsetypedef).

<a id="describe_edge_packaging_job"></a>

### describe_edge_packaging_job

A description of edge packaging jobs.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_edge_packaging_job` method.

Boto3 documentation:
[SageMaker.Client.describe_edge_packaging_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_edge_packaging_job)

Asynchronous method. Use `await describe_edge_packaging_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEdgePackagingJobRequestRequestTypeDef](./type_defs.md#describeedgepackagingjobrequestrequesttypedef).

Keyword-only arguments:

- `EdgePackagingJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeEdgePackagingJobResponseTypeDef](./type_defs.md#describeedgepackagingjobresponsetypedef).

<a id="describe_endpoint"></a>

### describe_endpoint

.

Type annotations for `aiobotocore.create_client("sagemaker").describe_endpoint`
method.

Boto3 documentation:
[SageMaker.Client.describe_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_endpoint)

Asynchronous method. Use `await describe_endpoint(...)` for a synchronous call.

Arguments mapping described in
[DescribeEndpointInputRequestTypeDef](./type_defs.md#describeendpointinputrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeEndpointOutputTypeDef](./type_defs.md#describeendpointoutputtypedef).

<a id="describe_endpoint_config"></a>

### describe_endpoint_config

.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_endpoint_config` method.

Boto3 documentation:
[SageMaker.Client.describe_endpoint_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_endpoint_config)

Asynchronous method. Use `await describe_endpoint_config(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEndpointConfigInputRequestTypeDef](./type_defs.md#describeendpointconfiginputrequesttypedef).

Keyword-only arguments:

- `EndpointConfigName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeEndpointConfigOutputTypeDef](./type_defs.md#describeendpointconfigoutputtypedef).

<a id="describe_experiment"></a>

### describe_experiment

Provides a list of an experiment's properties.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_experiment` method.

Boto3 documentation:
[SageMaker.Client.describe_experiment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_experiment)

Asynchronous method. Use `await describe_experiment(...)` for a synchronous
call.

Arguments mapping described in
[DescribeExperimentRequestRequestTypeDef](./type_defs.md#describeexperimentrequestrequesttypedef).

Keyword-only arguments:

- `ExperimentName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeExperimentResponseTypeDef](./type_defs.md#describeexperimentresponsetypedef).

<a id="describe_feature_group"></a>

### describe_feature_group

Use this operation to describe a `FeatureGroup`.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_feature_group` method.

Boto3 documentation:
[SageMaker.Client.describe_feature_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_feature_group)

Asynchronous method. Use `await describe_feature_group(...)` for a synchronous
call.

Arguments mapping described in
[DescribeFeatureGroupRequestRequestTypeDef](./type_defs.md#describefeaturegrouprequestrequesttypedef).

Keyword-only arguments:

- `FeatureGroupName`: `str` *(required)*
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeFeatureGroupResponseTypeDef](./type_defs.md#describefeaturegroupresponsetypedef).

<a id="describe_flow_definition"></a>

### describe_flow_definition

Returns information about the specified flow definition.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_flow_definition` method.

Boto3 documentation:
[SageMaker.Client.describe_flow_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_flow_definition)

Asynchronous method. Use `await describe_flow_definition(...)` for a
synchronous call.

Arguments mapping described in
[DescribeFlowDefinitionRequestRequestTypeDef](./type_defs.md#describeflowdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `FlowDefinitionName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeFlowDefinitionResponseTypeDef](./type_defs.md#describeflowdefinitionresponsetypedef).

<a id="describe_human_task_ui"></a>

### describe_human_task_ui

Returns information about the requested human task user interface (worker task
template).

Type annotations for
`aiobotocore.create_client("sagemaker").describe_human_task_ui` method.

Boto3 documentation:
[SageMaker.Client.describe_human_task_ui](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_human_task_ui)

Asynchronous method. Use `await describe_human_task_ui(...)` for a synchronous
call.

Arguments mapping described in
[DescribeHumanTaskUiRequestRequestTypeDef](./type_defs.md#describehumantaskuirequestrequesttypedef).

Keyword-only arguments:

- `HumanTaskUiName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeHumanTaskUiResponseTypeDef](./type_defs.md#describehumantaskuiresponsetypedef).

<a id="describe_hyper_parameter_tuning_job"></a>

### describe_hyper_parameter_tuning_job

Gets a description of a hyperparameter tuning job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_hyper_parameter_tuning_job`
method.

Boto3 documentation:
[SageMaker.Client.describe_hyper_parameter_tuning_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_hyper_parameter_tuning_job)

Asynchronous method. Use `await describe_hyper_parameter_tuning_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeHyperParameterTuningJobRequestRequestTypeDef](./type_defs.md#describehyperparametertuningjobrequestrequesttypedef).

Keyword-only arguments:

- `HyperParameterTuningJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeHyperParameterTuningJobResponseTypeDef](./type_defs.md#describehyperparametertuningjobresponsetypedef).

<a id="describe_image"></a>

### describe_image

Describes a SageMaker image.

Type annotations for `aiobotocore.create_client("sagemaker").describe_image`
method.

Boto3 documentation:
[SageMaker.Client.describe_image](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_image)

Asynchronous method. Use `await describe_image(...)` for a synchronous call.

Arguments mapping described in
[DescribeImageRequestRequestTypeDef](./type_defs.md#describeimagerequestrequesttypedef).

Keyword-only arguments:

- `ImageName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeImageResponseTypeDef](./type_defs.md#describeimageresponsetypedef).

<a id="describe_image_version"></a>

### describe_image_version

Describes a version of a SageMaker image.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_image_version` method.

Boto3 documentation:
[SageMaker.Client.describe_image_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_image_version)

Asynchronous method. Use `await describe_image_version(...)` for a synchronous
call.

Arguments mapping described in
[DescribeImageVersionRequestRequestTypeDef](./type_defs.md#describeimageversionrequestrequesttypedef).

Keyword-only arguments:

- `ImageName`: `str` *(required)*
- `Version`: `int`

Returns a `Coroutine` for
[DescribeImageVersionResponseTypeDef](./type_defs.md#describeimageversionresponsetypedef).

<a id="describe_inference_recommendations_job"></a>

### describe_inference_recommendations_job

Provides the results of the Inference Recommender job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_inference_recommendations_job`
method.

Boto3 documentation:
[SageMaker.Client.describe_inference_recommendations_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_inference_recommendations_job)

Asynchronous method. Use `await describe_inference_recommendations_job(...)`
for a synchronous call.

Arguments mapping described in
[DescribeInferenceRecommendationsJobRequestRequestTypeDef](./type_defs.md#describeinferencerecommendationsjobrequestrequesttypedef).

Keyword-only arguments:

- `JobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeInferenceRecommendationsJobResponseTypeDef](./type_defs.md#describeinferencerecommendationsjobresponsetypedef).

<a id="describe_labeling_job"></a>

### describe_labeling_job

Gets information about a labeling job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_labeling_job` method.

Boto3 documentation:
[SageMaker.Client.describe_labeling_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_labeling_job)

Asynchronous method. Use `await describe_labeling_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeLabelingJobRequestRequestTypeDef](./type_defs.md#describelabelingjobrequestrequesttypedef).

Keyword-only arguments:

- `LabelingJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeLabelingJobResponseTypeDef](./type_defs.md#describelabelingjobresponsetypedef).

<a id="describe_lineage_group"></a>

### describe_lineage_group

Provides a list of properties for the requested lineage group.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_lineage_group` method.

Boto3 documentation:
[SageMaker.Client.describe_lineage_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_lineage_group)

Asynchronous method. Use `await describe_lineage_group(...)` for a synchronous
call.

Arguments mapping described in
[DescribeLineageGroupRequestRequestTypeDef](./type_defs.md#describelineagegrouprequestrequesttypedef).

Keyword-only arguments:

- `LineageGroupName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeLineageGroupResponseTypeDef](./type_defs.md#describelineagegroupresponsetypedef).

<a id="describe_model"></a>

### describe_model

Describes a model that you created using the `CreateModel` API.

Type annotations for `aiobotocore.create_client("sagemaker").describe_model`
method.

Boto3 documentation:
[SageMaker.Client.describe_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_model)

Asynchronous method. Use `await describe_model(...)` for a synchronous call.

Arguments mapping described in
[DescribeModelInputRequestTypeDef](./type_defs.md#describemodelinputrequesttypedef).

Keyword-only arguments:

- `ModelName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelOutputTypeDef](./type_defs.md#describemodeloutputtypedef).

<a id="describe_model_bias_job_definition"></a>

### describe_model_bias_job_definition

Returns a description of a model bias job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_model_bias_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.describe_model_bias_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_model_bias_job_definition)

Asynchronous method. Use `await describe_model_bias_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[DescribeModelBiasJobDefinitionRequestRequestTypeDef](./type_defs.md#describemodelbiasjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelBiasJobDefinitionResponseTypeDef](./type_defs.md#describemodelbiasjobdefinitionresponsetypedef).

<a id="describe_model_explainability_job_definition"></a>

### describe_model_explainability_job_definition

Returns a description of a model explainability job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_model_explainability_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.describe_model_explainability_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_model_explainability_job_definition)

Asynchronous method. Use
`await describe_model_explainability_job_definition(...)` for a synchronous
call.

Arguments mapping described in
[DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef](./type_defs.md#describemodelexplainabilityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelExplainabilityJobDefinitionResponseTypeDef](./type_defs.md#describemodelexplainabilityjobdefinitionresponsetypedef).

<a id="describe_model_package"></a>

### describe_model_package

Returns a description of the specified model package, which is used to create
SageMaker models or list them on Amazon Web Services Marketplace.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_model_package` method.

Boto3 documentation:
[SageMaker.Client.describe_model_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_model_package)

Asynchronous method. Use `await describe_model_package(...)` for a synchronous
call.

Arguments mapping described in
[DescribeModelPackageInputRequestTypeDef](./type_defs.md#describemodelpackageinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelPackageOutputTypeDef](./type_defs.md#describemodelpackageoutputtypedef).

<a id="describe_model_package_group"></a>

### describe_model_package_group

Gets a description for the specified model group.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_model_package_group` method.

Boto3 documentation:
[SageMaker.Client.describe_model_package_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_model_package_group)

Asynchronous method. Use `await describe_model_package_group(...)` for a
synchronous call.

Arguments mapping described in
[DescribeModelPackageGroupInputRequestTypeDef](./type_defs.md#describemodelpackagegroupinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageGroupName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelPackageGroupOutputTypeDef](./type_defs.md#describemodelpackagegroupoutputtypedef).

<a id="describe_model_quality_job_definition"></a>

### describe_model_quality_job_definition

Returns a description of a model quality job definition.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_model_quality_job_definition`
method.

Boto3 documentation:
[SageMaker.Client.describe_model_quality_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_model_quality_job_definition)

Asynchronous method. Use `await describe_model_quality_job_definition(...)` for
a synchronous call.

Arguments mapping described in
[DescribeModelQualityJobDefinitionRequestRequestTypeDef](./type_defs.md#describemodelqualityjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `JobDefinitionName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelQualityJobDefinitionResponseTypeDef](./type_defs.md#describemodelqualityjobdefinitionresponsetypedef).

<a id="describe_monitoring_schedule"></a>

### describe_monitoring_schedule

Describes the schedule for a monitoring job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_monitoring_schedule` method.

Boto3 documentation:
[SageMaker.Client.describe_monitoring_schedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_monitoring_schedule)

Asynchronous method. Use `await describe_monitoring_schedule(...)` for a
synchronous call.

Arguments mapping described in
[DescribeMonitoringScheduleRequestRequestTypeDef](./type_defs.md#describemonitoringschedulerequestrequesttypedef).

Keyword-only arguments:

- `MonitoringScheduleName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeMonitoringScheduleResponseTypeDef](./type_defs.md#describemonitoringscheduleresponsetypedef).

<a id="describe_notebook_instance"></a>

### describe_notebook_instance

Returns information about a notebook instance.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_notebook_instance` method.

Boto3 documentation:
[SageMaker.Client.describe_notebook_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_notebook_instance)

Asynchronous method. Use `await describe_notebook_instance(...)` for a
synchronous call.

Arguments mapping described in
[DescribeNotebookInstanceInputRequestTypeDef](./type_defs.md#describenotebookinstanceinputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeNotebookInstanceOutputTypeDef](./type_defs.md#describenotebookinstanceoutputtypedef).

<a id="describe_notebook_instance_lifecycle_config"></a>

### describe_notebook_instance_lifecycle_config

Returns a description of a notebook instance lifecycle configuration.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_notebook_instance_lifecycle_config`
method.

Boto3 documentation:
[SageMaker.Client.describe_notebook_instance_lifecycle_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_notebook_instance_lifecycle_config)

Asynchronous method. Use
`await describe_notebook_instance_lifecycle_config(...)` for a synchronous
call.

Arguments mapping described in
[DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef](./type_defs.md#describenotebookinstancelifecycleconfiginputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceLifecycleConfigName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeNotebookInstanceLifecycleConfigOutputTypeDef](./type_defs.md#describenotebookinstancelifecycleconfigoutputtypedef).

<a id="describe_pipeline"></a>

### describe_pipeline

Describes the details of a pipeline.

Type annotations for `aiobotocore.create_client("sagemaker").describe_pipeline`
method.

Boto3 documentation:
[SageMaker.Client.describe_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_pipeline)

Asynchronous method. Use `await describe_pipeline(...)` for a synchronous call.

Arguments mapping described in
[DescribePipelineRequestRequestTypeDef](./type_defs.md#describepipelinerequestrequesttypedef).

Keyword-only arguments:

- `PipelineName`: `str` *(required)*

Returns a `Coroutine` for
[DescribePipelineResponseTypeDef](./type_defs.md#describepipelineresponsetypedef).

<a id="describe_pipeline_definition_for_execution"></a>

### describe_pipeline_definition_for_execution

Describes the details of an execution's pipeline definition.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_pipeline_definition_for_execution`
method.

Boto3 documentation:
[SageMaker.Client.describe_pipeline_definition_for_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_pipeline_definition_for_execution)

Asynchronous method. Use
`await describe_pipeline_definition_for_execution(...)` for a synchronous call.

Arguments mapping described in
[DescribePipelineDefinitionForExecutionRequestRequestTypeDef](./type_defs.md#describepipelinedefinitionforexecutionrequestrequesttypedef).

Keyword-only arguments:

- `PipelineExecutionArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribePipelineDefinitionForExecutionResponseTypeDef](./type_defs.md#describepipelinedefinitionforexecutionresponsetypedef).

<a id="describe_pipeline_execution"></a>

### describe_pipeline_execution

Describes the details of a pipeline execution.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_pipeline_execution` method.

Boto3 documentation:
[SageMaker.Client.describe_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_pipeline_execution)

Asynchronous method. Use `await describe_pipeline_execution(...)` for a
synchronous call.

Arguments mapping described in
[DescribePipelineExecutionRequestRequestTypeDef](./type_defs.md#describepipelineexecutionrequestrequesttypedef).

Keyword-only arguments:

- `PipelineExecutionArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribePipelineExecutionResponseTypeDef](./type_defs.md#describepipelineexecutionresponsetypedef).

<a id="describe_processing_job"></a>

### describe_processing_job

Returns a description of a processing job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_processing_job` method.

Boto3 documentation:
[SageMaker.Client.describe_processing_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_processing_job)

Asynchronous method. Use `await describe_processing_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeProcessingJobRequestRequestTypeDef](./type_defs.md#describeprocessingjobrequestrequesttypedef).

Keyword-only arguments:

- `ProcessingJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeProcessingJobResponseTypeDef](./type_defs.md#describeprocessingjobresponsetypedef).

<a id="describe_project"></a>

### describe_project

Describes the details of a project.

Type annotations for `aiobotocore.create_client("sagemaker").describe_project`
method.

Boto3 documentation:
[SageMaker.Client.describe_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_project)

Asynchronous method. Use `await describe_project(...)` for a synchronous call.

Arguments mapping described in
[DescribeProjectInputRequestTypeDef](./type_defs.md#describeprojectinputrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeProjectOutputTypeDef](./type_defs.md#describeprojectoutputtypedef).

<a id="describe_studio_lifecycle_config"></a>

### describe_studio_lifecycle_config

Describes the Studio Lifecycle Configuration.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_studio_lifecycle_config`
method.

Boto3 documentation:
[SageMaker.Client.describe_studio_lifecycle_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_studio_lifecycle_config)

Asynchronous method. Use `await describe_studio_lifecycle_config(...)` for a
synchronous call.

Arguments mapping described in
[DescribeStudioLifecycleConfigRequestRequestTypeDef](./type_defs.md#describestudiolifecycleconfigrequestrequesttypedef).

Keyword-only arguments:

- `StudioLifecycleConfigName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeStudioLifecycleConfigResponseTypeDef](./type_defs.md#describestudiolifecycleconfigresponsetypedef).

<a id="describe_subscribed_workteam"></a>

### describe_subscribed_workteam

Gets information about a work team provided by a vendor.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_subscribed_workteam` method.

Boto3 documentation:
[SageMaker.Client.describe_subscribed_workteam](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_subscribed_workteam)

Asynchronous method. Use `await describe_subscribed_workteam(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSubscribedWorkteamRequestRequestTypeDef](./type_defs.md#describesubscribedworkteamrequestrequesttypedef).

Keyword-only arguments:

- `WorkteamArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSubscribedWorkteamResponseTypeDef](./type_defs.md#describesubscribedworkteamresponsetypedef).

<a id="describe_training_job"></a>

### describe_training_job

Returns information about a training job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_training_job` method.

Boto3 documentation:
[SageMaker.Client.describe_training_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_training_job)

Asynchronous method. Use `await describe_training_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeTrainingJobRequestRequestTypeDef](./type_defs.md#describetrainingjobrequestrequesttypedef).

Keyword-only arguments:

- `TrainingJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTrainingJobResponseTypeDef](./type_defs.md#describetrainingjobresponsetypedef).

<a id="describe_transform_job"></a>

### describe_transform_job

Returns information about a transform job.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_transform_job` method.

Boto3 documentation:
[SageMaker.Client.describe_transform_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_transform_job)

Asynchronous method. Use `await describe_transform_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeTransformJobRequestRequestTypeDef](./type_defs.md#describetransformjobrequestrequesttypedef).

Keyword-only arguments:

- `TransformJobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTransformJobResponseTypeDef](./type_defs.md#describetransformjobresponsetypedef).

<a id="describe_trial"></a>

### describe_trial

Provides a list of a trial's properties.

Type annotations for `aiobotocore.create_client("sagemaker").describe_trial`
method.

Boto3 documentation:
[SageMaker.Client.describe_trial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_trial)

Asynchronous method. Use `await describe_trial(...)` for a synchronous call.

Arguments mapping described in
[DescribeTrialRequestRequestTypeDef](./type_defs.md#describetrialrequestrequesttypedef).

Keyword-only arguments:

- `TrialName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTrialResponseTypeDef](./type_defs.md#describetrialresponsetypedef).

<a id="describe_trial_component"></a>

### describe_trial_component

Provides a list of a trials component's properties.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_trial_component` method.

Boto3 documentation:
[SageMaker.Client.describe_trial_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_trial_component)

Asynchronous method. Use `await describe_trial_component(...)` for a
synchronous call.

Arguments mapping described in
[DescribeTrialComponentRequestRequestTypeDef](./type_defs.md#describetrialcomponentrequestrequesttypedef).

Keyword-only arguments:

- `TrialComponentName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTrialComponentResponseTypeDef](./type_defs.md#describetrialcomponentresponsetypedef).

<a id="describe_user_profile"></a>

### describe_user_profile

Describes a user profile.

Type annotations for
`aiobotocore.create_client("sagemaker").describe_user_profile` method.

Boto3 documentation:
[SageMaker.Client.describe_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_user_profile)

Asynchronous method. Use `await describe_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[DescribeUserProfileRequestRequestTypeDef](./type_defs.md#describeuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeUserProfileResponseTypeDef](./type_defs.md#describeuserprofileresponsetypedef).

<a id="describe_workforce"></a>

### describe_workforce

Lists private workforce information, including workforce name, Amazon Resource
Name (ARN), and, if applicable, allowed IP address ranges
([CIDRs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)\_
).

Type annotations for
`aiobotocore.create_client("sagemaker").describe_workforce` method.

Boto3 documentation:
[SageMaker.Client.describe_workforce](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_workforce)

Asynchronous method. Use `await describe_workforce(...)` for a synchronous
call.

Arguments mapping described in
[DescribeWorkforceRequestRequestTypeDef](./type_defs.md#describeworkforcerequestrequesttypedef).

Keyword-only arguments:

- `WorkforceName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeWorkforceResponseTypeDef](./type_defs.md#describeworkforceresponsetypedef).

<a id="describe_workteam"></a>

### describe_workteam

Gets information about a specific work team.

Type annotations for `aiobotocore.create_client("sagemaker").describe_workteam`
method.

Boto3 documentation:
[SageMaker.Client.describe_workteam](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_workteam)

Asynchronous method. Use `await describe_workteam(...)` for a synchronous call.

Arguments mapping described in
[DescribeWorkteamRequestRequestTypeDef](./type_defs.md#describeworkteamrequestrequesttypedef).

Keyword-only arguments:

- `WorkteamName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeWorkteamResponseTypeDef](./type_defs.md#describeworkteamresponsetypedef).

<a id="disable_sagemaker_servicecatalog_portfolio"></a>

### disable_sagemaker_servicecatalog_portfolio

Disables using Service Catalog in SageMaker.

Type annotations for
`aiobotocore.create_client("sagemaker").disable_sagemaker_servicecatalog_portfolio`
method.

Boto3 documentation:
[SageMaker.Client.disable_sagemaker_servicecatalog_portfolio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.disable_sagemaker_servicecatalog_portfolio)

Asynchronous method. Use
`await disable_sagemaker_servicecatalog_portfolio(...)` for a synchronous call.

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate_trial_component"></a>

### disassociate_trial_component

Disassociates a trial component from a trial.

Type annotations for
`aiobotocore.create_client("sagemaker").disassociate_trial_component` method.

Boto3 documentation:
[SageMaker.Client.disassociate_trial_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.disassociate_trial_component)

Asynchronous method. Use `await disassociate_trial_component(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateTrialComponentRequestRequestTypeDef](./type_defs.md#disassociatetrialcomponentrequestrequesttypedef).

Keyword-only arguments:

- `TrialComponentName`: `str` *(required)*
- `TrialName`: `str` *(required)*

Returns a `Coroutine` for
[DisassociateTrialComponentResponseTypeDef](./type_defs.md#disassociatetrialcomponentresponsetypedef).

<a id="enable_sagemaker_servicecatalog_portfolio"></a>

### enable_sagemaker_servicecatalog_portfolio

Enables using Service Catalog in SageMaker.

Type annotations for
`aiobotocore.create_client("sagemaker").enable_sagemaker_servicecatalog_portfolio`
method.

Boto3 documentation:
[SageMaker.Client.enable_sagemaker_servicecatalog_portfolio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.enable_sagemaker_servicecatalog_portfolio)

Asynchronous method. Use `await enable_sagemaker_servicecatalog_portfolio(...)`
for a synchronous call.

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("sagemaker").generate_presigned_url` method.

Boto3 documentation:
[SageMaker.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_device_fleet_report"></a>

### get_device_fleet_report

Describes a fleet.

Type annotations for
`aiobotocore.create_client("sagemaker").get_device_fleet_report` method.

Boto3 documentation:
[SageMaker.Client.get_device_fleet_report](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_device_fleet_report)

Asynchronous method. Use `await get_device_fleet_report(...)` for a synchronous
call.

Arguments mapping described in
[GetDeviceFleetReportRequestRequestTypeDef](./type_defs.md#getdevicefleetreportrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*

Returns a `Coroutine` for
[GetDeviceFleetReportResponseTypeDef](./type_defs.md#getdevicefleetreportresponsetypedef).

<a id="get_lineage_group_policy"></a>

### get_lineage_group_policy

The resource policy for the lineage group.

Type annotations for
`aiobotocore.create_client("sagemaker").get_lineage_group_policy` method.

Boto3 documentation:
[SageMaker.Client.get_lineage_group_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_lineage_group_policy)

Asynchronous method. Use `await get_lineage_group_policy(...)` for a
synchronous call.

Arguments mapping described in
[GetLineageGroupPolicyRequestRequestTypeDef](./type_defs.md#getlineagegrouppolicyrequestrequesttypedef).

Keyword-only arguments:

- `LineageGroupName`: `str` *(required)*

Returns a `Coroutine` for
[GetLineageGroupPolicyResponseTypeDef](./type_defs.md#getlineagegrouppolicyresponsetypedef).

<a id="get_model_package_group_policy"></a>

### get_model_package_group_policy

Gets a resource policy that manages access for a model group.

Type annotations for
`aiobotocore.create_client("sagemaker").get_model_package_group_policy` method.

Boto3 documentation:
[SageMaker.Client.get_model_package_group_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_model_package_group_policy)

Asynchronous method. Use `await get_model_package_group_policy(...)` for a
synchronous call.

Arguments mapping described in
[GetModelPackageGroupPolicyInputRequestTypeDef](./type_defs.md#getmodelpackagegrouppolicyinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageGroupName`: `str` *(required)*

Returns a `Coroutine` for
[GetModelPackageGroupPolicyOutputTypeDef](./type_defs.md#getmodelpackagegrouppolicyoutputtypedef).

<a id="get_sagemaker_servicecatalog_portfolio_status"></a>

### get_sagemaker_servicecatalog_portfolio_status

Gets the status of Service Catalog in SageMaker.

Type annotations for
`aiobotocore.create_client("sagemaker").get_sagemaker_servicecatalog_portfolio_status`
method.

Boto3 documentation:
[SageMaker.Client.get_sagemaker_servicecatalog_portfolio_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_sagemaker_servicecatalog_portfolio_status)

Asynchronous method. Use
`await get_sagemaker_servicecatalog_portfolio_status(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetSagemakerServicecatalogPortfolioStatusOutputTypeDef](./type_defs.md#getsagemakerservicecatalogportfoliostatusoutputtypedef).

<a id="get_search_suggestions"></a>

### get_search_suggestions

An auto-complete API for the search functionality in the Amazon SageMaker
console.

Type annotations for
`aiobotocore.create_client("sagemaker").get_search_suggestions` method.

Boto3 documentation:
[SageMaker.Client.get_search_suggestions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_search_suggestions)

Asynchronous method. Use `await get_search_suggestions(...)` for a synchronous
call.

Arguments mapping described in
[GetSearchSuggestionsRequestRequestTypeDef](./type_defs.md#getsearchsuggestionsrequestrequesttypedef).

Keyword-only arguments:

- `Resource`: [ResourceTypeType](./literals.md#resourcetypetype) *(required)*
- `SuggestionQuery`:
  [SuggestionQueryTypeDef](./type_defs.md#suggestionquerytypedef)

Returns a `Coroutine` for
[GetSearchSuggestionsResponseTypeDef](./type_defs.md#getsearchsuggestionsresponsetypedef).

<a id="list_actions"></a>

### list_actions

Lists the actions in your account and their properties.

Type annotations for `aiobotocore.create_client("sagemaker").list_actions`
method.

Boto3 documentation:
[SageMaker.Client.list_actions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_actions)

Asynchronous method. Use `await list_actions(...)` for a synchronous call.

Arguments mapping described in
[ListActionsRequestRequestTypeDef](./type_defs.md#listactionsrequestrequesttypedef).

Keyword-only arguments:

- `SourceUri`: `str`
- `ActionType`: `str`
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: [SortActionsByType](./literals.md#sortactionsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef).

<a id="list_algorithms"></a>

### list_algorithms

Lists the machine learning algorithms that have been created.

Type annotations for `aiobotocore.create_client("sagemaker").list_algorithms`
method.

Boto3 documentation:
[SageMaker.Client.list_algorithms](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_algorithms)

Asynchronous method. Use `await list_algorithms(...)` for a synchronous call.

Arguments mapping described in
[ListAlgorithmsInputRequestTypeDef](./type_defs.md#listalgorithmsinputrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NameContains`: `str`
- `NextToken`: `str`
- `SortBy`: [AlgorithmSortByType](./literals.md#algorithmsortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListAlgorithmsOutputTypeDef](./type_defs.md#listalgorithmsoutputtypedef).

<a id="list_app_image_configs"></a>

### list_app_image_configs

Lists the AppImageConfigs in your account and their properties.

Type annotations for
`aiobotocore.create_client("sagemaker").list_app_image_configs` method.

Boto3 documentation:
[SageMaker.Client.list_app_image_configs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_app_image_configs)

Asynchronous method. Use `await list_app_image_configs(...)` for a synchronous
call.

Arguments mapping described in
[ListAppImageConfigsRequestRequestTypeDef](./type_defs.md#listappimageconfigsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `ModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `ModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `SortBy`:
  [AppImageConfigSortKeyType](./literals.md#appimageconfigsortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListAppImageConfigsResponseTypeDef](./type_defs.md#listappimageconfigsresponsetypedef).

<a id="list_apps"></a>

### list_apps

Lists apps.

Type annotations for `aiobotocore.create_client("sagemaker").list_apps` method.

Boto3 documentation:
[SageMaker.Client.list_apps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_apps)

Asynchronous method. Use `await list_apps(...)` for a synchronous call.

Arguments mapping described in
[ListAppsRequestRequestTypeDef](./type_defs.md#listappsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `SortBy`: `Literal['CreationTime']` (see
  [AppSortKeyType](./literals.md#appsortkeytype))
- `DomainIdEquals`: `str`
- `UserProfileNameEquals`: `str`

Returns a `Coroutine` for
[ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef).

<a id="list_artifacts"></a>

### list_artifacts

Lists the artifacts in your account and their properties.

Type annotations for `aiobotocore.create_client("sagemaker").list_artifacts`
method.

Boto3 documentation:
[SageMaker.Client.list_artifacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_artifacts)

Asynchronous method. Use `await list_artifacts(...)` for a synchronous call.

Arguments mapping described in
[ListArtifactsRequestRequestTypeDef](./type_defs.md#listartifactsrequestrequesttypedef).

Keyword-only arguments:

- `SourceUri`: `str`
- `ArtifactType`: `str`
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: `Literal['CreationTime']` (see
  [SortArtifactsByType](./literals.md#sortartifactsbytype))
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListArtifactsResponseTypeDef](./type_defs.md#listartifactsresponsetypedef).

<a id="list_associations"></a>

### list_associations

Lists the associations in your account and their properties.

Type annotations for `aiobotocore.create_client("sagemaker").list_associations`
method.

Boto3 documentation:
[SageMaker.Client.list_associations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_associations)

Asynchronous method. Use `await list_associations(...)` for a synchronous call.

Arguments mapping described in
[ListAssociationsRequestRequestTypeDef](./type_defs.md#listassociationsrequestrequesttypedef).

Keyword-only arguments:

- `SourceArn`: `str`
- `DestinationArn`: `str`
- `SourceType`: `str`
- `DestinationType`: `str`
- `AssociationType`:
  [AssociationEdgeTypeType](./literals.md#associationedgetypetype)
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: [SortAssociationsByType](./literals.md#sortassociationsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListAssociationsResponseTypeDef](./type_defs.md#listassociationsresponsetypedef).

<a id="list_auto_ml_jobs"></a>

### list_auto_ml_jobs

Request a list of jobs.

Type annotations for `aiobotocore.create_client("sagemaker").list_auto_ml_jobs`
method.

Boto3 documentation:
[SageMaker.Client.list_auto_ml_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_auto_ml_jobs)

Asynchronous method. Use `await list_auto_ml_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListAutoMLJobsRequestRequestTypeDef](./type_defs.md#listautomljobsrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `StatusEquals`: [AutoMLJobStatusType](./literals.md#automljobstatustype)
- `SortOrder`: [AutoMLSortOrderType](./literals.md#automlsortordertype)
- `SortBy`: [AutoMLSortByType](./literals.md#automlsortbytype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListAutoMLJobsResponseTypeDef](./type_defs.md#listautomljobsresponsetypedef).

<a id="list_candidates_for_auto_ml_job"></a>

### list_candidates_for_auto_ml_job

List the candidates created for the job.

Type annotations for
`aiobotocore.create_client("sagemaker").list_candidates_for_auto_ml_job`
method.

Boto3 documentation:
[SageMaker.Client.list_candidates_for_auto_ml_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_candidates_for_auto_ml_job)

Asynchronous method. Use `await list_candidates_for_auto_ml_job(...)` for a
synchronous call.

Arguments mapping described in
[ListCandidatesForAutoMLJobRequestRequestTypeDef](./type_defs.md#listcandidatesforautomljobrequestrequesttypedef).

Keyword-only arguments:

- `AutoMLJobName`: `str` *(required)*
- `StatusEquals`: [CandidateStatusType](./literals.md#candidatestatustype)
- `CandidateNameEquals`: `str`
- `SortOrder`: [AutoMLSortOrderType](./literals.md#automlsortordertype)
- `SortBy`: [CandidateSortByType](./literals.md#candidatesortbytype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListCandidatesForAutoMLJobResponseTypeDef](./type_defs.md#listcandidatesforautomljobresponsetypedef).

<a id="list_code_repositories"></a>

### list_code_repositories

Gets a list of the Git repositories in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_code_repositories` method.

Boto3 documentation:
[SageMaker.Client.list_code_repositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_code_repositories)

Asynchronous method. Use `await list_code_repositories(...)` for a synchronous
call.

Arguments mapping described in
[ListCodeRepositoriesInputRequestTypeDef](./type_defs.md#listcoderepositoriesinputrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NameContains`: `str`
- `NextToken`: `str`
- `SortBy`: [CodeRepositorySortByType](./literals.md#coderepositorysortbytype)
- `SortOrder`:
  [CodeRepositorySortOrderType](./literals.md#coderepositorysortordertype)

Returns a `Coroutine` for
[ListCodeRepositoriesOutputTypeDef](./type_defs.md#listcoderepositoriesoutputtypedef).

<a id="list_compilation_jobs"></a>

### list_compilation_jobs

Lists model compilation jobs that satisfy various filters.

Type annotations for
`aiobotocore.create_client("sagemaker").list_compilation_jobs` method.

Boto3 documentation:
[SageMaker.Client.list_compilation_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_compilation_jobs)

Asynchronous method. Use `await list_compilation_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListCompilationJobsRequestRequestTypeDef](./type_defs.md#listcompilationjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `StatusEquals`:
  [CompilationJobStatusType](./literals.md#compilationjobstatustype)
- `SortBy`:
  [ListCompilationJobsSortByType](./literals.md#listcompilationjobssortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListCompilationJobsResponseTypeDef](./type_defs.md#listcompilationjobsresponsetypedef).

<a id="list_contexts"></a>

### list_contexts

Lists the contexts in your account and their properties.

Type annotations for `aiobotocore.create_client("sagemaker").list_contexts`
method.

Boto3 documentation:
[SageMaker.Client.list_contexts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_contexts)

Asynchronous method. Use `await list_contexts(...)` for a synchronous call.

Arguments mapping described in
[ListContextsRequestRequestTypeDef](./type_defs.md#listcontextsrequestrequesttypedef).

Keyword-only arguments:

- `SourceUri`: `str`
- `ContextType`: `str`
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: [SortContextsByType](./literals.md#sortcontextsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListContextsResponseTypeDef](./type_defs.md#listcontextsresponsetypedef).

<a id="list_data_quality_job_definitions"></a>

### list_data_quality_job_definitions

Lists the data quality job definitions in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_data_quality_job_definitions`
method.

Boto3 documentation:
[SageMaker.Client.list_data_quality_job_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_data_quality_job_definitions)

Asynchronous method. Use `await list_data_quality_job_definitions(...)` for a
synchronous call.

Arguments mapping described in
[ListDataQualityJobDefinitionsRequestRequestTypeDef](./type_defs.md#listdataqualityjobdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str`
- `SortBy`:
  [MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[ListDataQualityJobDefinitionsResponseTypeDef](./type_defs.md#listdataqualityjobdefinitionsresponsetypedef).

<a id="list_device_fleets"></a>

### list_device_fleets

Returns a list of devices in the fleet.

Type annotations for
`aiobotocore.create_client("sagemaker").list_device_fleets` method.

Boto3 documentation:
[SageMaker.Client.list_device_fleets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_device_fleets)

Asynchronous method. Use `await list_device_fleets(...)` for a synchronous
call.

Arguments mapping described in
[ListDeviceFleetsRequestRequestTypeDef](./type_defs.md#listdevicefleetsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `SortBy`:
  [ListDeviceFleetsSortByType](./literals.md#listdevicefleetssortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListDeviceFleetsResponseTypeDef](./type_defs.md#listdevicefleetsresponsetypedef).

<a id="list_devices"></a>

### list_devices

A list of devices.

Type annotations for `aiobotocore.create_client("sagemaker").list_devices`
method.

Boto3 documentation:
[SageMaker.Client.list_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_devices)

Asynchronous method. Use `await list_devices(...)` for a synchronous call.

Arguments mapping described in
[ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `LatestHeartbeatAfter`: `Union`\[`datetime`, `str`\]
- `ModelName`: `str`
- `DeviceFleetName`: `str`

Returns a `Coroutine` for
[ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef).

<a id="list_domains"></a>

### list_domains

Lists the domains.

Type annotations for `aiobotocore.create_client("sagemaker").list_domains`
method.

Boto3 documentation:
[SageMaker.Client.list_domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_domains)

Asynchronous method. Use `await list_domains(...)` for a synchronous call.

Arguments mapping described in
[ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef).

<a id="list_edge_packaging_jobs"></a>

### list_edge_packaging_jobs

Returns a list of edge packaging jobs.

Type annotations for
`aiobotocore.create_client("sagemaker").list_edge_packaging_jobs` method.

Boto3 documentation:
[SageMaker.Client.list_edge_packaging_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_edge_packaging_jobs)

Asynchronous method. Use `await list_edge_packaging_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListEdgePackagingJobsRequestRequestTypeDef](./type_defs.md#listedgepackagingjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `ModelNameContains`: `str`
- `StatusEquals`:
  [EdgePackagingJobStatusType](./literals.md#edgepackagingjobstatustype)
- `SortBy`:
  [ListEdgePackagingJobsSortByType](./literals.md#listedgepackagingjobssortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListEdgePackagingJobsResponseTypeDef](./type_defs.md#listedgepackagingjobsresponsetypedef).

<a id="list_endpoint_configs"></a>

### list_endpoint_configs

Lists endpoint configurations.

Type annotations for
`aiobotocore.create_client("sagemaker").list_endpoint_configs` method.

Boto3 documentation:
[SageMaker.Client.list_endpoint_configs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_endpoint_configs)

Asynchronous method. Use `await list_endpoint_configs(...)` for a synchronous
call.

Arguments mapping described in
[ListEndpointConfigsInputRequestTypeDef](./type_defs.md#listendpointconfigsinputrequesttypedef).

Keyword-only arguments:

- `SortBy`:
  [EndpointConfigSortKeyType](./literals.md#endpointconfigsortkeytype)
- `SortOrder`: [OrderKeyType](./literals.md#orderkeytype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[ListEndpointConfigsOutputTypeDef](./type_defs.md#listendpointconfigsoutputtypedef).

<a id="list_endpoints"></a>

### list_endpoints

Lists endpoints.

Type annotations for `aiobotocore.create_client("sagemaker").list_endpoints`
method.

Boto3 documentation:
[SageMaker.Client.list_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_endpoints)

Asynchronous method. Use `await list_endpoints(...)` for a synchronous call.

Arguments mapping described in
[ListEndpointsInputRequestTypeDef](./type_defs.md#listendpointsinputrequesttypedef).

Keyword-only arguments:

- `SortBy`: [EndpointSortKeyType](./literals.md#endpointsortkeytype)
- `SortOrder`: [OrderKeyType](./literals.md#orderkeytype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `StatusEquals`: [EndpointStatusType](./literals.md#endpointstatustype)

Returns a `Coroutine` for
[ListEndpointsOutputTypeDef](./type_defs.md#listendpointsoutputtypedef).

<a id="list_experiments"></a>

### list_experiments

Lists all the experiments in your account.

Type annotations for `aiobotocore.create_client("sagemaker").list_experiments`
method.

Boto3 documentation:
[SageMaker.Client.list_experiments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_experiments)

Asynchronous method. Use `await list_experiments(...)` for a synchronous call.

Arguments mapping described in
[ListExperimentsRequestRequestTypeDef](./type_defs.md#listexperimentsrequestrequesttypedef).

Keyword-only arguments:

- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: [SortExperimentsByType](./literals.md#sortexperimentsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef).

<a id="list_feature_groups"></a>

### list_feature_groups

List `FeatureGroup` s based on given filter and order.

Type annotations for
`aiobotocore.create_client("sagemaker").list_feature_groups` method.

Boto3 documentation:
[SageMaker.Client.list_feature_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_feature_groups)

Asynchronous method. Use `await list_feature_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListFeatureGroupsRequestRequestTypeDef](./type_defs.md#listfeaturegroupsrequestrequesttypedef).

Keyword-only arguments:

- `NameContains`: `str`
- `FeatureGroupStatusEquals`:
  [FeatureGroupStatusType](./literals.md#featuregroupstatustype)
- `OfflineStoreStatusEquals`:
  [OfflineStoreStatusValueType](./literals.md#offlinestorestatusvaluetype)
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `SortOrder`:
  [FeatureGroupSortOrderType](./literals.md#featuregroupsortordertype)
- `SortBy`: [FeatureGroupSortByType](./literals.md#featuregroupsortbytype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListFeatureGroupsResponseTypeDef](./type_defs.md#listfeaturegroupsresponsetypedef).

<a id="list_flow_definitions"></a>

### list_flow_definitions

Returns information about the flow definitions in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_flow_definitions` method.

Boto3 documentation:
[SageMaker.Client.list_flow_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_flow_definitions)

Asynchronous method. Use `await list_flow_definitions(...)` for a synchronous
call.

Arguments mapping described in
[ListFlowDefinitionsRequestRequestTypeDef](./type_defs.md#listflowdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListFlowDefinitionsResponseTypeDef](./type_defs.md#listflowdefinitionsresponsetypedef).

<a id="list_human_task_uis"></a>

### list_human_task_uis

Returns information about the human task user interfaces in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_human_task_uis` method.

Boto3 documentation:
[SageMaker.Client.list_human_task_uis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_human_task_uis)

Asynchronous method. Use `await list_human_task_uis(...)` for a synchronous
call.

Arguments mapping described in
[ListHumanTaskUisRequestRequestTypeDef](./type_defs.md#listhumantaskuisrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListHumanTaskUisResponseTypeDef](./type_defs.md#listhumantaskuisresponsetypedef).

<a id="list_hyper_parameter_tuning_jobs"></a>

### list_hyper_parameter_tuning_jobs

Gets a list of HyperParameterTuningJobSummary objects that describe the
hyperparameter tuning jobs launched in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_hyper_parameter_tuning_jobs`
method.

Boto3 documentation:
[SageMaker.Client.list_hyper_parameter_tuning_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_hyper_parameter_tuning_jobs)

Asynchronous method. Use `await list_hyper_parameter_tuning_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListHyperParameterTuningJobsRequestRequestTypeDef](./type_defs.md#listhyperparametertuningjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `SortBy`:
  [HyperParameterTuningJobSortByOptionsType](./literals.md#hyperparametertuningjobsortbyoptionstype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NameContains`: `str`
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `StatusEquals`:
  [HyperParameterTuningJobStatusType](./literals.md#hyperparametertuningjobstatustype)

Returns a `Coroutine` for
[ListHyperParameterTuningJobsResponseTypeDef](./type_defs.md#listhyperparametertuningjobsresponsetypedef).

<a id="list_image_versions"></a>

### list_image_versions

Lists the versions of a specified image and their properties.

Type annotations for
`aiobotocore.create_client("sagemaker").list_image_versions` method.

Boto3 documentation:
[SageMaker.Client.list_image_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_image_versions)

Asynchronous method. Use `await list_image_versions(...)` for a synchronous
call.

Arguments mapping described in
[ListImageVersionsRequestRequestTypeDef](./type_defs.md#listimageversionsrequestrequesttypedef).

Keyword-only arguments:

- `ImageName`: `str` *(required)*
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NextToken`: `str`
- `SortBy`: [ImageVersionSortByType](./literals.md#imageversionsortbytype)
- `SortOrder`:
  [ImageVersionSortOrderType](./literals.md#imageversionsortordertype)

Returns a `Coroutine` for
[ListImageVersionsResponseTypeDef](./type_defs.md#listimageversionsresponsetypedef).

<a id="list_images"></a>

### list_images

Lists the images in your account and their properties.

Type annotations for `aiobotocore.create_client("sagemaker").list_images`
method.

Boto3 documentation:
[SageMaker.Client.list_images](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_images)

Asynchronous method. Use `await list_images(...)` for a synchronous call.

Arguments mapping described in
[ListImagesRequestRequestTypeDef](./type_defs.md#listimagesrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NameContains`: `str`
- `NextToken`: `str`
- `SortBy`: [ImageSortByType](./literals.md#imagesortbytype)
- `SortOrder`: [ImageSortOrderType](./literals.md#imagesortordertype)

Returns a `Coroutine` for
[ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef).

<a id="list_inference_recommendations_jobs"></a>

### list_inference_recommendations_jobs

Lists recommendation jobs that satisfy various filters.

Type annotations for
`aiobotocore.create_client("sagemaker").list_inference_recommendations_jobs`
method.

Boto3 documentation:
[SageMaker.Client.list_inference_recommendations_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_recommendations_jobs)

Asynchronous method. Use `await list_inference_recommendations_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListInferenceRecommendationsJobsRequestRequestTypeDef](./type_defs.md#listinferencerecommendationsjobsrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `StatusEquals`:
  [RecommendationJobStatusType](./literals.md#recommendationjobstatustype)
- `SortBy`:
  [ListInferenceRecommendationsJobsSortByType](./literals.md#listinferencerecommendationsjobssortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListInferenceRecommendationsJobsResponseTypeDef](./type_defs.md#listinferencerecommendationsjobsresponsetypedef).

<a id="list_labeling_jobs"></a>

### list_labeling_jobs

Gets a list of labeling jobs.

Type annotations for
`aiobotocore.create_client("sagemaker").list_labeling_jobs` method.

Boto3 documentation:
[SageMaker.Client.list_labeling_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_labeling_jobs)

Asynchronous method. Use `await list_labeling_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListLabelingJobsRequestRequestTypeDef](./type_defs.md#listlabelingjobsrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NextToken`: `str`
- `NameContains`: `str`
- `SortBy`: [SortByType](./literals.md#sortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `StatusEquals`: [LabelingJobStatusType](./literals.md#labelingjobstatustype)

Returns a `Coroutine` for
[ListLabelingJobsResponseTypeDef](./type_defs.md#listlabelingjobsresponsetypedef).

<a id="list_labeling_jobs_for_workteam"></a>

### list_labeling_jobs_for_workteam

Gets a list of labeling jobs assigned to a specified work team.

Type annotations for
`aiobotocore.create_client("sagemaker").list_labeling_jobs_for_workteam`
method.

Boto3 documentation:
[SageMaker.Client.list_labeling_jobs_for_workteam](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_labeling_jobs_for_workteam)

Asynchronous method. Use `await list_labeling_jobs_for_workteam(...)` for a
synchronous call.

Arguments mapping described in
[ListLabelingJobsForWorkteamRequestRequestTypeDef](./type_defs.md#listlabelingjobsforworkteamrequestrequesttypedef).

Keyword-only arguments:

- `WorkteamArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `JobReferenceCodeContains`: `str`
- `SortBy`: `Literal['CreationTime']` (see
  [ListLabelingJobsForWorkteamSortByOptionsType](./literals.md#listlabelingjobsforworkteamsortbyoptionstype))
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListLabelingJobsForWorkteamResponseTypeDef](./type_defs.md#listlabelingjobsforworkteamresponsetypedef).

<a id="list_lineage_groups"></a>

### list_lineage_groups

A list of lineage groups shared with your Amazon Web Services account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_lineage_groups` method.

Boto3 documentation:
[SageMaker.Client.list_lineage_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_lineage_groups)

Asynchronous method. Use `await list_lineage_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListLineageGroupsRequestRequestTypeDef](./type_defs.md#listlineagegroupsrequestrequesttypedef).

Keyword-only arguments:

- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: [SortLineageGroupsByType](./literals.md#sortlineagegroupsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListLineageGroupsResponseTypeDef](./type_defs.md#listlineagegroupsresponsetypedef).

<a id="list_model_bias_job_definitions"></a>

### list_model_bias_job_definitions

Lists model bias jobs definitions that satisfy various filters.

Type annotations for
`aiobotocore.create_client("sagemaker").list_model_bias_job_definitions`
method.

Boto3 documentation:
[SageMaker.Client.list_model_bias_job_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_bias_job_definitions)

Asynchronous method. Use `await list_model_bias_job_definitions(...)` for a
synchronous call.

Arguments mapping described in
[ListModelBiasJobDefinitionsRequestRequestTypeDef](./type_defs.md#listmodelbiasjobdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str`
- `SortBy`:
  [MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[ListModelBiasJobDefinitionsResponseTypeDef](./type_defs.md#listmodelbiasjobdefinitionsresponsetypedef).

<a id="list_model_explainability_job_definitions"></a>

### list_model_explainability_job_definitions

Lists model explainability job definitions that satisfy various filters.

Type annotations for
`aiobotocore.create_client("sagemaker").list_model_explainability_job_definitions`
method.

Boto3 documentation:
[SageMaker.Client.list_model_explainability_job_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_explainability_job_definitions)

Asynchronous method. Use `await list_model_explainability_job_definitions(...)`
for a synchronous call.

Arguments mapping described in
[ListModelExplainabilityJobDefinitionsRequestRequestTypeDef](./type_defs.md#listmodelexplainabilityjobdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str`
- `SortBy`:
  [MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[ListModelExplainabilityJobDefinitionsResponseTypeDef](./type_defs.md#listmodelexplainabilityjobdefinitionsresponsetypedef).

<a id="list_model_metadata"></a>

### list_model_metadata

Lists the domain, framework, task, and model name of standard machine learning
models found in common model zoos.

Type annotations for
`aiobotocore.create_client("sagemaker").list_model_metadata` method.

Boto3 documentation:
[SageMaker.Client.list_model_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_metadata)

Asynchronous method. Use `await list_model_metadata(...)` for a synchronous
call.

Arguments mapping described in
[ListModelMetadataRequestRequestTypeDef](./type_defs.md#listmodelmetadatarequestrequesttypedef).

Keyword-only arguments:

- `SearchExpression`:
  [ModelMetadataSearchExpressionTypeDef](./type_defs.md#modelmetadatasearchexpressiontypedef)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListModelMetadataResponseTypeDef](./type_defs.md#listmodelmetadataresponsetypedef).

<a id="list_model_package_groups"></a>

### list_model_package_groups

Gets a list of the model groups in your Amazon Web Services account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_model_package_groups` method.

Boto3 documentation:
[SageMaker.Client.list_model_package_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_package_groups)

Asynchronous method. Use `await list_model_package_groups(...)` for a
synchronous call.

Arguments mapping described in
[ListModelPackageGroupsInputRequestTypeDef](./type_defs.md#listmodelpackagegroupsinputrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NameContains`: `str`
- `NextToken`: `str`
- `SortBy`:
  [ModelPackageGroupSortByType](./literals.md#modelpackagegroupsortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListModelPackageGroupsOutputTypeDef](./type_defs.md#listmodelpackagegroupsoutputtypedef).

<a id="list_model_packages"></a>

### list_model_packages

Lists the model packages that have been created.

Type annotations for
`aiobotocore.create_client("sagemaker").list_model_packages` method.

Boto3 documentation:
[SageMaker.Client.list_model_packages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_packages)

Asynchronous method. Use `await list_model_packages(...)` for a synchronous
call.

Arguments mapping described in
[ListModelPackagesInputRequestTypeDef](./type_defs.md#listmodelpackagesinputrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NameContains`: `str`
- `ModelApprovalStatus`:
  [ModelApprovalStatusType](./literals.md#modelapprovalstatustype)
- `ModelPackageGroupName`: `str`
- `ModelPackageType`:
  [ModelPackageTypeType](./literals.md#modelpackagetypetype)
- `NextToken`: `str`
- `SortBy`: [ModelPackageSortByType](./literals.md#modelpackagesortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListModelPackagesOutputTypeDef](./type_defs.md#listmodelpackagesoutputtypedef).

<a id="list_model_quality_job_definitions"></a>

### list_model_quality_job_definitions

Gets a list of model quality monitoring job definitions in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_model_quality_job_definitions`
method.

Boto3 documentation:
[SageMaker.Client.list_model_quality_job_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_quality_job_definitions)

Asynchronous method. Use `await list_model_quality_job_definitions(...)` for a
synchronous call.

Arguments mapping described in
[ListModelQualityJobDefinitionsRequestRequestTypeDef](./type_defs.md#listmodelqualityjobdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str`
- `SortBy`:
  [MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[ListModelQualityJobDefinitionsResponseTypeDef](./type_defs.md#listmodelqualityjobdefinitionsresponsetypedef).

<a id="list_models"></a>

### list_models

Lists models created with the `CreateModel` API.

Type annotations for `aiobotocore.create_client("sagemaker").list_models`
method.

Boto3 documentation:
[SageMaker.Client.list_models](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_models)

Asynchronous method. Use `await list_models(...)` for a synchronous call.

Arguments mapping described in
[ListModelsInputRequestTypeDef](./type_defs.md#listmodelsinputrequesttypedef).

Keyword-only arguments:

- `SortBy`: [ModelSortKeyType](./literals.md#modelsortkeytype)
- `SortOrder`: [OrderKeyType](./literals.md#orderkeytype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[ListModelsOutputTypeDef](./type_defs.md#listmodelsoutputtypedef).

<a id="list_monitoring_executions"></a>

### list_monitoring_executions

Returns list of all monitoring job executions.

Type annotations for
`aiobotocore.create_client("sagemaker").list_monitoring_executions` method.

Boto3 documentation:
[SageMaker.Client.list_monitoring_executions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_executions)

Asynchronous method. Use `await list_monitoring_executions(...)` for a
synchronous call.

Arguments mapping described in
[ListMonitoringExecutionsRequestRequestTypeDef](./type_defs.md#listmonitoringexecutionsrequestrequesttypedef).

Keyword-only arguments:

- `MonitoringScheduleName`: `str`
- `EndpointName`: `str`
- `SortBy`:
  [MonitoringExecutionSortKeyType](./literals.md#monitoringexecutionsortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `ScheduledTimeBefore`: `Union`\[`datetime`, `str`\]
- `ScheduledTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `StatusEquals`: [ExecutionStatusType](./literals.md#executionstatustype)
- `MonitoringJobDefinitionName`: `str`
- `MonitoringTypeEquals`:
  [MonitoringTypeType](./literals.md#monitoringtypetype)

Returns a `Coroutine` for
[ListMonitoringExecutionsResponseTypeDef](./type_defs.md#listmonitoringexecutionsresponsetypedef).

<a id="list_monitoring_schedules"></a>

### list_monitoring_schedules

Returns list of all monitoring schedules.

Type annotations for
`aiobotocore.create_client("sagemaker").list_monitoring_schedules` method.

Boto3 documentation:
[SageMaker.Client.list_monitoring_schedules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_schedules)

Asynchronous method. Use `await list_monitoring_schedules(...)` for a
synchronous call.

Arguments mapping described in
[ListMonitoringSchedulesRequestRequestTypeDef](./type_defs.md#listmonitoringschedulesrequestrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str`
- `SortBy`:
  [MonitoringScheduleSortKeyType](./literals.md#monitoringschedulesortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `StatusEquals`: [ScheduleStatusType](./literals.md#schedulestatustype)
- `MonitoringJobDefinitionName`: `str`
- `MonitoringTypeEquals`:
  [MonitoringTypeType](./literals.md#monitoringtypetype)

Returns a `Coroutine` for
[ListMonitoringSchedulesResponseTypeDef](./type_defs.md#listmonitoringschedulesresponsetypedef).

<a id="list_notebook_instance_lifecycle_configs"></a>

### list_notebook_instance_lifecycle_configs

Lists notebook instance lifestyle configurations created with the
CreateNotebookInstanceLifecycleConfig API.

Type annotations for
`aiobotocore.create_client("sagemaker").list_notebook_instance_lifecycle_configs`
method.

Boto3 documentation:
[SageMaker.Client.list_notebook_instance_lifecycle_configs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_notebook_instance_lifecycle_configs)

Asynchronous method. Use `await list_notebook_instance_lifecycle_configs(...)`
for a synchronous call.

Arguments mapping described in
[ListNotebookInstanceLifecycleConfigsInputRequestTypeDef](./type_defs.md#listnotebookinstancelifecycleconfigsinputrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `SortBy`:
  [NotebookInstanceLifecycleConfigSortKeyType](./literals.md#notebookinstancelifecycleconfigsortkeytype)
- `SortOrder`:
  [NotebookInstanceLifecycleConfigSortOrderType](./literals.md#notebookinstancelifecycleconfigsortordertype)
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[ListNotebookInstanceLifecycleConfigsOutputTypeDef](./type_defs.md#listnotebookinstancelifecycleconfigsoutputtypedef).

<a id="list_notebook_instances"></a>

### list_notebook_instances

Returns a list of the Amazon SageMaker notebook instances in the requester's
account in an Amazon Web Services Region.

Type annotations for
`aiobotocore.create_client("sagemaker").list_notebook_instances` method.

Boto3 documentation:
[SageMaker.Client.list_notebook_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_notebook_instances)

Asynchronous method. Use `await list_notebook_instances(...)` for a synchronous
call.

Arguments mapping described in
[ListNotebookInstancesInputRequestTypeDef](./type_defs.md#listnotebookinstancesinputrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `SortBy`:
  [NotebookInstanceSortKeyType](./literals.md#notebookinstancesortkeytype)
- `SortOrder`:
  [NotebookInstanceSortOrderType](./literals.md#notebookinstancesortordertype)
- `NameContains`: `str`
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `StatusEquals`:
  [NotebookInstanceStatusType](./literals.md#notebookinstancestatustype)
- `NotebookInstanceLifecycleConfigNameContains`: `str`
- `DefaultCodeRepositoryContains`: `str`
- `AdditionalCodeRepositoryEquals`: `str`

Returns a `Coroutine` for
[ListNotebookInstancesOutputTypeDef](./type_defs.md#listnotebookinstancesoutputtypedef).

<a id="list_pipeline_execution_steps"></a>

### list_pipeline_execution_steps

Gets a list of `PipeLineExecutionStep` objects.

Type annotations for
`aiobotocore.create_client("sagemaker").list_pipeline_execution_steps` method.

Boto3 documentation:
[SageMaker.Client.list_pipeline_execution_steps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipeline_execution_steps)

Asynchronous method. Use `await list_pipeline_execution_steps(...)` for a
synchronous call.

Arguments mapping described in
[ListPipelineExecutionStepsRequestRequestTypeDef](./type_defs.md#listpipelineexecutionstepsrequestrequesttypedef).

Keyword-only arguments:

- `PipelineExecutionArn`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListPipelineExecutionStepsResponseTypeDef](./type_defs.md#listpipelineexecutionstepsresponsetypedef).

<a id="list_pipeline_executions"></a>

### list_pipeline_executions

Gets a list of the pipeline executions.

Type annotations for
`aiobotocore.create_client("sagemaker").list_pipeline_executions` method.

Boto3 documentation:
[SageMaker.Client.list_pipeline_executions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipeline_executions)

Asynchronous method. Use `await list_pipeline_executions(...)` for a
synchronous call.

Arguments mapping described in
[ListPipelineExecutionsRequestRequestTypeDef](./type_defs.md#listpipelineexecutionsrequestrequesttypedef).

Keyword-only arguments:

- `PipelineName`: `str` *(required)*
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`:
  [SortPipelineExecutionsByType](./literals.md#sortpipelineexecutionsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListPipelineExecutionsResponseTypeDef](./type_defs.md#listpipelineexecutionsresponsetypedef).

<a id="list_pipeline_parameters_for_execution"></a>

### list_pipeline_parameters_for_execution

Gets a list of parameters for a pipeline execution.

Type annotations for
`aiobotocore.create_client("sagemaker").list_pipeline_parameters_for_execution`
method.

Boto3 documentation:
[SageMaker.Client.list_pipeline_parameters_for_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipeline_parameters_for_execution)

Asynchronous method. Use `await list_pipeline_parameters_for_execution(...)`
for a synchronous call.

Arguments mapping described in
[ListPipelineParametersForExecutionRequestRequestTypeDef](./type_defs.md#listpipelineparametersforexecutionrequestrequesttypedef).

Keyword-only arguments:

- `PipelineExecutionArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListPipelineParametersForExecutionResponseTypeDef](./type_defs.md#listpipelineparametersforexecutionresponsetypedef).

<a id="list_pipelines"></a>

### list_pipelines

Gets a list of pipelines.

Type annotations for `aiobotocore.create_client("sagemaker").list_pipelines`
method.

Boto3 documentation:
[SageMaker.Client.list_pipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipelines)

Asynchronous method. Use `await list_pipelines(...)` for a synchronous call.

Arguments mapping described in
[ListPipelinesRequestRequestTypeDef](./type_defs.md#listpipelinesrequestrequesttypedef).

Keyword-only arguments:

- `PipelineNamePrefix`: `str`
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: [SortPipelinesByType](./literals.md#sortpipelinesbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef).

<a id="list_processing_jobs"></a>

### list_processing_jobs

Lists processing jobs that satisfy various filters.

Type annotations for
`aiobotocore.create_client("sagemaker").list_processing_jobs` method.

Boto3 documentation:
[SageMaker.Client.list_processing_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_processing_jobs)

Asynchronous method. Use `await list_processing_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListProcessingJobsRequestRequestTypeDef](./type_defs.md#listprocessingjobsrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `StatusEquals`:
  [ProcessingJobStatusType](./literals.md#processingjobstatustype)
- `SortBy`: [SortByType](./literals.md#sortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListProcessingJobsResponseTypeDef](./type_defs.md#listprocessingjobsresponsetypedef).

<a id="list_projects"></a>

### list_projects

Gets a list of the projects in an Amazon Web Services account.

Type annotations for `aiobotocore.create_client("sagemaker").list_projects`
method.

Boto3 documentation:
[SageMaker.Client.list_projects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_projects)

Asynchronous method. Use `await list_projects(...)` for a synchronous call.

Arguments mapping described in
[ListProjectsInputRequestTypeDef](./type_defs.md#listprojectsinputrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `MaxResults`: `int`
- `NameContains`: `str`
- `NextToken`: `str`
- `SortBy`: [ProjectSortByType](./literals.md#projectsortbytype)
- `SortOrder`: [ProjectSortOrderType](./literals.md#projectsortordertype)

Returns a `Coroutine` for
[ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef).

<a id="list_studio_lifecycle_configs"></a>

### list_studio_lifecycle_configs

Lists the Studio Lifecycle Configurations in your Amazon Web Services Account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_studio_lifecycle_configs` method.

Boto3 documentation:
[SageMaker.Client.list_studio_lifecycle_configs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_studio_lifecycle_configs)

Asynchronous method. Use `await list_studio_lifecycle_configs(...)` for a
synchronous call.

Arguments mapping described in
[ListStudioLifecycleConfigsRequestRequestTypeDef](./type_defs.md#liststudiolifecycleconfigsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `NameContains`: `str`
- `AppTypeEquals`:
  [StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype)
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `ModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `ModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `SortBy`:
  [StudioLifecycleConfigSortKeyType](./literals.md#studiolifecycleconfigsortkeytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListStudioLifecycleConfigsResponseTypeDef](./type_defs.md#liststudiolifecycleconfigsresponsetypedef).

<a id="list_subscribed_workteams"></a>

### list_subscribed_workteams

Gets a list of the work teams that you are subscribed to in the Amazon Web
Services Marketplace.

Type annotations for
`aiobotocore.create_client("sagemaker").list_subscribed_workteams` method.

Boto3 documentation:
[SageMaker.Client.list_subscribed_workteams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_subscribed_workteams)

Asynchronous method. Use `await list_subscribed_workteams(...)` for a
synchronous call.

Arguments mapping described in
[ListSubscribedWorkteamsRequestRequestTypeDef](./type_defs.md#listsubscribedworkteamsrequestrequesttypedef).

Keyword-only arguments:

- `NameContains`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListSubscribedWorkteamsResponseTypeDef](./type_defs.md#listsubscribedworkteamsresponsetypedef).

<a id="list_tags"></a>

### list_tags

Returns the tags for the specified Amazon SageMaker resource.

Type annotations for `aiobotocore.create_client("sagemaker").list_tags` method.

Boto3 documentation:
[SageMaker.Client.list_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_tags)

Asynchronous method. Use `await list_tags(...)` for a synchronous call.

Arguments mapping described in
[ListTagsInputRequestTypeDef](./type_defs.md#listtagsinputrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListTagsOutputTypeDef](./type_defs.md#listtagsoutputtypedef).

<a id="list_training_jobs"></a>

### list_training_jobs

Lists training jobs.

Type annotations for
`aiobotocore.create_client("sagemaker").list_training_jobs` method.

Boto3 documentation:
[SageMaker.Client.list_training_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_training_jobs)

Asynchronous method. Use `await list_training_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListTrainingJobsRequestRequestTypeDef](./type_defs.md#listtrainingjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `StatusEquals`: [TrainingJobStatusType](./literals.md#trainingjobstatustype)
- `SortBy`: [SortByType](./literals.md#sortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListTrainingJobsResponseTypeDef](./type_defs.md#listtrainingjobsresponsetypedef).

<a id="list_training_jobs_for_hyper_parameter_tuning_job"></a>

### list_training_jobs_for_hyper_parameter_tuning_job

Gets a list of TrainingJobSummary objects that describe the training jobs that
a hyperparameter tuning job launched.

Type annotations for
`aiobotocore.create_client("sagemaker").list_training_jobs_for_hyper_parameter_tuning_job`
method.

Boto3 documentation:
[SageMaker.Client.list_training_jobs_for_hyper_parameter_tuning_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_training_jobs_for_hyper_parameter_tuning_job)

Asynchronous method. Use
`await list_training_jobs_for_hyper_parameter_tuning_job(...)` for a
synchronous call.

Arguments mapping described in
[ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef](./type_defs.md#listtrainingjobsforhyperparametertuningjobrequestrequesttypedef).

Keyword-only arguments:

- `HyperParameterTuningJobName`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`
- `StatusEquals`: [TrainingJobStatusType](./literals.md#trainingjobstatustype)
- `SortBy`:
  [TrainingJobSortByOptionsType](./literals.md#trainingjobsortbyoptionstype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)

Returns a `Coroutine` for
[ListTrainingJobsForHyperParameterTuningJobResponseTypeDef](./type_defs.md#listtrainingjobsforhyperparametertuningjobresponsetypedef).

<a id="list_transform_jobs"></a>

### list_transform_jobs

Lists transform jobs.

Type annotations for
`aiobotocore.create_client("sagemaker").list_transform_jobs` method.

Boto3 documentation:
[SageMaker.Client.list_transform_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_transform_jobs)

Asynchronous method. Use `await list_transform_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListTransformJobsRequestRequestTypeDef](./type_defs.md#listtransformjobsrequestrequesttypedef).

Keyword-only arguments:

- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeAfter`: `Union`\[`datetime`, `str`\]
- `LastModifiedTimeBefore`: `Union`\[`datetime`, `str`\]
- `NameContains`: `str`
- `StatusEquals`:
  [TransformJobStatusType](./literals.md#transformjobstatustype)
- `SortBy`: [SortByType](./literals.md#sortbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListTransformJobsResponseTypeDef](./type_defs.md#listtransformjobsresponsetypedef).

<a id="list_trial_components"></a>

### list_trial_components

Lists the trial components in your account.

Type annotations for
`aiobotocore.create_client("sagemaker").list_trial_components` method.

Boto3 documentation:
[SageMaker.Client.list_trial_components](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_trial_components)

Asynchronous method. Use `await list_trial_components(...)` for a synchronous
call.

Arguments mapping described in
[ListTrialComponentsRequestRequestTypeDef](./type_defs.md#listtrialcomponentsrequestrequesttypedef).

Keyword-only arguments:

- `ExperimentName`: `str`
- `TrialName`: `str`
- `SourceArn`: `str`
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`:
  [SortTrialComponentsByType](./literals.md#sorttrialcomponentsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListTrialComponentsResponseTypeDef](./type_defs.md#listtrialcomponentsresponsetypedef).

<a id="list_trials"></a>

### list_trials

Lists the trials in your account.

Type annotations for `aiobotocore.create_client("sagemaker").list_trials`
method.

Boto3 documentation:
[SageMaker.Client.list_trials](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_trials)

Asynchronous method. Use `await list_trials(...)` for a synchronous call.

Arguments mapping described in
[ListTrialsRequestRequestTypeDef](./type_defs.md#listtrialsrequestrequesttypedef).

Keyword-only arguments:

- `ExperimentName`: `str`
- `TrialComponentName`: `str`
- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `SortBy`: [SortTrialsByType](./literals.md#sorttrialsbytype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListTrialsResponseTypeDef](./type_defs.md#listtrialsresponsetypedef).

<a id="list_user_profiles"></a>

### list_user_profiles

Lists user profiles.

Type annotations for
`aiobotocore.create_client("sagemaker").list_user_profiles` method.

Boto3 documentation:
[SageMaker.Client.list_user_profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_user_profiles)

Asynchronous method. Use `await list_user_profiles(...)` for a synchronous
call.

Arguments mapping described in
[ListUserProfilesRequestRequestTypeDef](./type_defs.md#listuserprofilesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `SortBy`: [UserProfileSortKeyType](./literals.md#userprofilesortkeytype)
- `DomainIdEquals`: `str`
- `UserProfileNameContains`: `str`

Returns a `Coroutine` for
[ListUserProfilesResponseTypeDef](./type_defs.md#listuserprofilesresponsetypedef).

<a id="list_workforces"></a>

### list_workforces

Use this operation to list all private and vendor workforces in an Amazon Web
Services Region.

Type annotations for `aiobotocore.create_client("sagemaker").list_workforces`
method.

Boto3 documentation:
[SageMaker.Client.list_workforces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_workforces)

Asynchronous method. Use `await list_workforces(...)` for a synchronous call.

Arguments mapping described in
[ListWorkforcesRequestRequestTypeDef](./type_defs.md#listworkforcesrequestrequesttypedef).

Keyword-only arguments:

- `SortBy`:
  [ListWorkforcesSortByOptionsType](./literals.md#listworkforcessortbyoptionstype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NameContains`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListWorkforcesResponseTypeDef](./type_defs.md#listworkforcesresponsetypedef).

<a id="list_workteams"></a>

### list_workteams

Gets a list of private work teams that you have defined in a region.

Type annotations for `aiobotocore.create_client("sagemaker").list_workteams`
method.

Boto3 documentation:
[SageMaker.Client.list_workteams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_workteams)

Asynchronous method. Use `await list_workteams(...)` for a synchronous call.

Arguments mapping described in
[ListWorkteamsRequestRequestTypeDef](./type_defs.md#listworkteamsrequestrequesttypedef).

Keyword-only arguments:

- `SortBy`:
  [ListWorkteamsSortByOptionsType](./literals.md#listworkteamssortbyoptionstype)
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NameContains`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListWorkteamsResponseTypeDef](./type_defs.md#listworkteamsresponsetypedef).

<a id="put_model_package_group_policy"></a>

### put_model_package_group_policy

Adds a resouce policy to control access to a model group.

Type annotations for
`aiobotocore.create_client("sagemaker").put_model_package_group_policy` method.

Boto3 documentation:
[SageMaker.Client.put_model_package_group_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.put_model_package_group_policy)

Asynchronous method. Use `await put_model_package_group_policy(...)` for a
synchronous call.

Arguments mapping described in
[PutModelPackageGroupPolicyInputRequestTypeDef](./type_defs.md#putmodelpackagegrouppolicyinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageGroupName`: `str` *(required)*
- `ResourcePolicy`: `str` *(required)*

Returns a `Coroutine` for
[PutModelPackageGroupPolicyOutputTypeDef](./type_defs.md#putmodelpackagegrouppolicyoutputtypedef).

<a id="query_lineage"></a>

### query_lineage

Use this action to inspect your lineage and discover relationships between
entities.

Type annotations for `aiobotocore.create_client("sagemaker").query_lineage`
method.

Boto3 documentation:
[SageMaker.Client.query_lineage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.query_lineage)

Asynchronous method. Use `await query_lineage(...)` for a synchronous call.

Arguments mapping described in
[QueryLineageRequestRequestTypeDef](./type_defs.md#querylineagerequestrequesttypedef).

Keyword-only arguments:

- `StartArns`: `Sequence`\[`str`\] *(required)*
- `Direction`: [DirectionType](./literals.md#directiontype)
- `IncludeEdges`: `bool`
- `Filters`: [QueryFiltersTypeDef](./type_defs.md#queryfilterstypedef)
- `MaxDepth`: `int`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[QueryLineageResponseTypeDef](./type_defs.md#querylineageresponsetypedef).

<a id="register_devices"></a>

### register_devices

Register devices.

Type annotations for `aiobotocore.create_client("sagemaker").register_devices`
method.

Boto3 documentation:
[SageMaker.Client.register_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.register_devices)

Asynchronous method. Use `await register_devices(...)` for a synchronous call.

Arguments mapping described in
[RegisterDevicesRequestRequestTypeDef](./type_defs.md#registerdevicesrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*
- `Devices`: `Sequence`\[[DeviceTypeDef](./type_defs.md#devicetypedef)\]
  *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="render_ui_template"></a>

### render_ui_template

Renders the UI template so that you can preview the worker's experience.

Type annotations for
`aiobotocore.create_client("sagemaker").render_ui_template` method.

Boto3 documentation:
[SageMaker.Client.render_ui_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.render_ui_template)

Asynchronous method. Use `await render_ui_template(...)` for a synchronous
call.

Arguments mapping described in
[RenderUiTemplateRequestRequestTypeDef](./type_defs.md#renderuitemplaterequestrequesttypedef).

Keyword-only arguments:

- `Task`: [RenderableTaskTypeDef](./type_defs.md#renderabletasktypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `UiTemplate`: [UiTemplateTypeDef](./type_defs.md#uitemplatetypedef)
- `HumanTaskUiArn`: `str`

Returns a `Coroutine` for
[RenderUiTemplateResponseTypeDef](./type_defs.md#renderuitemplateresponsetypedef).

<a id="retry_pipeline_execution"></a>

### retry_pipeline_execution

Retry the execution of the pipeline.

Type annotations for
`aiobotocore.create_client("sagemaker").retry_pipeline_execution` method.

Boto3 documentation:
[SageMaker.Client.retry_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.retry_pipeline_execution)

Asynchronous method. Use `await retry_pipeline_execution(...)` for a
synchronous call.

Arguments mapping described in
[RetryPipelineExecutionRequestRequestTypeDef](./type_defs.md#retrypipelineexecutionrequestrequesttypedef).

Keyword-only arguments:

- `PipelineExecutionArn`: `str` *(required)*
- `ClientRequestToken`: `str` *(required)*

Returns a `Coroutine` for
[RetryPipelineExecutionResponseTypeDef](./type_defs.md#retrypipelineexecutionresponsetypedef).

<a id="search"></a>

### search

Finds Amazon SageMaker resources that match a search query.

Type annotations for `aiobotocore.create_client("sagemaker").search` method.

Boto3 documentation:
[SageMaker.Client.search](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.search)

Asynchronous method. Use `await search(...)` for a synchronous call.

Arguments mapping described in
[SearchRequestRequestTypeDef](./type_defs.md#searchrequestrequesttypedef).

Keyword-only arguments:

- `Resource`: [ResourceTypeType](./literals.md#resourcetypetype) *(required)*
- `SearchExpression`:
  [SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
- `SortBy`: `str`
- `SortOrder`: [SearchSortOrderType](./literals.md#searchsortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[SearchResponseTypeDef](./type_defs.md#searchresponsetypedef).

<a id="send_pipeline_execution_step_failure"></a>

### send_pipeline_execution_step_failure

Notifies the pipeline that the execution of a callback step failed, along with
a message describing why.

Type annotations for
`aiobotocore.create_client("sagemaker").send_pipeline_execution_step_failure`
method.

Boto3 documentation:
[SageMaker.Client.send_pipeline_execution_step_failure](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.send_pipeline_execution_step_failure)

Asynchronous method. Use `await send_pipeline_execution_step_failure(...)` for
a synchronous call.

Arguments mapping described in
[SendPipelineExecutionStepFailureRequestRequestTypeDef](./type_defs.md#sendpipelineexecutionstepfailurerequestrequesttypedef).

Keyword-only arguments:

- `CallbackToken`: `str` *(required)*
- `FailureReason`: `str`
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[SendPipelineExecutionStepFailureResponseTypeDef](./type_defs.md#sendpipelineexecutionstepfailureresponsetypedef).

<a id="send_pipeline_execution_step_success"></a>

### send_pipeline_execution_step_success

Notifies the pipeline that the execution of a callback step succeeded and
provides a list of the step's output parameters.

Type annotations for
`aiobotocore.create_client("sagemaker").send_pipeline_execution_step_success`
method.

Boto3 documentation:
[SageMaker.Client.send_pipeline_execution_step_success](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.send_pipeline_execution_step_success)

Asynchronous method. Use `await send_pipeline_execution_step_success(...)` for
a synchronous call.

Arguments mapping described in
[SendPipelineExecutionStepSuccessRequestRequestTypeDef](./type_defs.md#sendpipelineexecutionstepsuccessrequestrequesttypedef).

Keyword-only arguments:

- `CallbackToken`: `str` *(required)*
- `OutputParameters`:
  `Sequence`\[[OutputParameterTypeDef](./type_defs.md#outputparametertypedef)\]
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[SendPipelineExecutionStepSuccessResponseTypeDef](./type_defs.md#sendpipelineexecutionstepsuccessresponsetypedef).

<a id="start_monitoring_schedule"></a>

### start_monitoring_schedule

Starts a previously stopped monitoring schedule.

Type annotations for
`aiobotocore.create_client("sagemaker").start_monitoring_schedule` method.

Boto3 documentation:
[SageMaker.Client.start_monitoring_schedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_monitoring_schedule)

Asynchronous method. Use `await start_monitoring_schedule(...)` for a
synchronous call.

Arguments mapping described in
[StartMonitoringScheduleRequestRequestTypeDef](./type_defs.md#startmonitoringschedulerequestrequesttypedef).

Keyword-only arguments:

- `MonitoringScheduleName`: `str` *(required)*

<a id="start_notebook_instance"></a>

### start_notebook_instance

Launches an ML compute instance with the latest version of the libraries and
attaches your ML storage volume.

Type annotations for
`aiobotocore.create_client("sagemaker").start_notebook_instance` method.

Boto3 documentation:
[SageMaker.Client.start_notebook_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_notebook_instance)

Asynchronous method. Use `await start_notebook_instance(...)` for a synchronous
call.

Arguments mapping described in
[StartNotebookInstanceInputRequestTypeDef](./type_defs.md#startnotebookinstanceinputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceName`: `str` *(required)*

<a id="start_pipeline_execution"></a>

### start_pipeline_execution

Starts a pipeline execution.

Type annotations for
`aiobotocore.create_client("sagemaker").start_pipeline_execution` method.

Boto3 documentation:
[SageMaker.Client.start_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_pipeline_execution)

Asynchronous method. Use `await start_pipeline_execution(...)` for a
synchronous call.

Arguments mapping described in
[StartPipelineExecutionRequestRequestTypeDef](./type_defs.md#startpipelineexecutionrequestrequesttypedef).

Keyword-only arguments:

- `PipelineName`: `str` *(required)*
- `ClientRequestToken`: `str` *(required)*
- `PipelineExecutionDisplayName`: `str`
- `PipelineParameters`:
  `Sequence`\[[ParameterTypeDef](./type_defs.md#parametertypedef)\]
- `PipelineExecutionDescription`: `str`

Returns a `Coroutine` for
[StartPipelineExecutionResponseTypeDef](./type_defs.md#startpipelineexecutionresponsetypedef).

<a id="stop_auto_ml_job"></a>

### stop_auto_ml_job

A method for forcing the termination of a running job.

Type annotations for `aiobotocore.create_client("sagemaker").stop_auto_ml_job`
method.

Boto3 documentation:
[SageMaker.Client.stop_auto_ml_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_auto_ml_job)

Asynchronous method. Use `await stop_auto_ml_job(...)` for a synchronous call.

Arguments mapping described in
[StopAutoMLJobRequestRequestTypeDef](./type_defs.md#stopautomljobrequestrequesttypedef).

Keyword-only arguments:

- `AutoMLJobName`: `str` *(required)*

<a id="stop_compilation_job"></a>

### stop_compilation_job

Stops a model compilation job.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_compilation_job` method.

Boto3 documentation:
[SageMaker.Client.stop_compilation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_compilation_job)

Asynchronous method. Use `await stop_compilation_job(...)` for a synchronous
call.

Arguments mapping described in
[StopCompilationJobRequestRequestTypeDef](./type_defs.md#stopcompilationjobrequestrequesttypedef).

Keyword-only arguments:

- `CompilationJobName`: `str` *(required)*

<a id="stop_edge_packaging_job"></a>

### stop_edge_packaging_job

Request to stop an edge packaging job.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_edge_packaging_job` method.

Boto3 documentation:
[SageMaker.Client.stop_edge_packaging_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_edge_packaging_job)

Asynchronous method. Use `await stop_edge_packaging_job(...)` for a synchronous
call.

Arguments mapping described in
[StopEdgePackagingJobRequestRequestTypeDef](./type_defs.md#stopedgepackagingjobrequestrequesttypedef).

Keyword-only arguments:

- `EdgePackagingJobName`: `str` *(required)*

<a id="stop_hyper_parameter_tuning_job"></a>

### stop_hyper_parameter_tuning_job

Stops a running hyperparameter tuning job and all running training jobs that
the tuning job launched.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_hyper_parameter_tuning_job`
method.

Boto3 documentation:
[SageMaker.Client.stop_hyper_parameter_tuning_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_hyper_parameter_tuning_job)

Asynchronous method. Use `await stop_hyper_parameter_tuning_job(...)` for a
synchronous call.

Arguments mapping described in
[StopHyperParameterTuningJobRequestRequestTypeDef](./type_defs.md#stophyperparametertuningjobrequestrequesttypedef).

Keyword-only arguments:

- `HyperParameterTuningJobName`: `str` *(required)*

<a id="stop_inference_recommendations_job"></a>

### stop_inference_recommendations_job

Stops an Inference Recommender job.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_inference_recommendations_job`
method.

Boto3 documentation:
[SageMaker.Client.stop_inference_recommendations_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_inference_recommendations_job)

Asynchronous method. Use `await stop_inference_recommendations_job(...)` for a
synchronous call.

Arguments mapping described in
[StopInferenceRecommendationsJobRequestRequestTypeDef](./type_defs.md#stopinferencerecommendationsjobrequestrequesttypedef).

Keyword-only arguments:

- `JobName`: `str` *(required)*

<a id="stop_labeling_job"></a>

### stop_labeling_job

Stops a running labeling job.

Type annotations for `aiobotocore.create_client("sagemaker").stop_labeling_job`
method.

Boto3 documentation:
[SageMaker.Client.stop_labeling_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_labeling_job)

Asynchronous method. Use `await stop_labeling_job(...)` for a synchronous call.

Arguments mapping described in
[StopLabelingJobRequestRequestTypeDef](./type_defs.md#stoplabelingjobrequestrequesttypedef).

Keyword-only arguments:

- `LabelingJobName`: `str` *(required)*

<a id="stop_monitoring_schedule"></a>

### stop_monitoring_schedule

Stops a previously started monitoring schedule.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_monitoring_schedule` method.

Boto3 documentation:
[SageMaker.Client.stop_monitoring_schedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_monitoring_schedule)

Asynchronous method. Use `await stop_monitoring_schedule(...)` for a
synchronous call.

Arguments mapping described in
[StopMonitoringScheduleRequestRequestTypeDef](./type_defs.md#stopmonitoringschedulerequestrequesttypedef).

Keyword-only arguments:

- `MonitoringScheduleName`: `str` *(required)*

<a id="stop_notebook_instance"></a>

### stop_notebook_instance

Terminates the ML compute instance.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_notebook_instance` method.

Boto3 documentation:
[SageMaker.Client.stop_notebook_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_notebook_instance)

Asynchronous method. Use `await stop_notebook_instance(...)` for a synchronous
call.

Arguments mapping described in
[StopNotebookInstanceInputRequestTypeDef](./type_defs.md#stopnotebookinstanceinputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceName`: `str` *(required)*

<a id="stop_pipeline_execution"></a>

### stop_pipeline_execution

Stops a pipeline execution.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_pipeline_execution` method.

Boto3 documentation:
[SageMaker.Client.stop_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_pipeline_execution)

Asynchronous method. Use `await stop_pipeline_execution(...)` for a synchronous
call.

Arguments mapping described in
[StopPipelineExecutionRequestRequestTypeDef](./type_defs.md#stoppipelineexecutionrequestrequesttypedef).

Keyword-only arguments:

- `PipelineExecutionArn`: `str` *(required)*
- `ClientRequestToken`: `str` *(required)*

Returns a `Coroutine` for
[StopPipelineExecutionResponseTypeDef](./type_defs.md#stoppipelineexecutionresponsetypedef).

<a id="stop_processing_job"></a>

### stop_processing_job

Stops a processing job.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_processing_job` method.

Boto3 documentation:
[SageMaker.Client.stop_processing_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_processing_job)

Asynchronous method. Use `await stop_processing_job(...)` for a synchronous
call.

Arguments mapping described in
[StopProcessingJobRequestRequestTypeDef](./type_defs.md#stopprocessingjobrequestrequesttypedef).

Keyword-only arguments:

- `ProcessingJobName`: `str` *(required)*

<a id="stop_training_job"></a>

### stop_training_job

Stops a training job.

Type annotations for `aiobotocore.create_client("sagemaker").stop_training_job`
method.

Boto3 documentation:
[SageMaker.Client.stop_training_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_training_job)

Asynchronous method. Use `await stop_training_job(...)` for a synchronous call.

Arguments mapping described in
[StopTrainingJobRequestRequestTypeDef](./type_defs.md#stoptrainingjobrequestrequesttypedef).

Keyword-only arguments:

- `TrainingJobName`: `str` *(required)*

<a id="stop_transform_job"></a>

### stop_transform_job

Stops a transform job.

Type annotations for
`aiobotocore.create_client("sagemaker").stop_transform_job` method.

Boto3 documentation:
[SageMaker.Client.stop_transform_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_transform_job)

Asynchronous method. Use `await stop_transform_job(...)` for a synchronous
call.

Arguments mapping described in
[StopTransformJobRequestRequestTypeDef](./type_defs.md#stoptransformjobrequestrequesttypedef).

Keyword-only arguments:

- `TransformJobName`: `str` *(required)*

<a id="update_action"></a>

### update_action

Updates an action.

Type annotations for `aiobotocore.create_client("sagemaker").update_action`
method.

Boto3 documentation:
[SageMaker.Client.update_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_action)

Asynchronous method. Use `await update_action(...)` for a synchronous call.

Arguments mapping described in
[UpdateActionRequestRequestTypeDef](./type_defs.md#updateactionrequestrequesttypedef).

Keyword-only arguments:

- `ActionName`: `str` *(required)*
- `Description`: `str`
- `Status`: [ActionStatusType](./literals.md#actionstatustype)
- `Properties`: `Mapping`\[`str`, `str`\]
- `PropertiesToRemove`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[UpdateActionResponseTypeDef](./type_defs.md#updateactionresponsetypedef).

<a id="update_app_image_config"></a>

### update_app_image_config

Updates the properties of an AppImageConfig.

Type annotations for
`aiobotocore.create_client("sagemaker").update_app_image_config` method.

Boto3 documentation:
[SageMaker.Client.update_app_image_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_app_image_config)

Asynchronous method. Use `await update_app_image_config(...)` for a synchronous
call.

Arguments mapping described in
[UpdateAppImageConfigRequestRequestTypeDef](./type_defs.md#updateappimageconfigrequestrequesttypedef).

Keyword-only arguments:

- `AppImageConfigName`: `str` *(required)*
- `KernelGatewayImageConfig`:
  [KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef)

Returns a `Coroutine` for
[UpdateAppImageConfigResponseTypeDef](./type_defs.md#updateappimageconfigresponsetypedef).

<a id="update_artifact"></a>

### update_artifact

Updates an artifact.

Type annotations for `aiobotocore.create_client("sagemaker").update_artifact`
method.

Boto3 documentation:
[SageMaker.Client.update_artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_artifact)

Asynchronous method. Use `await update_artifact(...)` for a synchronous call.

Arguments mapping described in
[UpdateArtifactRequestRequestTypeDef](./type_defs.md#updateartifactrequestrequesttypedef).

Keyword-only arguments:

- `ArtifactArn`: `str` *(required)*
- `ArtifactName`: `str`
- `Properties`: `Mapping`\[`str`, `str`\]
- `PropertiesToRemove`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[UpdateArtifactResponseTypeDef](./type_defs.md#updateartifactresponsetypedef).

<a id="update_code_repository"></a>

### update_code_repository

Updates the specified Git repository with the specified values.

Type annotations for
`aiobotocore.create_client("sagemaker").update_code_repository` method.

Boto3 documentation:
[SageMaker.Client.update_code_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_code_repository)

Asynchronous method. Use `await update_code_repository(...)` for a synchronous
call.

Arguments mapping described in
[UpdateCodeRepositoryInputRequestTypeDef](./type_defs.md#updatecoderepositoryinputrequesttypedef).

Keyword-only arguments:

- `CodeRepositoryName`: `str` *(required)*
- `GitConfig`:
  [GitConfigForUpdateTypeDef](./type_defs.md#gitconfigforupdatetypedef)

Returns a `Coroutine` for
[UpdateCodeRepositoryOutputTypeDef](./type_defs.md#updatecoderepositoryoutputtypedef).

<a id="update_context"></a>

### update_context

Updates a context.

Type annotations for `aiobotocore.create_client("sagemaker").update_context`
method.

Boto3 documentation:
[SageMaker.Client.update_context](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_context)

Asynchronous method. Use `await update_context(...)` for a synchronous call.

Arguments mapping described in
[UpdateContextRequestRequestTypeDef](./type_defs.md#updatecontextrequestrequesttypedef).

Keyword-only arguments:

- `ContextName`: `str` *(required)*
- `Description`: `str`
- `Properties`: `Mapping`\[`str`, `str`\]
- `PropertiesToRemove`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[UpdateContextResponseTypeDef](./type_defs.md#updatecontextresponsetypedef).

<a id="update_device_fleet"></a>

### update_device_fleet

Updates a fleet of devices.

Type annotations for
`aiobotocore.create_client("sagemaker").update_device_fleet` method.

Boto3 documentation:
[SageMaker.Client.update_device_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_device_fleet)

Asynchronous method. Use `await update_device_fleet(...)` for a synchronous
call.

Arguments mapping described in
[UpdateDeviceFleetRequestRequestTypeDef](./type_defs.md#updatedevicefleetrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*
- `OutputConfig`:
  [EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef)
  *(required)*
- `RoleArn`: `str`
- `Description`: `str`
- `EnableIotRoleAlias`: `bool`

<a id="update_devices"></a>

### update_devices

Updates one or more devices in a fleet.

Type annotations for `aiobotocore.create_client("sagemaker").update_devices`
method.

Boto3 documentation:
[SageMaker.Client.update_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_devices)

Asynchronous method. Use `await update_devices(...)` for a synchronous call.

Arguments mapping described in
[UpdateDevicesRequestRequestTypeDef](./type_defs.md#updatedevicesrequestrequesttypedef).

Keyword-only arguments:

- `DeviceFleetName`: `str` *(required)*
- `Devices`: `Sequence`\[[DeviceTypeDef](./type_defs.md#devicetypedef)\]
  *(required)*

<a id="update_domain"></a>

### update_domain

Updates the default settings for new user profiles in the domain.

Type annotations for `aiobotocore.create_client("sagemaker").update_domain`
method.

Boto3 documentation:
[SageMaker.Client.update_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_domain)

Asynchronous method. Use `await update_domain(...)` for a synchronous call.

Arguments mapping described in
[UpdateDomainRequestRequestTypeDef](./type_defs.md#updatedomainrequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `DefaultUserSettings`:
  [UserSettingsTypeDef](./type_defs.md#usersettingstypedef)
- `DomainSettingsForUpdate`:
  [DomainSettingsForUpdateTypeDef](./type_defs.md#domainsettingsforupdatetypedef)

Returns a `Coroutine` for
[UpdateDomainResponseTypeDef](./type_defs.md#updatedomainresponsetypedef).

<a id="update_endpoint"></a>

### update_endpoint

Deploys the new `EndpointConfig` specified in the request, switches to using
newly created endpoint, and then deletes resources provisioned for the endpoint
using the previous `EndpointConfig` (there is no availability loss).

Type annotations for `aiobotocore.create_client("sagemaker").update_endpoint`
method.

Boto3 documentation:
[SageMaker.Client.update_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_endpoint)

Asynchronous method. Use `await update_endpoint(...)` for a synchronous call.

Arguments mapping described in
[UpdateEndpointInputRequestTypeDef](./type_defs.md#updateendpointinputrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str` *(required)*
- `EndpointConfigName`: `str` *(required)*
- `RetainAllVariantProperties`: `bool`
- `ExcludeRetainedVariantProperties`:
  `Sequence`\[[VariantPropertyTypeDef](./type_defs.md#variantpropertytypedef)\]
- `DeploymentConfig`:
  [DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef)
- `RetainDeploymentConfig`: `bool`

Returns a `Coroutine` for
[UpdateEndpointOutputTypeDef](./type_defs.md#updateendpointoutputtypedef).

<a id="update_endpoint_weights_and_capacities"></a>

### update_endpoint_weights_and_capacities

Updates variant weight of one or more variants associated with an existing
endpoint, or capacity of one variant associated with an existing endpoint.

Type annotations for
`aiobotocore.create_client("sagemaker").update_endpoint_weights_and_capacities`
method.

Boto3 documentation:
[SageMaker.Client.update_endpoint_weights_and_capacities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_endpoint_weights_and_capacities)

Asynchronous method. Use `await update_endpoint_weights_and_capacities(...)`
for a synchronous call.

Arguments mapping described in
[UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef](./type_defs.md#updateendpointweightsandcapacitiesinputrequesttypedef).

Keyword-only arguments:

- `EndpointName`: `str` *(required)*
- `DesiredWeightsAndCapacities`:
  `Sequence`\[[DesiredWeightAndCapacityTypeDef](./type_defs.md#desiredweightandcapacitytypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateEndpointWeightsAndCapacitiesOutputTypeDef](./type_defs.md#updateendpointweightsandcapacitiesoutputtypedef).

<a id="update_experiment"></a>

### update_experiment

Adds, updates, or removes the description of an experiment.

Type annotations for `aiobotocore.create_client("sagemaker").update_experiment`
method.

Boto3 documentation:
[SageMaker.Client.update_experiment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_experiment)

Asynchronous method. Use `await update_experiment(...)` for a synchronous call.

Arguments mapping described in
[UpdateExperimentRequestRequestTypeDef](./type_defs.md#updateexperimentrequestrequesttypedef).

Keyword-only arguments:

- `ExperimentName`: `str` *(required)*
- `DisplayName`: `str`
- `Description`: `str`

Returns a `Coroutine` for
[UpdateExperimentResponseTypeDef](./type_defs.md#updateexperimentresponsetypedef).

<a id="update_image"></a>

### update_image

Updates the properties of a SageMaker image.

Type annotations for `aiobotocore.create_client("sagemaker").update_image`
method.

Boto3 documentation:
[SageMaker.Client.update_image](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_image)

Asynchronous method. Use `await update_image(...)` for a synchronous call.

Arguments mapping described in
[UpdateImageRequestRequestTypeDef](./type_defs.md#updateimagerequestrequesttypedef).

Keyword-only arguments:

- `ImageName`: `str` *(required)*
- `DeleteProperties`: `Sequence`\[`str`\]
- `Description`: `str`
- `DisplayName`: `str`
- `RoleArn`: `str`

Returns a `Coroutine` for
[UpdateImageResponseTypeDef](./type_defs.md#updateimageresponsetypedef).

<a id="update_model_package"></a>

### update_model_package

Updates a versioned model.

Type annotations for
`aiobotocore.create_client("sagemaker").update_model_package` method.

Boto3 documentation:
[SageMaker.Client.update_model_package](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_model_package)

Asynchronous method. Use `await update_model_package(...)` for a synchronous
call.

Arguments mapping described in
[UpdateModelPackageInputRequestTypeDef](./type_defs.md#updatemodelpackageinputrequesttypedef).

Keyword-only arguments:

- `ModelPackageArn`: `str` *(required)*
- `ModelApprovalStatus`:
  [ModelApprovalStatusType](./literals.md#modelapprovalstatustype)
- `ApprovalDescription`: `str`
- `CustomerMetadataProperties`: `Mapping`\[`str`, `str`\]
- `CustomerMetadataPropertiesToRemove`: `Sequence`\[`str`\]
- `AdditionalInferenceSpecificationsToAdd`:
  `Sequence`\[[AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef)\]

Returns a `Coroutine` for
[UpdateModelPackageOutputTypeDef](./type_defs.md#updatemodelpackageoutputtypedef).

<a id="update_monitoring_schedule"></a>

### update_monitoring_schedule

Updates a previously created schedule.

Type annotations for
`aiobotocore.create_client("sagemaker").update_monitoring_schedule` method.

Boto3 documentation:
[SageMaker.Client.update_monitoring_schedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_schedule)

Asynchronous method. Use `await update_monitoring_schedule(...)` for a
synchronous call.

Arguments mapping described in
[UpdateMonitoringScheduleRequestRequestTypeDef](./type_defs.md#updatemonitoringschedulerequestrequesttypedef).

Keyword-only arguments:

- `MonitoringScheduleName`: `str` *(required)*
- `MonitoringScheduleConfig`:
  [MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateMonitoringScheduleResponseTypeDef](./type_defs.md#updatemonitoringscheduleresponsetypedef).

<a id="update_notebook_instance"></a>

### update_notebook_instance

Updates a notebook instance.

Type annotations for
`aiobotocore.create_client("sagemaker").update_notebook_instance` method.

Boto3 documentation:
[SageMaker.Client.update_notebook_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_notebook_instance)

Asynchronous method. Use `await update_notebook_instance(...)` for a
synchronous call.

Arguments mapping described in
[UpdateNotebookInstanceInputRequestTypeDef](./type_defs.md#updatenotebookinstanceinputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceName`: `str` *(required)*
- `InstanceType`: [InstanceTypeType](./literals.md#instancetypetype)
- `RoleArn`: `str`
- `LifecycleConfigName`: `str`
- `DisassociateLifecycleConfig`: `bool`
- `VolumeSizeInGB`: `int`
- `DefaultCodeRepository`: `str`
- `AdditionalCodeRepositories`: `Sequence`\[`str`\]
- `AcceleratorTypes`:
  `Sequence`\[[NotebookInstanceAcceleratorTypeType](./literals.md#notebookinstanceacceleratortypetype)\]
- `DisassociateAcceleratorTypes`: `bool`
- `DisassociateDefaultCodeRepository`: `bool`
- `DisassociateAdditionalCodeRepositories`: `bool`
- `RootAccess`: [RootAccessType](./literals.md#rootaccesstype)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_notebook_instance_lifecycle_config"></a>

### update_notebook_instance_lifecycle_config

Updates a notebook instance lifecycle configuration created with the
CreateNotebookInstanceLifecycleConfig API.

Type annotations for
`aiobotocore.create_client("sagemaker").update_notebook_instance_lifecycle_config`
method.

Boto3 documentation:
[SageMaker.Client.update_notebook_instance_lifecycle_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_notebook_instance_lifecycle_config)

Asynchronous method. Use `await update_notebook_instance_lifecycle_config(...)`
for a synchronous call.

Arguments mapping described in
[UpdateNotebookInstanceLifecycleConfigInputRequestTypeDef](./type_defs.md#updatenotebookinstancelifecycleconfiginputrequesttypedef).

Keyword-only arguments:

- `NotebookInstanceLifecycleConfigName`: `str` *(required)*
- `OnCreate`:
  `Sequence`\[[NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef)\]
- `OnStart`:
  `Sequence`\[[NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_pipeline"></a>

### update_pipeline

Updates a pipeline.

Type annotations for `aiobotocore.create_client("sagemaker").update_pipeline`
method.

Boto3 documentation:
[SageMaker.Client.update_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_pipeline)

Asynchronous method. Use `await update_pipeline(...)` for a synchronous call.

Arguments mapping described in
[UpdatePipelineRequestRequestTypeDef](./type_defs.md#updatepipelinerequestrequesttypedef).

Keyword-only arguments:

- `PipelineName`: `str` *(required)*
- `PipelineDisplayName`: `str`
- `PipelineDefinition`: `str`
- `PipelineDescription`: `str`
- `RoleArn`: `str`

Returns a `Coroutine` for
[UpdatePipelineResponseTypeDef](./type_defs.md#updatepipelineresponsetypedef).

<a id="update_pipeline_execution"></a>

### update_pipeline_execution

Updates a pipeline execution.

Type annotations for
`aiobotocore.create_client("sagemaker").update_pipeline_execution` method.

Boto3 documentation:
[SageMaker.Client.update_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_pipeline_execution)

Asynchronous method. Use `await update_pipeline_execution(...)` for a
synchronous call.

Arguments mapping described in
[UpdatePipelineExecutionRequestRequestTypeDef](./type_defs.md#updatepipelineexecutionrequestrequesttypedef).

Keyword-only arguments:

- `PipelineExecutionArn`: `str` *(required)*
- `PipelineExecutionDescription`: `str`
- `PipelineExecutionDisplayName`: `str`

Returns a `Coroutine` for
[UpdatePipelineExecutionResponseTypeDef](./type_defs.md#updatepipelineexecutionresponsetypedef).

<a id="update_project"></a>

### update_project

Updates a machine learning (ML) project that is created from a template that
sets up an ML pipeline from training to deploying an approved model.

Type annotations for `aiobotocore.create_client("sagemaker").update_project`
method.

Boto3 documentation:
[SageMaker.Client.update_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_project)

Asynchronous method. Use `await update_project(...)` for a synchronous call.

Arguments mapping described in
[UpdateProjectInputRequestTypeDef](./type_defs.md#updateprojectinputrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ProjectDescription`: `str`
- `ServiceCatalogProvisioningUpdateDetails`:
  [ServiceCatalogProvisioningUpdateDetailsTypeDef](./type_defs.md#servicecatalogprovisioningupdatedetailstypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[UpdateProjectOutputTypeDef](./type_defs.md#updateprojectoutputtypedef).

<a id="update_training_job"></a>

### update_training_job

Update a model training job to request a new Debugger profiling configuration.

Type annotations for
`aiobotocore.create_client("sagemaker").update_training_job` method.

Boto3 documentation:
[SageMaker.Client.update_training_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_training_job)

Asynchronous method. Use `await update_training_job(...)` for a synchronous
call.

Arguments mapping described in
[UpdateTrainingJobRequestRequestTypeDef](./type_defs.md#updatetrainingjobrequestrequesttypedef).

Keyword-only arguments:

- `TrainingJobName`: `str` *(required)*
- `ProfilerConfig`:
  [ProfilerConfigForUpdateTypeDef](./type_defs.md#profilerconfigforupdatetypedef)
- `ProfilerRuleConfigurations`:
  `Sequence`\[[ProfilerRuleConfigurationTypeDef](./type_defs.md#profilerruleconfigurationtypedef)\]

Returns a `Coroutine` for
[UpdateTrainingJobResponseTypeDef](./type_defs.md#updatetrainingjobresponsetypedef).

<a id="update_trial"></a>

### update_trial

Updates the display name of a trial.

Type annotations for `aiobotocore.create_client("sagemaker").update_trial`
method.

Boto3 documentation:
[SageMaker.Client.update_trial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial)

Asynchronous method. Use `await update_trial(...)` for a synchronous call.

Arguments mapping described in
[UpdateTrialRequestRequestTypeDef](./type_defs.md#updatetrialrequestrequesttypedef).

Keyword-only arguments:

- `TrialName`: `str` *(required)*
- `DisplayName`: `str`

Returns a `Coroutine` for
[UpdateTrialResponseTypeDef](./type_defs.md#updatetrialresponsetypedef).

<a id="update_trial_component"></a>

### update_trial_component

Updates one or more properties of a trial component.

Type annotations for
`aiobotocore.create_client("sagemaker").update_trial_component` method.

Boto3 documentation:
[SageMaker.Client.update_trial_component](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial_component)

Asynchronous method. Use `await update_trial_component(...)` for a synchronous
call.

Arguments mapping described in
[UpdateTrialComponentRequestRequestTypeDef](./type_defs.md#updatetrialcomponentrequestrequesttypedef).

Keyword-only arguments:

- `TrialComponentName`: `str` *(required)*
- `DisplayName`: `str`
- `Status`:
  [TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef)
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `Parameters`: `Mapping`\[`str`,
  [TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef)\]
- `ParametersToRemove`: `Sequence`\[`str`\]
- `InputArtifacts`: `Mapping`\[`str`,
  [TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef)\]
- `InputArtifactsToRemove`: `Sequence`\[`str`\]
- `OutputArtifacts`: `Mapping`\[`str`,
  [TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef)\]
- `OutputArtifactsToRemove`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[UpdateTrialComponentResponseTypeDef](./type_defs.md#updatetrialcomponentresponsetypedef).

<a id="update_user_profile"></a>

### update_user_profile

Updates a user profile.

Type annotations for
`aiobotocore.create_client("sagemaker").update_user_profile` method.

Boto3 documentation:
[SageMaker.Client.update_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_user_profile)

Asynchronous method. Use `await update_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[UpdateUserProfileRequestRequestTypeDef](./type_defs.md#updateuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `DomainId`: `str` *(required)*
- `UserProfileName`: `str` *(required)*
- `UserSettings`: [UserSettingsTypeDef](./type_defs.md#usersettingstypedef)

Returns a `Coroutine` for
[UpdateUserProfileResponseTypeDef](./type_defs.md#updateuserprofileresponsetypedef).

<a id="update_workforce"></a>

### update_workforce

Use this operation to update your workforce.

Type annotations for `aiobotocore.create_client("sagemaker").update_workforce`
method.

Boto3 documentation:
[SageMaker.Client.update_workforce](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workforce)

Asynchronous method. Use `await update_workforce(...)` for a synchronous call.

Arguments mapping described in
[UpdateWorkforceRequestRequestTypeDef](./type_defs.md#updateworkforcerequestrequesttypedef).

Keyword-only arguments:

- `WorkforceName`: `str` *(required)*
- `SourceIpConfig`:
  [SourceIpConfigTypeDef](./type_defs.md#sourceipconfigtypedef)
- `OidcConfig`: [OidcConfigTypeDef](./type_defs.md#oidcconfigtypedef)

Returns a `Coroutine` for
[UpdateWorkforceResponseTypeDef](./type_defs.md#updateworkforceresponsetypedef).

<a id="update_workteam"></a>

### update_workteam

Updates an existing work team with new member definitions or description.

Type annotations for `aiobotocore.create_client("sagemaker").update_workteam`
method.

Boto3 documentation:
[SageMaker.Client.update_workteam](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workteam)

Asynchronous method. Use `await update_workteam(...)` for a synchronous call.

Arguments mapping described in
[UpdateWorkteamRequestRequestTypeDef](./type_defs.md#updateworkteamrequestrequesttypedef).

Keyword-only arguments:

- `WorkteamName`: `str` *(required)*
- `MemberDefinitions`:
  `Sequence`\[[MemberDefinitionTypeDef](./type_defs.md#memberdefinitiontypedef)\]
- `Description`: `str`
- `NotificationConfiguration`:
  [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)

Returns a `Coroutine` for
[UpdateWorkteamResponseTypeDef](./type_defs.md#updateworkteamresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("sagemaker").get_paginator`
method with overloads.

- `client.get_paginator("list_actions")` ->
  [ListActionsPaginator](./paginators.md#listactionspaginator)
- `client.get_paginator("list_algorithms")` ->
  [ListAlgorithmsPaginator](./paginators.md#listalgorithmspaginator)
- `client.get_paginator("list_app_image_configs")` ->
  [ListAppImageConfigsPaginator](./paginators.md#listappimageconfigspaginator)
- `client.get_paginator("list_apps")` ->
  [ListAppsPaginator](./paginators.md#listappspaginator)
- `client.get_paginator("list_artifacts")` ->
  [ListArtifactsPaginator](./paginators.md#listartifactspaginator)
- `client.get_paginator("list_associations")` ->
  [ListAssociationsPaginator](./paginators.md#listassociationspaginator)
- `client.get_paginator("list_auto_ml_jobs")` ->
  [ListAutoMLJobsPaginator](./paginators.md#listautomljobspaginator)
- `client.get_paginator("list_candidates_for_auto_ml_job")` ->
  [ListCandidatesForAutoMLJobPaginator](./paginators.md#listcandidatesforautomljobpaginator)
- `client.get_paginator("list_code_repositories")` ->
  [ListCodeRepositoriesPaginator](./paginators.md#listcoderepositoriespaginator)
- `client.get_paginator("list_compilation_jobs")` ->
  [ListCompilationJobsPaginator](./paginators.md#listcompilationjobspaginator)
- `client.get_paginator("list_contexts")` ->
  [ListContextsPaginator](./paginators.md#listcontextspaginator)
- `client.get_paginator("list_data_quality_job_definitions")` ->
  [ListDataQualityJobDefinitionsPaginator](./paginators.md#listdataqualityjobdefinitionspaginator)
- `client.get_paginator("list_device_fleets")` ->
  [ListDeviceFleetsPaginator](./paginators.md#listdevicefleetspaginator)
- `client.get_paginator("list_devices")` ->
  [ListDevicesPaginator](./paginators.md#listdevicespaginator)
- `client.get_paginator("list_domains")` ->
  [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- `client.get_paginator("list_edge_packaging_jobs")` ->
  [ListEdgePackagingJobsPaginator](./paginators.md#listedgepackagingjobspaginator)
- `client.get_paginator("list_endpoint_configs")` ->
  [ListEndpointConfigsPaginator](./paginators.md#listendpointconfigspaginator)
- `client.get_paginator("list_endpoints")` ->
  [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- `client.get_paginator("list_experiments")` ->
  [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
- `client.get_paginator("list_feature_groups")` ->
  [ListFeatureGroupsPaginator](./paginators.md#listfeaturegroupspaginator)
- `client.get_paginator("list_flow_definitions")` ->
  [ListFlowDefinitionsPaginator](./paginators.md#listflowdefinitionspaginator)
- `client.get_paginator("list_human_task_uis")` ->
  [ListHumanTaskUisPaginator](./paginators.md#listhumantaskuispaginator)
- `client.get_paginator("list_hyper_parameter_tuning_jobs")` ->
  [ListHyperParameterTuningJobsPaginator](./paginators.md#listhyperparametertuningjobspaginator)
- `client.get_paginator("list_image_versions")` ->
  [ListImageVersionsPaginator](./paginators.md#listimageversionspaginator)
- `client.get_paginator("list_images")` ->
  [ListImagesPaginator](./paginators.md#listimagespaginator)
- `client.get_paginator("list_inference_recommendations_jobs")` ->
  [ListInferenceRecommendationsJobsPaginator](./paginators.md#listinferencerecommendationsjobspaginator)
- `client.get_paginator("list_labeling_jobs")` ->
  [ListLabelingJobsPaginator](./paginators.md#listlabelingjobspaginator)
- `client.get_paginator("list_labeling_jobs_for_workteam")` ->
  [ListLabelingJobsForWorkteamPaginator](./paginators.md#listlabelingjobsforworkteampaginator)
- `client.get_paginator("list_lineage_groups")` ->
  [ListLineageGroupsPaginator](./paginators.md#listlineagegroupspaginator)
- `client.get_paginator("list_model_bias_job_definitions")` ->
  [ListModelBiasJobDefinitionsPaginator](./paginators.md#listmodelbiasjobdefinitionspaginator)
- `client.get_paginator("list_model_explainability_job_definitions")` ->
  [ListModelExplainabilityJobDefinitionsPaginator](./paginators.md#listmodelexplainabilityjobdefinitionspaginator)
- `client.get_paginator("list_model_metadata")` ->
  [ListModelMetadataPaginator](./paginators.md#listmodelmetadatapaginator)
- `client.get_paginator("list_model_package_groups")` ->
  [ListModelPackageGroupsPaginator](./paginators.md#listmodelpackagegroupspaginator)
- `client.get_paginator("list_model_packages")` ->
  [ListModelPackagesPaginator](./paginators.md#listmodelpackagespaginator)
- `client.get_paginator("list_model_quality_job_definitions")` ->
  [ListModelQualityJobDefinitionsPaginator](./paginators.md#listmodelqualityjobdefinitionspaginator)
- `client.get_paginator("list_models")` ->
  [ListModelsPaginator](./paginators.md#listmodelspaginator)
- `client.get_paginator("list_monitoring_executions")` ->
  [ListMonitoringExecutionsPaginator](./paginators.md#listmonitoringexecutionspaginator)
- `client.get_paginator("list_monitoring_schedules")` ->
  [ListMonitoringSchedulesPaginator](./paginators.md#listmonitoringschedulespaginator)
- `client.get_paginator("list_notebook_instance_lifecycle_configs")` ->
  [ListNotebookInstanceLifecycleConfigsPaginator](./paginators.md#listnotebookinstancelifecycleconfigspaginator)
- `client.get_paginator("list_notebook_instances")` ->
  [ListNotebookInstancesPaginator](./paginators.md#listnotebookinstancespaginator)
- `client.get_paginator("list_pipeline_execution_steps")` ->
  [ListPipelineExecutionStepsPaginator](./paginators.md#listpipelineexecutionstepspaginator)
- `client.get_paginator("list_pipeline_executions")` ->
  [ListPipelineExecutionsPaginator](./paginators.md#listpipelineexecutionspaginator)
- `client.get_paginator("list_pipeline_parameters_for_execution")` ->
  [ListPipelineParametersForExecutionPaginator](./paginators.md#listpipelineparametersforexecutionpaginator)
- `client.get_paginator("list_pipelines")` ->
  [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- `client.get_paginator("list_processing_jobs")` ->
  [ListProcessingJobsPaginator](./paginators.md#listprocessingjobspaginator)
- `client.get_paginator("list_studio_lifecycle_configs")` ->
  [ListStudioLifecycleConfigsPaginator](./paginators.md#liststudiolifecycleconfigspaginator)
- `client.get_paginator("list_subscribed_workteams")` ->
  [ListSubscribedWorkteamsPaginator](./paginators.md#listsubscribedworkteamspaginator)
- `client.get_paginator("list_tags")` ->
  [ListTagsPaginator](./paginators.md#listtagspaginator)
- `client.get_paginator("list_training_jobs")` ->
  [ListTrainingJobsPaginator](./paginators.md#listtrainingjobspaginator)
- `client.get_paginator("list_training_jobs_for_hyper_parameter_tuning_job")`
  ->
  [ListTrainingJobsForHyperParameterTuningJobPaginator](./paginators.md#listtrainingjobsforhyperparametertuningjobpaginator)
- `client.get_paginator("list_transform_jobs")` ->
  [ListTransformJobsPaginator](./paginators.md#listtransformjobspaginator)
- `client.get_paginator("list_trial_components")` ->
  [ListTrialComponentsPaginator](./paginators.md#listtrialcomponentspaginator)
- `client.get_paginator("list_trials")` ->
  [ListTrialsPaginator](./paginators.md#listtrialspaginator)
- `client.get_paginator("list_user_profiles")` ->
  [ListUserProfilesPaginator](./paginators.md#listuserprofilespaginator)
- `client.get_paginator("list_workforces")` ->
  [ListWorkforcesPaginator](./paginators.md#listworkforcespaginator)
- `client.get_paginator("list_workteams")` ->
  [ListWorkteamsPaginator](./paginators.md#listworkteamspaginator)
- `client.get_paginator("search")` ->
  [SearchPaginator](./paginators.md#searchpaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `aiobotocore.create_client("sagemaker").get_waiter` method
with overloads.

- `client.get_waiter("endpoint_deleted")` ->
  [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)
- `client.get_waiter("endpoint_in_service")` ->
  [EndpointInServiceWaiter](./waiters.md#endpointinservicewaiter)
- `client.get_waiter("image_created")` ->
  [ImageCreatedWaiter](./waiters.md#imagecreatedwaiter)
- `client.get_waiter("image_deleted")` ->
  [ImageDeletedWaiter](./waiters.md#imagedeletedwaiter)
- `client.get_waiter("image_updated")` ->
  [ImageUpdatedWaiter](./waiters.md#imageupdatedwaiter)
- `client.get_waiter("image_version_created")` ->
  [ImageVersionCreatedWaiter](./waiters.md#imageversioncreatedwaiter)
- `client.get_waiter("image_version_deleted")` ->
  [ImageVersionDeletedWaiter](./waiters.md#imageversiondeletedwaiter)
- `client.get_waiter("notebook_instance_deleted")` ->
  [NotebookInstanceDeletedWaiter](./waiters.md#notebookinstancedeletedwaiter)
- `client.get_waiter("notebook_instance_in_service")` ->
  [NotebookInstanceInServiceWaiter](./waiters.md#notebookinstanceinservicewaiter)
- `client.get_waiter("notebook_instance_stopped")` ->
  [NotebookInstanceStoppedWaiter](./waiters.md#notebookinstancestoppedwaiter)
- `client.get_waiter("processing_job_completed_or_stopped")` ->
  [ProcessingJobCompletedOrStoppedWaiter](./waiters.md#processingjobcompletedorstoppedwaiter)
- `client.get_waiter("training_job_completed_or_stopped")` ->
  [TrainingJobCompletedOrStoppedWaiter](./waiters.md#trainingjobcompletedorstoppedwaiter)
- `client.get_waiter("transform_job_completed_or_stopped")` ->
  [TransformJobCompletedOrStoppedWaiter](./waiters.md#transformjobcompletedorstoppedwaiter)

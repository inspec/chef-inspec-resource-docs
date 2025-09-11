+++
title = "google_run_jobs resource"
platform = "gcp"
draft = false
gh_repo = "inspec-gcp"


[menu.gcp]
title = "google_run_jobs"
identifier = "inspec/resources/gcp/google_run_jobs resource"
parent = "inspec/resources/gcp"
+++

Use the `google_run_jobs` InSpec audit resource to test the properties of a Google Cloud Job resource.

## Examples

```ruby
  describe google_run_jobs(parent: 'projects/{project}/locations/{location}') do
    it { should exist }
    its('names') { should include 'value_name' }
    its('creators') { should include 'value_creator' }
  end
```

## Parameters

Parameters that can be accessed from the `google_run_jobs` resource:

See [google_run_job](google_run_job) for more detailed information.

* `names`: an array of `google_run_job` name
* `uids`: an array of `google_run_job` uid
* `generations`: an array of `google_run_job` generation
* `labels`: an array of `google_run_job` labels
* `annotations`: an array of `google_run_job` annotations
* `create_times`: an array of `google_run_job` create_time
* `update_times`: an array of `google_run_job` update_time
* `delete_times`: an array of `google_run_job` delete_time
* `expire_times`: an array of `google_run_job` expire_time
* `creators`: an array of `google_run_job` creator
* `last_modifiers`: an array of `google_run_job` last_modifier
* `clients`: an array of `google_run_job` client
* `client_versions`: an array of `google_run_job` client_version
* `launch_stages`: an array of `google_run_job` launch_stage
* `binary_authorizations`: an array of `google_run_job` binary_authorization
* `templates`: an array of `google_run_job` template
* `observed_generations`: an array of `google_run_job` observed_generation
* `terminal_conditions`: an array of `google_run_job` terminal_condition
* `conditions`: an array of `google_run_job` conditions
* `execution_counts`: an array of `google_run_job` execution_count
* `latest_created_executions`: an array of `google_run_job` latest_created_execution
* `reconcilings`: an array of `google_run_job` reconciling
* `satisfies_pzs`: an array of `google_run_job` satisfies_pzs
* `start_execution_tokens`: an array of `google_run_job` start_execution_token
* `run_execution_tokens`: an array of `google_run_job` run_execution_token
* `etags`: an array of `google_run_job` etag

## Properties

Properties that can be accessed from the `google_run_jobs` resource:

See [google_run_job](google_run_job) for more detailed information.

* `names`: an array of `google_run_job` name
* `uids`: an array of `google_run_job` uid
* `generations`: an array of `google_run_job` generation
* `labels`: an array of `google_run_job` labels
* `annotations`: an array of `google_run_job` annotations
* `create_times`: an array of `google_run_job` create_time
* `update_times`: an array of `google_run_job` update_time
* `delete_times`: an array of `google_run_job` delete_time
* `expire_times`: an array of `google_run_job` expire_time
* `creators`: an array of `google_run_job` creator
* `last_modifiers`: an array of `google_run_job` last_modifier
* `clients`: an array of `google_run_job` client
* `client_versions`: an array of `google_run_job` client_version
* `launch_stages`: an array of `google_run_job` launch_stage
* `binary_authorizations`: an array of `google_run_job` binary_authorization
* `templates`: an array of `google_run_job` template
* `observed_generations`: an array of `google_run_job` observed_generation
* `terminal_conditions`: an array of `google_run_job` terminal_condition
* `conditions`: an array of `google_run_job` conditions
* `execution_counts`: an array of `google_run_job` execution_count
* `latest_created_executions`: an array of `google_run_job` latest_created_execution
* `reconcilings`: an array of `google_run_job` reconciling
* `satisfies_pzs`: an array of `google_run_job` satisfies_pzs
* `start_execution_tokens`: an array of `google_run_job` start_execution_token
* `run_execution_tokens`: an array of `google_run_job` run_execution_token
* `etags`: an array of `google_run_job` etag

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [https://run.googleapis.com/](https://console.cloud.google.com/apis/library/run.googleapis.com/) is enabled for the current project.

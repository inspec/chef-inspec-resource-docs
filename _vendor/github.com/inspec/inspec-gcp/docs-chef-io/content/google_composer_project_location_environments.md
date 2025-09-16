+++
title = "google_composer_project_location_environments resource"

draft = false


[menu.gcp]
title = "google_composer_project_location_environments"
identifier = "inspec/resources/gcp/google_composer_project_location_environments resource"
parent = "inspec/resources/gcp"
+++

Use the `google_composer_project_location_environments` InSpec audit resource to to test a Google Cloud ProjectLocationEnvironment resource.

## Examples

```ruby
    describe google_composer_project_location_environments(parent: ' value_parent') do
    it { should exist }
    its('name') { should include('value_name') }
    its('uuid') { should include('value_uuid') }
    its('state') { should include('value_state') }
    its('create_time') { should include('value_createtime') }
    its('update_time') { should include('value_updatetime') }
    its('satisfies_pzs') { should include('value_satisfies_pzs') }
  end
```

## Properties

Properties that can be accessed from the `google_composer_project_location_environments` resource:

See [google_composer_project_location_environment](google_composer_project_location_environment) for more detailed information.

  * `names`: an array of `google_composer_project_location_environment` name
  * `configs`: an array of `google_composer_project_location_environment` config
  * `uuids`: an array of `google_composer_project_location_environment` uuid
  * `states`: an array of `google_composer_project_location_environment` state
  * `create_times`: an array of `google_composer_project_location_environment` create_time
  * `update_times`: an array of `google_composer_project_location_environment` update_time
  * `labels`: an array of `google_composer_project_location_environment` labels
  * `satisfies_pzs`: an array of `google_composer_project_location_environment` satisfies_pzs
  * `storage_configs`: an array of `google_composer_project_location_environment` storage_config

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [https://composer.googleapis.com/](https://console.cloud.google.com/apis/library/composer.googleapis.com/) is enabled for the current project.

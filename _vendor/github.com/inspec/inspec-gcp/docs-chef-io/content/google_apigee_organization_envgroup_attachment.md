+++
title = "google_apigee_organization_envgroup_attachment resource"
platform = "gcp"
draft = false
gh_repo = "inspec-gcp"

[menu.gcp]
title = "google_apigee_organization_envgroup_attachment"
identifier = "inspec/resources/gcp/google_apigee_organization_envgroup_attachment resource"
parent = "inspec/resources/gcp"
+++

Use the `google_apigee_organization_envgroup_attachment` InSpec audit resource to to test a Google Cloud OrganizationEnvgroupAttachment resource.

## Examples

```
describe google_apigee_organization_envgroup_attachment(name: ' value_name') do
	it { should exist }
	its('created_at') { should cmp 'value_createdat' }
	its('environment') { should cmp 'value_environment' }
	its('environment_group_id') { should cmp 'value_environmentgroupid' }
	its('name') { should cmp 'value_name' }

end

describe google_apigee_organization_envgroup_attachment(name: "does_not_exit") do
	it { should_not exist }
end
```

## Properties

Properties that can be accessed from the `google_apigee_organization_envgroup_attachment` resource:


  * `created_at`: The time at which the environment group attachment was created as milliseconds since epoch.

  * `environment`: ID of the attached environment.

  * `environment_group_id`: ID of the environment group.

  * `name`: ID of the environment group attachment.


## GCP permissions

Ensure the [Apigee API](https://console.cloud.google.com/apis/library/apigee.googleapis.com/) is enabled for the current project.

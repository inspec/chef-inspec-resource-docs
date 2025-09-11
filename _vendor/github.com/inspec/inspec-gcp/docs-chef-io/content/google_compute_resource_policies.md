+++
title = "google_compute_resource_policies resource"
platform = "gcp"
draft = false
gh_repo = "inspec-gcp"

[menu.gcp]
title = "google_compute_resource_policies"
identifier = "inspec/resources/gcp/google_compute_resource_policies resource"
parent = "inspec/resources/gcp"
+++

Use the `google_compute_resource_policies` InSpec audit resource to to test a Google Cloud ResourcePolicy resource.

## Examples

```ruby
  describe google_compute_resource_policies(project: 'chef-gcp-inspec', region: ' value_region') do
    it { should exist }
  end
```

## Properties

Properties that can be accessed from the `google_compute_resource_policies` resource:

See [google_compute_resource_policy](google_compute_resource_policy) for more detailed information.

  * `kinds`: an array of `google_compute_resource_policy` kind
  * `ids`: an array of `google_compute_resource_policy` id
  * `creation_timestamps`: an array of `google_compute_resource_policy` creation_timestamp
  * `self_links`: an array of `google_compute_resource_policy` self_link
  * `self_link_with_ids`: an array of `google_compute_resource_policy` self_link_with_id
  * `regions`: an array of `google_compute_resource_policy` region
  * `descriptions`: an array of `google_compute_resource_policy` description
  * `names`: an array of `google_compute_resource_policy` name
  * `vm_maintenance_policies`: an array of `google_compute_resource_policy` vm_maintenance_policy
  * `snapshot_schedule_policies`: an array of `google_compute_resource_policy` snapshot_schedule_policy
  * `group_placement_policies`: an array of `google_compute_resource_policy` group_placement_policy
  * `instance_schedule_policies`: an array of `google_compute_resource_policy` instance_schedule_policy
  * `statuses`: an array of `google_compute_resource_policy` status
  * `resource_statuses`: an array of `google_compute_resource_policy` resource_status

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [Compute Engine API](https://console.cloud.google.com/apis/library/compute.googleapis.com/) is enabled for the current project.

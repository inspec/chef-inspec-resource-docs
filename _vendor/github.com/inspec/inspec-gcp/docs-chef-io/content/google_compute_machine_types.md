+++
title = "google_compute_machine_types resource"

draft = false


[menu.gcp]
title = "google_compute_machine_types"
identifier = "inspec/resources/gcp/google_compute_machine_types resource"
parent = "inspec/resources/gcp"
+++

Use the `google_compute_machine_types` InSpec audit resource to to test a Google Cloud MachineType resource.

## Examples

```ruby
  describe google_compute_machine_types(project: 'chef-gcp-inspec', zone: ' value_zone') do
    it { should exist }
  end
```

## Properties

Properties that can be accessed from the `google_compute_machine_types` resource:

See [google_compute_machine_type](google_compute_machine_type) for more detailed information.

  * `kinds`: an array of `google_compute_machine_type` kind
  * `ids`: an array of `google_compute_machine_type` id
  * `creation_timestamps`: an array of `google_compute_machine_type` creation_timestamp
  * `names`: an array of `google_compute_machine_type` name
  * `descriptions`: an array of `google_compute_machine_type` description
  * `guest_cpus`: an array of `google_compute_machine_type` guest_cpus
  * `memory_mbs`: an array of `google_compute_machine_type` memory_mb
  * `image_space_gbs`: an array of `google_compute_machine_type` image_space_gb
  * `scratch_disks`: an array of `google_compute_machine_type` scratch_disks
  * `maximum_persistent_disks`: an array of `google_compute_machine_type` maximum_persistent_disks
  * `maximum_persistent_disks_size_gbs`: an array of `google_compute_machine_type` maximum_persistent_disks_size_gb
  * `deprecateds`: an array of `google_compute_machine_type` deprecated
  * `zones`: an array of `google_compute_machine_type` zone
  * `self_links`: an array of `google_compute_machine_type` self_link
  * `is_shared_cpus`: an array of `google_compute_machine_type` is_shared_cpu
  * `accelerators`: an array of `google_compute_machine_type` accelerators

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [Compute Engine API](https://console.cloud.google.com/apis/library/compute.googleapis.com/) is enabled for the current project.

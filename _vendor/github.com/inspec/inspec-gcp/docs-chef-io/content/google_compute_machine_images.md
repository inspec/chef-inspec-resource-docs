+++
title = "google_compute_machine_images resource"
platform = "gcp"
draft = false
gh_repo = "inspec-gcp"

[menu.gcp]
title = "google_compute_machine_images"
identifier = "inspec/resources/gcp/google_compute_machine_images resource"
parent = "inspec/resources/gcp"
+++

Use the `google_compute_machine_images` InSpec audit resource to to test a Google Cloud MachineImage resource.

## Examples

```ruby
  describe google_compute_machine_images(project: 'chef-gcp-inspec') do
    it { should exist }
  end
```

## Properties

Properties that can be accessed from the `google_compute_machine_images` resource:

See [google_compute_machine_image](google_compute_machine_image) for more detailed information.

  * `kinds`: an array of `google_compute_machine_image` kind
  * `ids`: an array of `google_compute_machine_image` id
  * `creation_timestamps`: an array of `google_compute_machine_image` creation_timestamp
  * `names`: an array of `google_compute_machine_image` name
  * `descriptions`: an array of `google_compute_machine_image` description
  * `self_links`: an array of `google_compute_machine_image` self_link
  * `source_instances`: an array of `google_compute_machine_image` source_instance
  * `statuses`: an array of `google_compute_machine_image` status
  * `source_instance_properties`: an array of `google_compute_machine_image` source_instance_properties
  * `instance_properties`: an array of `google_compute_machine_image` instance_properties
  * `saved_disks`: an array of `google_compute_machine_image` saved_disks
  * `storage_locations`: an array of `google_compute_machine_image` storage_locations
  * `machine_image_encryption_keys`: an array of `google_compute_machine_image` machine_image_encryption_key
  * `guest_flushes`: an array of `google_compute_machine_image` guest_flush
  * `source_disk_encryption_keys`: an array of `google_compute_machine_image` source_disk_encryption_keys
  * `total_storage_bytes`: an array of `google_compute_machine_image` total_storage_bytes
  * `satisfies_pzs`: an array of `google_compute_machine_image` satisfies_pzs

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [Compute Engine API](https://console.cloud.google.com/apis/library/compute.googleapis.com/) is enabled for the current project.

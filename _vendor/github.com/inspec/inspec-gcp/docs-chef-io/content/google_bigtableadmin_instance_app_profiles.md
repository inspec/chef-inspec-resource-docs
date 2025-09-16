+++
title = "google_bigtableadmin_instance_app_profiles resource"

draft = false



[menu.gcp]
title = "google_bigtableadmin_instance_app_profiles"
identifier = "inspec/resources/gcp/google_bigtableadmin_instance_app_profiles resource"
parent = "inspec/resources/gcp"
+++

Use the `google_bigtableadmin_instance_app_profiles` InSpec audit resource to test the properties of a Google Cloud InstanceAppProfile resource.

## Examples

```ruby
  describe google_bigtableadmin_instance_app_profiles(parent: ' value_parent') do
    it { should exist }
    its('names') { should include 'value_name' }
  end
```

## Parameters

Parameters that can be accessed from the `google_bigtableadmin_instance_app_profiles` resource:

See [google_bigtableadmin_instance_app_profile](google_bigtableadmin_instance_app_profile) for more detailed information.

* `names`: an array of `google_bigtableadmin_instance_app_profile` name
* `etags`: an array of `google_bigtableadmin_instance_app_profile` etag
* `descriptions`: an array of `google_bigtableadmin_instance_app_profile` description
* `multi_cluster_routing_use_anies`: an array of `google_bigtableadmin_instance_app_profile` multi_cluster_routing_use_any
* `single_cluster_routings`: an array of `google_bigtableadmin_instance_app_profile` single_cluster_routing
* `priorities`: an array of `google_bigtableadmin_instance_app_profile` priority
* `standard_isolations`: an array of `google_bigtableadmin_instance_app_profile` standard_isolation
* `data_boost_isolation_read_onlies`: an array of `google_bigtableadmin_instance_app_profile` data_boost_isolation_read_only

## Properties

Properties that can be accessed from the `google_bigtableadmin_instance_app_profiles` resource:

See [google_bigtableadmin_instance_app_profile](google_bigtableadmin_instance_app_profile) for more detailed information.

* `names`: an array of `google_bigtableadmin_instance_app_profile` name
* `etags`: an array of `google_bigtableadmin_instance_app_profile` etag
* `descriptions`: an array of `google_bigtableadmin_instance_app_profile` description
* `multi_cluster_routing_use_anies`: an array of `google_bigtableadmin_instance_app_profile` multi_cluster_routing_use_any
* `single_cluster_routings`: an array of `google_bigtableadmin_instance_app_profile` single_cluster_routing
* `priorities`: an array of `google_bigtableadmin_instance_app_profile` priority
* `standard_isolations`: an array of `google_bigtableadmin_instance_app_profile` standard_isolation
* `data_boost_isolation_read_onlies`: an array of `google_bigtableadmin_instance_app_profile` data_boost_isolation_read_only

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [https://bigtableadmin.googleapis.com/](https://console.cloud.google.com/apis/library/bigtableadmin.googleapis.com/) is enabled for the current project.

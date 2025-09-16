+++
title = "google_compute_network_firewall_policies resource"

draft = false


[menu.gcp]
title = "google_compute_network_firewall_policies"
identifier = "inspec/resources/gcp/google_compute_network_firewall_policies resource"
parent = "inspec/resources/gcp"
+++

Use the `google_compute_network_firewall_policies` InSpec audit resource to to test a Google Cloud NetworkFirewallPolicy resource.

## Examples

```ruby
    describe google_compute_network_firewall_policies(project: 'chef-gcp-inspec') do
    it { should exist }
  end
```

## Properties

Properties that can be accessed from the `google_compute_network_firewall_policies` resource:

See [google_compute_network_firewall_policy](google_compute_network_firewall_policy) for more detailed information.

  * `kinds`: an array of `google_compute_network_firewall_policy` kind
  * `ids`: an array of `google_compute_network_firewall_policy` id
  * `creation_timestamps`: an array of `google_compute_network_firewall_policy` creation_timestamp
  * `names`: an array of `google_compute_network_firewall_policy` name
  * `descriptions`: an array of `google_compute_network_firewall_policy` description
  * `rules`: an array of `google_compute_network_firewall_policy` rules
  * `fingerprints`: an array of `google_compute_network_firewall_policy` fingerprint
  * `self_links`: an array of `google_compute_network_firewall_policy` self_link
  * `self_link_with_ids`: an array of `google_compute_network_firewall_policy` self_link_with_id
  * `associations`: an array of `google_compute_network_firewall_policy` associations
  * `rule_tuple_counts`: an array of `google_compute_network_firewall_policy` rule_tuple_count
  * `short_names`: an array of `google_compute_network_firewall_policy` short_name
  * `display_names`: an array of `google_compute_network_firewall_policy` display_name
  * `parents`: an array of `google_compute_network_firewall_policy` parent
  * `regions`: an array of `google_compute_network_firewall_policy` region

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [Compute Engine API](https://console.cloud.google.com/apis/library/compute.googleapis.com/) is enabled for the current project.

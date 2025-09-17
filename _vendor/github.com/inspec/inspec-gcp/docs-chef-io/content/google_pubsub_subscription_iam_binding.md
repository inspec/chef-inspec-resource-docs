+++
title = "google_pubsub_subscription_iam_binding resource"

draft = false


[menu.gcp]
title = "google_pubsub_subscription_iam_binding"
identifier = "inspec/resources/gcp/google_pubsub_subscription_iam_binding resource"
parent = "inspec/resources/gcp"
+++

## Syntax

A `google_pubsub_subscription_iam_binding` is used to test a Google Subscription Iam Bindings

## Examples

```ruby
describe google_pubsub_subscription_iam_binding(project: "project", name: "name", role: "roles/editor") do
  it { should exist }
  its('members') { should include 'user:testuser@example.com' }
end
```


## Properties

Properties that can be accessed from the `google_pubsub_subscription_iam_binding` resource:

  * `role`: Role that is assigned to members. For example, roles/viewer, roles/editor, or roles/owner.

  * `members`: Specifies the identities requesting access for a Cloud Platform resource.


## GCP permissions

Ensure the [Cloud Pub/Sub API](https://console.cloud.google.com/apis/library/pubsub.googleapis.com/) is enabled for the current project.

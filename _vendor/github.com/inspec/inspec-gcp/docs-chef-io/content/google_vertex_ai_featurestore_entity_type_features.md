+++
title = "google_vertex_ai_featurestore_entity_type_features resource"
platform = "gcp"
draft = false
gh_repo = "inspec-gcp"

[menu.gcp]
title = "google_vertex_ai_featurestore_entity_type_features"
identifier = "inspec/resources/gcp/google_vertex_ai_featurestore_entity_type_features resource"
parent = "inspec/resources/gcp"
+++

Use the `google_vertex_ai_featurestore_entity_type_features` InSpec audit resource to to test a Google Cloud FeaturestoreEntityTypeFeature resource.

## Examples

```ruby
    describe google_vertex_ai_featurestore_entity_type_features(parent: "projects/#{gcp_project_id}/locations/#{featurestore_entity_type_feature['region']}/featurestores/#{featurestore_entity_type_feature['featurestore']}/entityTypes/#{featurestore_entity_type_feature['entityType']}", region: ' value_region') do
    it { should exist }
  end
```

## Properties

Properties that can be accessed from the `google_vertex_ai_featurestore_entity_type_features` resource:

See [google_vertex_ai_featurestore_entity_type_feature](google_vertex_ai_featurestore_entity_type_feature) for more detailed information.

  * `descriptions`: an array of `google_vertex_ai_featurestore_entity_type_feature` description
  * `create_times`: an array of `google_vertex_ai_featurestore_entity_type_feature` create_time
  * `monitoring_stats_anomalies`: an array of `google_vertex_ai_featurestore_entity_type_feature` monitoring_stats_anomalies
  * `etags`: an array of `google_vertex_ai_featurestore_entity_type_feature` etag
  * `labels`: an array of `google_vertex_ai_featurestore_entity_type_feature` labels
  * `names`: an array of `google_vertex_ai_featurestore_entity_type_feature` name
  * `update_times`: an array of `google_vertex_ai_featurestore_entity_type_feature` update_time
  * `disable_monitorings`: an array of `google_vertex_ai_featurestore_entity_type_feature` disable_monitoring
  * `value_types`: an array of `google_vertex_ai_featurestore_entity_type_feature` value_type

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

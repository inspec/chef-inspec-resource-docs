+++
title = "google_vertex_ai_metadata_stores_contexts resource"

draft = false


[menu.gcp]
title = "google_vertex_ai_metadata_stores_contexts"
identifier = "inspec/resources/gcp/google_vertex_ai_metadata_stores_contexts resource"
parent = "inspec/resources/gcp"
+++

Use the `google_vertex_ai_metadata_stores_contexts` InSpec audit resource to to test a Google Cloud MetadataStoresContext resource.

## Examples

```ruby
    describe google_vertex_ai_metadata_stores_contexts(parent: "projects/#{gcp_project_id}/locations/#{metadata_stores_context['region']}/metadataStores/#{metadata_stores_context['metadataStore']}", region: ' value_region') do
    it { should exist }
  end
```

## Properties

Properties that can be accessed from the `google_vertex_ai_metadata_stores_contexts` resource:

See [google_vertex_ai_metadata_stores_context](google_vertex_ai_metadata_stores_context) for more detailed information.

  * `names`: an array of `google_vertex_ai_metadata_stores_context` name
  * `schema_titles`: an array of `google_vertex_ai_metadata_stores_context` schema_title
  * `etags`: an array of `google_vertex_ai_metadata_stores_context` etag
  * `descriptions`: an array of `google_vertex_ai_metadata_stores_context` description
  * `display_names`: an array of `google_vertex_ai_metadata_stores_context` display_name
  * `schema_versions`: an array of `google_vertex_ai_metadata_stores_context` schema_version
  * `create_times`: an array of `google_vertex_ai_metadata_stores_context` create_time
  * `labels`: an array of `google_vertex_ai_metadata_stores_context` labels
  * `metadata`: an array of `google_vertex_ai_metadata_stores_context` metadata
  * `update_times`: an array of `google_vertex_ai_metadata_stores_context` update_time
  * `parent_contexts`: an array of `google_vertex_ai_metadata_stores_context` parent_contexts

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

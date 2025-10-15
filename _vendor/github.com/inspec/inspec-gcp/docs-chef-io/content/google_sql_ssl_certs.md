+++
title = "google_sql_ssl_certs resource"

draft = false


[menu.gcp]
title = "google_sql_ssl_certs"
identifier = "inspec/resources/gcp/google_sql_ssl_certs resource"
parent = "inspec/resources/gcp"
+++

Use the `google_sql_ssl_certs` InSpec audit resource to to test a Google Cloud SslCerts resource.

## Examples

```ruby
describe google_sql_ssl_certs(project: 'chef-gcp-inspec', instance: 'test-pg') do
  it { should exist }
  its('instances') { should include 'test-pg' }
  its('common_names') { should include 'C=US,O=Google\, Inc,CN=Google Cloud SQL Server CA,dnQualifier=68c79386-b63e-4998-8254-ba59729cdf78' }
  its('sha1_fingerprints') { should include '80c5c611c0a591db967c7dda3467e23127288fed' }
end

describe google_sql_ssl_certs(project: 'chef-gcp-inspec', instance: 'nonexistent') do
  it { should_not exist }
end
```

## Properties

Properties that can be accessed from the `google_sql_ssl_certs` resource:

See [google_sql_ssl_cert](google_sql_ssl_cert) for more detailed information.

  * `certs`: an array of `google_sql_ssl_cert` cert
  * `cert_serial_numbers`: an array of `google_sql_ssl_cert` cert_serial_number
  * `common_names`: an array of `google_sql_ssl_cert` common_name
  * `create_times`: an array of `google_sql_ssl_cert` create_time
  * `expiration_times`: an array of `google_sql_ssl_cert` expiration_time
  * `instances`: an array of `google_sql_ssl_cert` instance
  * `sha1_fingerprints`: an array of `google_sql_ssl_cert` sha1_fingerprint

## Filter criteria

This resource supports all of the above properties as filter criteria, which can be used
with `where` as a block or a method.

## GCP permissions

Ensure the [Cloud SQL Admin API](https://console.cloud.google.com/apis/library/sqladmin.googleapis.com/) is enabled for the current project.

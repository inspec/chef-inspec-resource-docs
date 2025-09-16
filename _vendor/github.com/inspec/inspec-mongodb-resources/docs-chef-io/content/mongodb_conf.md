+++
title = "mongodb_conf resource"
draft = false


[menu.mongodb]
    title = "mongodb_conf"
    identifier = "inspec/resources/mongodb/mongodb_conf.md mongodb_conf resource"
    parent = "inspec/resources/mongodb"
+++

Use the `mongodb_conf` Chef InSpec audit resource to test the contents of the configuration file for MongoDB, typically located at `/etc/mongod.conf` or `C:\Program Files\MongoDB\Server\<version>\bin\mongod.cfg`, depending on the platform.

## Syntax

A `mongodb_conf` resource block declares one (or more) settings in the `mongodb.conf` file, and then compares the setting in the configuration file to the value stated in the test:

```ruby
describe mongodb_conf('path') do
  its('setting') { should eq 'value' }
end
```

where

- `'setting'` specifies a setting in the `mongodb.conf` file
- `('path')` is the non-default path to the `mongodb.conf` file (optional)
- `should eq 'value'` is the value that is expected

## Examples

The following examples show how to use this Chef InSpec audit resource.

Test the key management configuration options:

```ruby
describe mongodb_conf do
  its(["security", "enableEncryption"]) { should eq true }
end
```

Test the port on which MongoDB listens:

```ruby
describe mongodb_conf do
  its(["net", "port"]) { should eq 27017 }
end
```

Test the security configuration options:

```ruby
describe mongodb_conf do
  its(["security", "authorization"]) { should eq "enabled" }
end
```

## Matchers

{{< readfile file="content/reusable/md/inspec_matchers_link.md" >}}

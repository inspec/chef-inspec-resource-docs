+++
title = "rabbitmq_config resource"
draft = false

[menu.rabbitmq]
    title = "rabbitmq_config"
    identifier = "inspec/resources/rabbitmq/rabbitmq_config.md rabbitmq_config resource"
    parent = "inspec/resources/rabbitmq"
+++

Use the `rabbitmq_config` Chef InSpec audit resource to test configuration data for the RabbitMQ daemon located at `/etc/rabbitmq/rabbitmq.config` on Linux and Unix platforms.

## Syntax

A `rabbitmq_config` resource block declares the RabbitMQ configuration data to be tested:

```ruby
describe rabbitmq_config.params('rabbit', 'ssl_listeners') do
  it { should cmp 5671 }
end
```

where

- `params` is the list of parameters configured in the RabbitMQ config file
- `{ should cmp 5671 }` tests the value of `rabbit.ssl_listeners` as read from `rabbitmq.config` versus the value declared in the test

## Examples

The following examples show how to use this Chef InSpec audit resource.

Test the list of TCP listeners:

```ruby
describe rabbitmq_config.params('rabbit', 'tcp_listeners') do
  it { should eq [5672] }
end
```

## Matchers

{{< readfile file="content/reusable/md/inspec_matchers_link.md" >}}

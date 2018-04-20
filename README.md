# born4it-amqp-starter
Example of an AMQP starter using Spring Boot and Spring AMQP

* Provide configuration properties to describe an AMQP setup, being the brokers, virtual hosts, users, exchanges, queues, dead letter queues, queue bindings ...
* Provide auto creation of the defined AMQP setup upon application startup, configuration change ...

```
born4it:
  amqp:
    servers:
      primary:
        addresses: foo
        virtualhost: foo
        username: foo
        password: foo
        exchanges:
          foo:
            queues:
              app1.foo
                dlq: true
              app2.foo
                dlq: false
```

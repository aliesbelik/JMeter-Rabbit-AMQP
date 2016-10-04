# JMeter-Rabbit-AMQP
======================

A [JMeter](http://jmeter.apache.org/) plugin to publish & consume messages from [RabbitMQ](http://www.rabbitmq.com/) or any [AMQP](http://www.amqp.org/) message broker.


JMeter Runtime Dependencies
---------------------------

Prior to building or installing this JMeter plugin, ensure that the [RabbitMQ client library](https://www.rabbitmq.com/java-client.html) (amqp-client-3.x.x.jar) is installed in JMeter's lib/ directory.


Build Dependencies
------------------

Build dependencies are managed by Maven.<br>
JARs should automatically be downloaded by Maven as part of the build process.

In addition, you'll need to copy or symlink the following from JMeter's lib/ext directory:
* ApacheJMeter_core.jar

Building
--------

The project is built using Maven.<br>
To execute the build script, just execute:

```
maven package
```

Installing
----------

To install the plugin, build the project and copy the generated JMeterAMQPSampler.jar from target/dist to JMeter's lib/ext/ directory.

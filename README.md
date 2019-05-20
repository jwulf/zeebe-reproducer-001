# zeebe-reproducer-001

Reproducer for a Zeebe issue, demonstrating a minimal reproducer.

# Expected behavior

With the included BPMN model, I expect the arrow before the message catch event to be green after a message passes through it.

# Actual behavior

What actually happens is that the message is caught, but the arrow is not green.

# Steps to Reproduce

1. Start the broker using `docker-compose` and this [configuration](https://github.com/zeebe-io/zeebe-docker-compose/tree/master/simple-monitor):

```
docker-compose up
```


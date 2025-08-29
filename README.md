# k8s pod to debug networking issues

## How to use:

- Apply the pod.yaml manifest

## DNS Resoution

- Shell into the pod

```bash
dig example.com +short
```

## Network Connectivity

```bash
nc -vz example.com 443
```

# psql pod to debug postgresql issues

```bash
psql -h your-postgres-host -U youruser -d yourdb
```

```bash
kafkacat -b my-kafka:9092 \
-G mytestgroup my-topic \
-X security.protocol=SASL_SSL \
-X sasl.mechanisms=PLAIN \
-X sasl.username='' \
-X sasl.password=''
```

```bash
kafkacat -b my-kafka:9092 \
-C \
-o beginning \
-t my-topic\
-X security.protocol=SASL_SSL \
-X sasl.mechanisms=PLAIN \
-X sasl.username='' \
-X sasl.password=''
```
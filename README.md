# kafka
Produce SBP streams over Kafka, consume it and analyze on demand.

## Installation on MacOsX

```
brew install openssl zookeeper kafka librdkafka;
stack init;
stack build;
```

## Running on MacOsX

Open two terminals. In the first,

```
./scripts/start_zookeeper.sh;
./scripts/add_example_topic.sh;
```

In the second,

```
stack run;
```

# To Do
1. Send different SBP messages to different topics & consume
2. Calculate e.g. min error live.

# Source
At this point, the repo is a fork of
[https://github.com/haskell-works/hw-kafka-client]

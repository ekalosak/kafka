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
1. Send different SBP messages to 2 different topics & consume.
2. Calculate e.g. min error live by sending only position.
3. Build reader monad that can be sent as a kafka message containing workflow
   ID, Piksi ID, or Piksi Run ID. This makes wrapping relevant SBP cleaner.
4. Read from topic, get ^^ monad contents, and do a basic gnss-analysis over a
   piksi run.

# Source
At this point, the repo is a fork of
[https://github.com/haskell-works/hw-kafka-client]

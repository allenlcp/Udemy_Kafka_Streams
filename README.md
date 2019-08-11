# Udemy_Kafka_Streams

## Terminology

<img width="300" alt="Topics, partitions and offsets" src="https://github.com/allenlcp/Udemy_Kafka_Streams/blob/master/resources/images/img_0001.png">

**Stream** - is a sequence of immutable data records, that fully ordered, can be replayed, and is fault tolerant (think of a Kafka Topic as a parallel)

**Stream Processor** - is a node in the processor topology (graph). It transforms incoming streams, record by record, and may create a new stream from it

**Topology** - is a graph of processors chained together by streams

<img width="300" alt="Topics, partitions and offsets" src="https://github.com/allenlcp/Udemy_Kafka_Streams/blob/master/resources/images/img_0002.png">

**Source Processor** - is a special processor that takes its data directly from a Kafka Topic.  It has no predecessors in a topology, and doesn't transform the data.

**Sink Processor** - is a processor that does not have children, it sends the stream data directly to a Kafka topic

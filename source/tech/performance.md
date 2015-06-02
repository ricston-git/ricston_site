## About performance

For questions pertaining to the measurement or improvement of code and application efficiency.

The performance of applications is often a paramount concern for mission critical systems. If your question pertains to optimization, whether it be database queries, algorithms, reducing network/transactional overhead, or anything that deals with speed or capacity, consider using this tag.

A good question states performance goals that need to be achieved as well as other restrictions. Trying to optimize something without measuring is not a "performance" question or work, but most likely personal entertainment - expect a question without goals/measurements to be treated as such.

Performance for many programs is represented in [big O notation](https://en.wikipedia.org/wiki/Big_O_notation), which classifies how an algorithm's resource requirements change in response to a change in input size.

This tag can also represent [system performance](http://en.wikipedia.org/wiki/Performance_tuning), which is one of key non-functional requirements of an application or system.

The two main measures of performance are

*   Throughput (how many in a time frame). Example of units: transactions per second (TPS), megabytes per second (MB/s), giga-bits per second (Gb/s), messages/request/pages per second.
*   Latency (how long for an action). For example, seek time of 8 ms and search time of 100 ms.

Latency is often qualified with a statistical measure. Note: latencies usually don't follow a [normal distribution](https://en.wikipedia.org/wiki/Normal_distribution) and have very high upper limits compared with the average latency. As such the [standard deviation](https://en.wikipedia.org/wiki/Standard_deviation) is not useful.

*   Average latency. The average of all the latencies.
*   Typical or [median](https://en.wikipedia.org/wiki/Median) latency. The mid-point of the range of possible latencies. This is usually 50% to 90% of the average latency. As this is the lowest figure it is often reported by vendors.
*   Percentile latency. The figure it is less than or equal to N% of the time. That is, 99 percentile if the latency it is not more than this, 99 times out of 100.
*   Worst or maximum latency. The highest latency measured.

When seeking to improve performance: prototype and measure first, optimize only if and where needed.

**See also:** [optimization](http://stackoverflow.com/questions/tagged/optimization "show questions tagged 'optimization'") [profiling](http://stackoverflow.com/questions/tagged/profiling "show questions tagged 'profiling'") [assembly](http://stackoverflow.com/questions/tagged/assembly "show questions tagged 'assembly'") [compiler](http://stackoverflow.com/questions/tagged/compiler "show questions tagged 'compiler'") [low-latency](http://stackoverflow.com/questions/tagged/low-latency "show questions tagged 'low-latency'")
Once an application process uses an external data source, its performance can be bottlenecked
by the throughput and latency of said data source. When a slower external data source is used,
frequently accessed data is often moved temporarily to a faster storage that is closer to the
application to boost the application’s performance. This faster intermediate data storage is
called the application’s cache, a term originating from the French verb “cacher” which means “to
hide.”


Why cache
The cache’s main purpose is to reduce the time needed to access data stored outside of the
application’s main memory space. Additionally, caching is also an extremely powerful tool for
scaling up external data sources and mitigating the effects that usage spikes have on them.
An application-side cache effectively reduces all resource demands needed to serve data from
external sources, thus freeing these resources for other uses. Without the use of a cache, the
application interacts with the data source for every request, whereas when a cache is employed
only a single request to the external data source is needed, with subsequent access served from
the cache.
Additionally, a cache also contributes to the application’s availability. External data sources
may experience failures that result in degraded or terminated service. During such outages the
cache can still serve data to the application and thus retain its availability


References
- https://redislabs.com/wp-content/uploads/2016/03/15-Reasons-Caching-is-best-with-Redis-RedisLabs-1.pdf

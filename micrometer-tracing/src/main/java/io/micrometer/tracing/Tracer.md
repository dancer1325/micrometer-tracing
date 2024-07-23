* API /
  * 👁️heavily influenced by Brave 👁️
  * uses
    * create
      * root span / -- captures the -- critical path of a request
      * child spans / -- allocate latency related to -- outgoing requests
  * use cases
    * if you trace 1! thread code -> run | `ScopedSpan`
      * _Example:_ Check javadoc code -- TODO: Add in a real code --
    * if you need more features OR finer control -> run | `Span`
      * _Example:_ Check javadoc code -- TODO: Add in a real code --
* `Tracer.SpanInScope`
  * == scope of a span
  * to let go -> you need to close it -- `close()` --
* `nextSpan()`
  * -- based on the -- current span | scope
    * if there is NO span -> new trace will be created
    * if there is a span -> child span will be created
* `withSpan(Span)`
  * what does it do?
    * input Span -- pass to be the -- current span
  * recommendation
    * wrap with `try-with-resource`
* `startScopedSpan(String)`
  * uses
    * tracing in-process commands
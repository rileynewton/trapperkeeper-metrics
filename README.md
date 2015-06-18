# `trapperkeeper-metrics`

`trapperkeeper-metrics` is a library intended to help make it easier to track
metrics in other Trapperkeeper applications.  It includes:

 * a TK service that manages the life cycle of your metrics registry
 * config-driven control of metrics and metrics reporting
 * other miscellaneous utility functions for working with metrics

For more detailed information (what this library does and doesn't do, more
detailed tips on how to write code against it, future plans, etc.), check out the
[documentation](./documentation/index.md).

## HTTP Metrics with `comidi`

To get the most value out of this library, use it in concert with
[comidi](https://github.com/puppetlabs/comidi) (to take advantage of the
built-in HTTP metrics; see the comidi docs)
and the [Trapperkeeper Status Service](https://github.com/puppetlabs/trapperkeeper-status)
(to expose the most useful metrics data from your app via HTTP).

The comidi repo contains a working example app that illustrates how to tie
everything together.


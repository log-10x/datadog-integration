# CHANGELOG - log10x

<!-- towncrier release notes start -->

## 1.0.1 / 2026-11-11

***Fixed***:

* The share panel on the dashboard now shows the bytes passed to Standard Indexing (route `pass`) as a percent of bytes read.
* Removed the `log10x.bytes.encoded.count` metric and its dashboard panel. Compaction does not apply to Datadog, so the metric carried no data.

***Changed***:

* The "No reduction" monitor is now "Everything passes to the Standard path" and reads `routestate:pass`.
* The "Check is not reporting" monitor has one name for every host; its message still names the host.
* The forwarded metrics are described as counting every route, split by `routestate`.
* The README covers a second Agent instance for the Retriever's offload and retrieval metrics, and the Free tier the engine runs on without a license.
* The dashboard logo loads from doc.log10x.com.

## 1.0.0 / 2026-09-13

***Added***:

* Initial Release

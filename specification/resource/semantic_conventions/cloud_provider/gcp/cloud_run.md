# Google Cloud Run

**Status**: [Experimental][DocumentStatus]

These conventions are recommended for resources running on Cloud Run.

**Type:** `gcp.cloud_run`

**Description:** Resource attributes for Cloud Run.

<!-- semconv gcp.cloud_run -->
| Attribute  | Type | Description  | Examples  | Requirement Level |
|---|---|---|---|---|
| `gcp.cloud_run.job.execution` | string | The name of the Cloud Run [execution](https://cloud.google.com/run/docs/managing/job-executions) being run for the Job, as set by the [`CLOUD_RUN_EXECUTION`](https://cloud.google.com/run/docs/container-contract#jobs-env-vars) environment variable. | `job-name-xxxx`; `sample-job-mdw84` | Recommended |
| `gcp.cloud_run.job.task_index` | int | The index for a task within an execution as provided by the [`CLOUD_RUN_TASK_INDEX`](https://cloud.google.com/run/docs/container-contract#jobs-env-vars) environment variable. | `0`; `1` | Recommended |
<!-- endsemconv -->

[DocumentStatus]: https://github.com/open-telemetry/opentelemetry-specification/blob/v1.21.0/specification/document-status.md

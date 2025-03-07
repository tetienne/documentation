---
title: Set up Tracing on a Buildkite Pipeline
kind: documentation
further_reading:
    - link: "/continuous_integration/explore_pipelines"
      tag: "Documentation"
      text: "Explore Pipeline Execution Results and Performance"
    - link: "/continuous_integration/troubleshooting/"
      tag: "Documentation"
      text: "Troubleshooting CI"
---

{{< site-region region="us5,gov" >}}
<div class="alert alert-warning">
The selected Datadog site ({{< region-param key="dd_site_name" >}}) is not supported.
</div>
{{< /site-region >}}

{{< site-region region="us,eu,us3" >}}
## Configure the Datadog integration

The steps to activate the Datadog integration for [Buildkite][1] are:

1. Go to **Settings > Notification Services** in Buildkite and click add a **Datadog Pipeline Visibility** integration.
2. Fill in the form with the following information:
   * **Description**: A description to help identify the integration in the future, such as Datadog CI Visibility integration.
   * **API key**: your [Datadog API Key][2].
   * **Datadog site**: {{< region-param key="dd_site" code="true" >}}
   * **Pipelines**: Select all pipelines or the subset of pipelines you want to trace.
   * **Branch filtering**: Leave empty to trace all branches or select the subset of branches you want to trace.
3. Click **Add Datadog Pipeline Visibility Notification** to save the integration.

## Visualize pipeline data in Datadog

The [Pipelines][3] and [Pipeline Executions][4] pages populate with data after the pipelines finish.

**Note**: The Pipelines page shows data for only the default branch of each repository.

{{< /site-region >}}

## Further reading

{{< partial name="whats-next/whats-next.html" >}}
[1]: https://buildkite.com
[2]: https://app.datadoghq.com/organization-settings/api-keys
[3]: https://app.datadoghq.com/ci/pipelines
[4]: https://app.datadoghq.com/ci/pipeline-executions

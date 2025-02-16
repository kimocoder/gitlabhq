# Insights **[ULTIMATE]**

> Introduced in [GitLab Ultimate](https://about.gitlab.com/pricing/) 11.9 behind the `insights` feature flag.

CAUTION: **Beta:**
Insights is considered beta, and is not ready for production use.
Follow [gitlab-org/quality/team-tasks#137](https://gitlab.com/gitlab-org/quality/team-tasks/issues/137#general-availability)
for updates.

Configure the Insights that matter for your groups to explore data such as
triage hygiene, issues created/closed per a given period, average time for merge
requests to be merged and much more.

![Insights example stacked bar chart](img/insights_example_stacked_bar_chart.png)

## View your group's Insights

You can access your group's Insights by clicking the **Overview > Insights**
link in the left sidebar:

![Insights sidebar link](img/insights_sidebar_link.png)

## Configure your Insights

Navigate to your group's **Settings > General**, expand **Insights**, and choose
the project that holds your `.gitlab/insights.yml` configuration file:

![group insights configuration](img/insights_group_configuration.png)

If no configuration was set, a [default configuration file](
https://gitlab.com/gitlab-org/gitlab-ee/blob/master/ee/fixtures/insights/ee/fixtures/insights/default.yml)
will be used.

See the [Project's Insights documentation](../../project/insights/index.md) for
more details about the `.gitlab/insights.yml` configuration file.

## Permissions

If you have access to view a group, then you have access to view their Insights.

NOTE: **Note:**
Issues or merge requests that you don't have access to (because you don't have
access to the project they belong to, or because they are confidential) are
filtered out of the Insights charts.

You may also consult the [group permissions table](../../permissions.md#group-members-permissions).

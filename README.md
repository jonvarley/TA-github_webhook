# Splunk Add-on for GitHub Webhooks

The **Splunk Add-on for GitHub Webhooks** provides a structure for collecting data from GitHub Webhooks and maps them to the DevOps data model.

## Sourcetypes for the **Splunk Add-on for GitHub Webhooks**

The sourcetypes map to the Github Webhook event as described in the [Github Webhook Event Payloads Documentation](https://developer.github.com/webhooks/event-payloads/)

| Sourcetype										| Description 	|
  -------------------------------------------------	| -------------	|
| github:webhook:check_run							| Check run activity has occurred |
| github:webhook:check_suite						| Check suite activity has occurred |
| github:webhook:commit_comment						| A commit comment is created |
| github:webhook:content_reference					| A new content reference is created |
| github:webhook:create								| A Git branch or tag is created |
| github:webhook:delete								| A Git branch or tag is deleted |
| github:webhook:deploy_key							| A deploy key is added or removed from a repository |
| github:webhook:deployment							| A deployment is created |
| github:webhook:deployment_status					| A deployment is created |
| github:webhook:fork								| A user forks a repository |
| github:webhook:github_app_authorization			| When someone revokes their authorization of a GitHub App, this event occurs |
| github:webhook:gollum								| A wiki page is created or updated |
| github:webhook:installation						| Activity related to a GitHub App installation |
| github:webhook:installation_repositories			| Activity related to repositories being added to a GitHub App installation |
| github:webhook:issue_comment						| Activity related to an issue comment |
| github:webhook:issues								| Activity related to an issue |
| github:webhook:label								| Activity related to a label |
| github:webhook:marketplace_purchase				| Activity related to a GitHub Marketplace purchase |
| github:webhook:member								| Activity related to repository collaborators |
| github:webhook:membership							| Activity related to team membership |
| github:webhook:meta								| The webhook this event is configured on was deleted |
| github:webhook:milestone							| Activity related to milestones |
| github:webhook:organization						| Activity related to an organization and its members |
| github:webhook:org_block							| Activity related to people being blocked in an organization |
| github:webhook:package							| Activity related to GitHub Packages |
| github:webhook:page_build							| Represents an attempted build of a GitHub Pages site, whether successful or not |
| github:webhook:ping								| A simple ping event to let you know you've set up the webhook correctly |
| github:webhook:project_card						| Activity related to project cards |
| github:webhook:project_column						| Activity related to columns in a project board |
| github:webhook:project							| Activity related to project boards |
| github:webhook:public								| When a private repository is made public |
| github:webhook:pull_request						| Activity related to pull requests |
| github:webhook:pull_request_review				| Activity related to pull request reviews |
| github:webhook:pull_request_review_comment		| Activity related to pull request review comments in the pull request's unified diff |
| github:webhook:push								| One or more commits are pushed to a repository branch or tag |
| github:webhook:release							| Activity related to a release |
| github:webhook:repository_dispatch				| This event occurs when a GitHub App sends a POST request to the "Create a repository dispatch event" endpoint |
| github:webhook:repository							| Activity related to a repository |
| github:webhook:repository_import					| Activity related to a repository being imported to GitHub |
| github:webhook:repository_vulnerability_alert		| Activity related to security vulnerability alerts in a repository |
| github:webhook:security_advisory					| Activity related to a security advisory |
| github:webhook:sponsorship						| Activity related to a sponsorship listing |
| github:webhook:star								| Activity related to a repository being starred |
| github:webhook:status								| When the status of a Git commit changes |
| github:webhook:team								| Activity related to an organization's team |
| github:webhook:team_add							| When a repository is added to a team |
| github:webhook:watch								| When someone stars a repository |
| github:webhook:workflow_dispatch					| This event occurs when someone triggers a workflow run on GitHub |

## Compatibility

This add-on was built on version 8.0.3 of Splunk Enterprise and is compatible with the following software and platforms:

| Splunk platform versions          | 8.x |
| CIM                               | N/A |
| Supported OS for data collection  | All supported operating systems |
| Vendor products                   | Tested using GitHub.com |

## Installation

Installing this add-on involves the following steps:

1. Download the add-on
2. Determine where to install this add-on in your deployment using the table below.
3. Configure HEC input to receive GitHub data as described below.
4. Configure Github Webhook to send webhook data to the HEC endpoint.

## Reference 
- This Add-on was built via [Splunk Add-On Builder](https://docs.splunk.com/Documentation/AddonBuilder/latest/UserGuide/Thirdpartysoftwarecredits).

# Slack GitHub Notification Setup

Subscribe to GitHub Actions deployment notifications in a Slack channel
using the [Slack GitHub App](https://slack.github.com/).

## Prerequisites

- Slack GitHub App installed in your workspace

## Subscribe to Workflow Notifications

Run the following commands in your Slack channel:

```text
/github subscribe ysoftman/sbbs workflows:{event:"push" branch:"main"}
```

This sends workflow start/success/failure notifications on `main` branch pushes.

## Subscribe to Deployment Events

```text
/github subscribe ysoftman/sbbs deployments
```

## Check Current Subscriptions

```text
/github subscribe list
```

## Unsubscribe Unnecessary Events

```text
/github unsubscribe ysoftman/sbbs issues pulls commits releases
```

> [!IMPORTANT]
> This project is _community supported_. This means that you should not contact
> Qlik Support for help with these apps. See below for additional information
> on how to raise issues on this repository to ask for help.

# Qlik Cloud Automation Analyzer

> **Note**
> This application is one of a set of community built and supported monitoring apps for Qlik Cloud.
> For links to all monitoring apps, visit the [Qlik Cloud Monitoring Apps](https://github.com/qlik-oss/qlik-cloud-monitoring-apps) repository.

The Automation Analyzer is a Qlik Sense application built for Qlik Cloud, which
helps you to analyze and monitor Qlik Application Automation runs in your tenant.

![Sheets in the app](/images/readme_sheets.png)

Some of the benefits of this application are as follows:

- Track number of automations by type and by user
- Analyze concurrent automations
- Compare current month vs prior month runs
- Analyze failed runs - view all schedules and their statuses
- Tie in Qlik Alerting

This application:

- Pulls a max of 90 days of automation run history, and will then continue to build from there incrementally using QVDs.
- Does not pull in runs that are currently running.
- Should not be used as an audit application.

Endpoints:

- audits
- tenants
- spaces
- users
- automations
- automations/{id}/runs/{id}

## Installing/ updating

This application can be installed via an interactive Qlik Automate [installer](https://community.qlik.com/t5/Official-Support-Articles/Qlik-Cloud-Monitoring-Apps-Workflow-Guide/ta-p/2134140) or [manually](/../../releases) using the PDF guide.

## Support policy

This app is provided as-is and is not supported by Qlik. Over time, the APIs and
metrics used by the app may change, so it is advised to monitor this repository
for updates, and to update the app promptly when new versions are available.

If you have issues while using this app, support is provided on a best-efforts
basis by contributors to this project.

If you have an issue:

- Review the FAQ section in this readme to see if your issue is a common one
- Review open and closed [issues](/../../issues)
- Open a [new issue](/../../issues/new), following the issue template

If you are able to resolve the issue, then close your issue with the resolution,
and if you feel inclined, open a PR with your proposed changes so that we can
consider including the improvement in the next release of the app.

Thank you for your support!

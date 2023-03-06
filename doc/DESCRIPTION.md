WebUI for smartd S.M.A.R.T monitoring

> NOTE: Scrutiny is a Work-in-Progress and still has some rough edges.

# Introduction

If you run a server with more than a couple of hard drives, you're probably already familiar with S.M.A.R.T and the `smartd` daemon. If not, it's an incredible open source project described as the following:

> smartd is a daemon that monitors the Self-Monitoring, Analysis and Reporting Technology (SMART) system built into many ATA, IDE and SCSI-3 hard drives. The purpose of SMART is to monitor the reliability of the hard drive and predict drive failures, and to carry out different types of drive self-tests.

Theses S.M.A.R.T hard drive self-tests can help you detect and replace failing hard drives before they cause permanent data loss. However, there's a couple issues with `smartd`:

- There are more than a hundred S.M.A.R.T attributes, however `smartd` does not differentiate between critical and informational metrics
- `smartd` does not record S.M.A.R.T attribute history, so it can be hard to determine if an attribute is degrading slowly over time.
- S.M.A.R.T attribute thresholds are set by the manufacturer. In some cases these thresholds are unset, or are so high that they can only be used to confirm a failed drive, rather than detecting a drive about to fail.
- `smartd` is a command line only tool. For head-less servers a web UI would be more valuable.

**Scrutiny is a Hard Drive Health Dashboard & Monitoring solution, merging manufacturer provided S.M.A.R.T metrics with real-world failure rates.**

# Features

Scrutiny is a simple but focused application, with a couple of core features:

- Web UI Dashboard - focused on Critical metrics
- `smartd` integration (no re-inventing the wheel)
- Auto-detection of all connected hard-drives
- S.M.A.R.T metric tracking for historical trends
- Customized thresholds using real world failure rates
- Temperature tracking
- Provided as an all-in-one Docker image (but can be installed manually)
- Configurable Alerting/Notifications via Webhooks
- (Future) Hard Drive performance testing & tracking

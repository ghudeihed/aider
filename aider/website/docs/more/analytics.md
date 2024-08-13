---
parent: More info
nav_order: 500
---

# Analytics

Aider uses MixPanel to collect anonymous analytics that are used to help
improve aider. 
**Analytics is currently turned off by default**, but expected to be turned on by default in
a future release.

## Anonymous, no personal info

No personal information is collected: no user identity, none of your code,
prompts or chat messages.

Aider collects information on which models are used and with how many tokens,
which edit formats are used, how often features and commands are used,
information about exceptions, etc.
These analytics are associated with an anonymous,
randomly generated UUID4 user identifier.

This information helps improve aider by identifying which models, edit formats,
features and commands are most used.
It also helps uncover bugs that users are experiencing, so that they can be fixed
in upcoming releases.

## Sample analytics data

To get a better sense of what type of data is collected, you can review some
[sample analytics logs](https://github.com/paul-gauthier/aider/blob/main/aider/website/assets/sample-analytics.jsonl).
These are the last 1,000 analytics events from the author's
personal use of aider.

## Enabling & disabling analytics

You can easily opt out of analytics forever by running this command one time:

```
aider --analytics-disable
```

To enable analytics for a single session, you can run:

```
aider --analytics
```

To disable analytics for a single session, you can run:

```
aider --no-analytics
```

## Logging and inspecting analytics

You can get a full log of all the data that aider is collecting,
in case you would like to audit or inspect this data.

```
aider --analytics-log filename.jsonl
```

If you want to just log analytics without reporting them to MixPanel, you can do:

```
aider --analytics-log filename.jsonl --no-analytics
```


## Reporting issues

Please open a
[GitHub Issue](https://github.com/paul-gauthier/aider/issues)
if you have concerns about any of the analytics that aider is collecting.


## Legal compliance 

Aider is committed to complying with applicable data protection and privacy laws, including but not limited to the General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA). Here's how we ensure compliance:

1. No Personal Data Processing: We do not collect or process any personal data. All data collected is anonymous and cannot be linked back to individual users.

2. Legal Basis: The collection of anonymous usage data is based on legitimate interest to improve our software and user experience.

3. Data Retention: Anonymous usage data is retained for a period of 5 years, after which it is automatically deleted.

4. User Rights: As we do not collect personal data, individual data subject rights (such as access, rectification, erasure) are not applicable. However, users have the right to opt-out of data collection entirely (see "Disabling analytics" section).

5. Data Protection: We implement appropriate technical and organizational measures to ensure a level of security appropriate to the risk.

If you have any questions or concerns about our data practices, 
please contact us by opening a
[GitHub Issue](https://github.com/paul-gauthier/aider/issues).

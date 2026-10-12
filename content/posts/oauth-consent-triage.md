---
title: "How I triage OAuth consent grants in Entra ID"
date: 2026-10-11   # set to the day you publish — Hugo hides future dates
draft: true          # change to false when ready to publish
tags: ["entra-id", "oauth", "kql", "detection"]
summary: "What a risky consent grant looks like in the audit logs, how to triage one, and a KQL detection you can test in your own tenant."
---

<!--
POST TEMPLATE — delete these comments before publishing.
Use lab data only: no client names, tenant IDs, IP addresses or real alert text.
-->

## The threat

<!-- What the attacker does and why it matters. Link a real public incident report or Microsoft guidance. -->

## How it works

<!-- The technique in plain words. MITRE ATT&CK: T1528 Steal Application Access Token. -->

## Lab setup

<!-- Your test tenant, the test app you registered, the permissions you requested. Enough for a reader to reproduce it. -->

## The detection

```kql
// Replace with your tested query
AuditLogs
| where OperationName == "Consent to application"
| take 10
```

<!-- Explain the query line by line. -->

## Testing

<!-- How you triggered it, what fired, a screenshot from your lab. -->

## False positives and tuning

<!-- Which legitimate activity looks the same, and how you handled it. -->

## Limits

<!-- What this detection misses. Be honest — this is what makes the post credible. -->

## Links

- Detection in the repository: <!-- link -->
- Sources: <!-- links -->

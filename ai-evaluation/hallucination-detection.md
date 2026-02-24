# Hallucination Detection – AI Evaluation Sample

## Overview

This sample demonstrates how I identify, analyze, and correct hallucinations in AI-generated technical content.

A hallucination occurs when an AI system:
- Produces information that is incorrect or unverifiable
- Invents features, behaviors, or causes
- Sounds confident but lacks factual grounding

This example shows a real-world evaluation workflow.

---

## Example 1: Feature Availability Hallucination

### AI-Generated Response (Before)

The system automatically encrypts all user data at rest and in transit using AES-256 encryption by default.

---

### Issue Identified

- The response **asserts a security feature** without confirmation.
- No product documentation confirms default AES-256 encryption.
- This could lead to **compliance and trust issues**.

This is a **high-risk hallucination**.

---

### Human Evaluation Notes

- Security claims must be explicitly verified.
- If documentation is unclear, the AI should avoid absolute statements.
- Safer responses must include conditions or references.

---

### Corrected Response (After)

User data is encrypted in transit using industry-standard protocols.  
Encryption at rest depends on the deployment configuration and must be verified with your administrator or official product documentation.

---

## Example 2: Root Cause Hallucination

### AI-Generated Response (Before)

Your payment failed due to an internal server outage.

---

### Issue Identified

- Root cause is stated without evidence.
- The system does not expose outage-level diagnostics.
- Misleads the user and increases support load.

---

### Corrected Response (After)

The payment could not be completed due to a temporary system issue.  
Please wait a few minutes and retry the transaction. If the issue persists, contact support.

---

## Hallucination Detection Checklist

When reviewing AI-generated content, I check for:

- ❓ Unsupported claims presented as facts
- ❓ Assumed root causes without data
- ❓ Feature descriptions not present in official docs
- ❓ Overly confident language (“always”, “guaranteed”)
- ❓ Missing uncertainty indicators where required

---

## Risk Classification

| Hallucination Type | Risk Level |
|-------------------|-----------|
| Security claims   | High      |
| Compliance claims | High      |
| Error causes      | Medium    |
| Performance claims| Medium    |
| UI descriptions  | Low–Medium|

---

## Audience

- AI training and evaluation teams
- Technical writers
- Product and support teams

---

*This sample is recreated for portfolio purposes and does not reflect any real product behavior.*

# Siwanplan Scheduled Routine

Cloud scheduled routine for Siwanplan content operations.

## Purpose

This repository documents a cloud-based scheduled task that helps operate Siwanplan content workflows for doctors and clinic owners.

The routine is designed to find timely content candidates for Threads, using official sources and recent news. It does not publish posts, upload to social media, or send external messages automatically.

## Automation Link

https://chatgpt.com/scheduled?automationId=6ac338e041088190a0ba6695599cbfff&automationSource=cloud&share_dialog=true

## Runtime

- Execution environment: Cloud
- Local computer execution: Off
- Start in a new chat each run: On
- Timezone: Asia/Seoul
- Main schedule: Daily at 08:40

## Main Routine

Every morning, the automation finds three timely Siwanplan content candidates for doctors and clinic owners.

Each candidate includes:

- Candidate title
- Why the topic is timely
- Doctor or clinic-owner angle
- Money, responsibility, and insurance-adjacent connection point
- Duplicate-avoidance note
- Source link and date
- Recommendation order

## Source Scope

The routine prioritizes official and reliable sources:

- Ministry of Health and Welfare
- Financial Services Commission
- Financial Supervisory Service
- National Tax Service
- Ministry of Employment and Labor
- Health Insurance Review and Assessment Service
- Ministry of Land, Infrastructure and Transport
- Korea Policy Briefing
- Recent reliable news when useful

## Safety Rules

- Do not publish to Threads automatically.
- Do not upload to Instagram automatically.
- Do not post comments automatically.
- Do not send external messages automatically.
- Produce drafts, candidates, summaries, and review notes only.
- Treat "좋아", "응", or "괜찮아" as feedback, not publishing approval.
- Publish only after explicit approval such as "올려줘", "업로드해", or "이대로 올려".
- Check recent content history and avoid topics with more than 50% overlap.
- Verify sources and dates.
- Flag insurance advertising compliance risks.

## Repository Contents

```text
siwanplan-scheduled-routine/
├─ README.md
├─ prompts/
│  └─ siwanplan-hot-topics.md
├─ docs/
│  └─ automation-settings.md
└─ examples/
   └─ sample-output.md
```

## Submission Notes

This repository is a documentation package for the scheduled task. The actual scheduled task runs in ChatGPT/Codex cloud through the shared automation link above.

# Screenshot and walkthrough plan

[Back to the project overview](../README.md)

Use an isolated demonstration environment with synthetic records. These are planned captures, not screenshots of completed validation.

## Capture list

| File to add under `assets/screenshots/` | View | Suggested caption |
| --- | --- | --- |
| `01-dispatch-overview.png` | Web dispatch board with several synthetic jobs and technicians | Dispatchers coordinate service requests, assignments, and job status from a shared operations view. |
| `02-vehicle-fitment-quote.png` | Vehicle selection, compatible batteries, and demo quote | Vehicle-to-battery fitment connects intake to compatible products and shared pricing rules. |
| `03-scheduling-map.png` | Appointment planning and map using demonstration locations | Scheduling and map-based planning connect each appointment to a technician's field work. |
| `04-technician-job.png` | Native assigned-job detail | Technicians receive job and vehicle information in the field. |
| `05-installation-documentation.png` | Native installation-photo workflow using staged photos | Installation documentation is connected to the service record. |
| `06-service-payment-review.png` | Web job history or payment-review screen with synthetic data | Service history and payment records give staff context for follow-up and reconciliation. |

Prioritize the dispatch overview, fitment quote, and two native views. Four readable images are enough for a first public version. Only use screens that are implemented and render correctly in the demonstration build; adjust captions to match what is actually visible.

## Before publishing

- Use fake names, reserved example email addresses, and clearly synthetic records. Do not use a production database just to get realistic screenshots.
- Keep real customer addresses, employee locations, phone numbers, vehicle identifiers, payment identifiers, and customer photos out of the scene. Prefer replacing source data to blurring it afterward.
- Keep credentials, tokens, session URLs, developer tools, notifications, and internal infrastructure details out of the frame.
- Show only demo pricing. Do not initiate real payments, send real SMS, or dispatch real jobs to create screenshots.
- Use staged installation photos you are allowed to publish. Remove unnecessary image metadata before publication.
- Capture web screens at a consistent desktop size and native screens at a consistent portrait size. Keep the text readable and crop unnecessary browser/device chrome.
- Review every final image at full size before adding it to Git. Deleting a committed image later does not remove it from repository history.
- Once images are approved, embed them in the README with concise captions and descriptive alt text. Remove the pending-capture note only when the images exist.

## Optional short video

A 60–90 second recording can follow the same synthetic job from dispatcher intake to the technician's view. Explain the user problem, show the fitment workflow, switch to the native app, and close with a brief explanation of the shared backend. Do not imply a successful live payment or a completed production rollout from a demonstration.

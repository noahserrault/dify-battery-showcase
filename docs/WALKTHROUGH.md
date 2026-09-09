# Web and native-app walkthrough

[Project overview](../README.md) · [Engineering overview](ENGINEERING.md)

These screenshots show the DIFY staging website and Android sandbox app on a Pixel 8 emulator. They were taken on September 8, 2026, using fictional customers, service locations, and technicians. Prices are demo examples, not advertised rates.

## Jobs

Dispatchers can compare job status, appointments, assignments, and payment information in one searchable table. This view is filtered to five demo jobs.

![Jobs table filtered to five synthetic DIFY service records](../assets/screenshots/02-jobs-overview.jpg)

## Dispatch board

The board groups jobs by technician and shows their status and appointment windows. This refreshed capture shows three calls assigned to Technician A, two to Technician B, and one new intake awaiting assignment. These demo jobs are dated September 5, which is why they appear overdue.

<details>
<summary>View dispatcher board</summary>

![Dispatcher board with three demo calls assigned to Technician A, two to Technician B, and one unassigned](../assets/screenshots/01-dispatch-balanced.png)

</details>

## Intake and quoting

Dispatchers enter the customer, location, and vehicle, check technician availability, and select a battery from the catalog. The estimate includes taxes and fees. This example was filled out for the screenshot and not saved.

Vehicle selection and catalog selection are separate steps here. Battery-fitment guidance is also available in the lookup view.

<details>
<summary>View intake and recommended quote</summary>

![Unsaved synthetic intake form with vehicle selection, scheduling, and a catalog-based recommended estimate](../assets/screenshots/03-intake-quote.jpg)

</details>

## Route planning

The map shows stop order, appointment windows, and estimated drive times. Lines connect the stops rather than following roads. Live GPS is hidden when viewing a past date.

<details>
<summary>View planning map and stop sequence</summary>

![Austin planning map showing five synthetic service stops and a technician route summary](../assets/screenshots/05-planning-map.jpg)

</details>

## Service records

Opening a job shows its vehicle, battery, service address, schedule, and assigned technician. This screenshot shows the top of an in-progress demo job.

<details>
<summary>View staff service record</summary>

![Staff job-detail interface for a synthetic in-progress battery installation](../assets/screenshots/04-service-record.jpg)

</details>

## Technician app

Technicians can see their current stop and the rest of the day's route. Opening a job brings up dispatcher notes, vehicle and battery details, and required photos.

<p>
  <img src="../assets/screenshots/06-native-route.png" width="270" alt="Native technician route with the current stop and other synthetic assignments" />
  <img src="../assets/screenshots/07-native-job.png" width="270" alt="Native job sheet with dispatch notes, vehicle and battery details" />
  <img src="../assets/screenshots/08-native-documentation.png" width="270" alt="Native required-photo interface with old and new battery photo slots and a payment entry point" />
</p>

The job sheet includes slots for old and new battery photos, pricing, and a checkout button. No photos were uploaded or payments taken for these screenshots.

## Capture notes

- Existing demo records were reused without changing their assignments, schedules, or status.
- The Android screenshots show the installed sandbox app, version 1.0.0, updated September 4.
- No customer calls, messages, payments, or photo uploads were made. Location tracking was not enabled.
- These are interface examples, not a record of completed production, payment, or offline testing.

The [capture checklist](SCREENSHOT_PLAN.md) covers future screenshot updates and a short video.

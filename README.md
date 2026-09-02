# Incident Banner for osTicket

**Incident and maintenance management for osTicket.**

Incident Banner adds a structured incident-management workflow to an existing osTicket helpdesk. It is designed for organizations that need a quick, visible way to communicate outages, degraded services, planned maintenance, location connectivity problems, cloud-service interruptions, and other operational events.

Rather than relying on a single static notice, Incident Banner allows authorized staff to create and manage incidents, publish updates, link related helpdesk tickets, schedule maintenance, review incident history, and generate printable reports.

> **Current release:** v1.0.0  
> **Tested with:** osTicket 1.18.4  
> **License:** GNU GPL v2

---

## Features

- Multiple active incident banners at the same time
- Public client-portal incidents and internal staff-only incidents
- Info, Minor, Major, and Critical severity levels with distinct banner colors
- Live client and staff updates through AJAX without requiring a manual page refresh
- Expandable client update timelines displayed newest first
- Planned maintenance with start and end times
- Optional manager approval for scheduled maintenance
- Team-based Incident Linker and Maintenance Scheduler permissions
- Incident Manager access for selected agents and osTicket administrators
- Link one or more helpdesk tickets to an incident
- Manager reminder when all linked tickets are closed or resolved
- Configurable resolved-banner display period
- Numeric incident identifiers such as `INC-2026-0001`
- Active, Scheduled, Resolved, and All incident history views
- Search by incident number, title, affected service, or linked ticket
- Detailed incident audit history
- Printable incident reports
- Agent and Admin Panel reminders for active incidents
- Optional email notifications, disabled by default
- Native osTicket cron processing for scheduled lifecycle events
- HTTPS-compatible client and staff bridge assets

---

## Public and Internal Incidents

Incident Banner supports both public and internal events.

**Public incidents** can be displayed to users on the client portal and to staff inside the helpdesk.

**Internal incidents** remain available to appropriate helpdesk staff without being displayed publicly to end users.

This allows the same system to be used for customer-facing outages, internal IT events, and planned maintenance.

---

## Permissions and Workflow

Incident Banner was designed with different helpdesk roles in mind.

Higher-level Incident Managers can create, update, resolve, and administer incidents. Other trusted agents can be granted narrower permissions, such as linking open tickets to an existing incident or scheduling maintenance events, without receiving full incident-management access.

This makes it possible to extend selected incident functions to technicians, department heads, supervisors, or other trusted users while keeping administrative functions restricted.

---

## Tested Environment

Incident Banner v1.0.0 was developed and tested with:

- osTicket 1.18.4
- Apache 2.4 on Ubuntu
- PHP 8.4
- MariaDB/MySQL-compatible storage
- HTTP and HTTPS client portals
- One-minute osTicket cron execution

Compatibility with other versions, themes, plugins, web servers, PHP versions, databases, or future osTicket releases is not guaranteed.

Support for additional osTicket versions may be evaluated in future releases.

---

## Installation Overview

Incident Banner is intended for self-hosted osTicket installations and requires administrator-level access to the osTicket server.

Installation includes:

- Copying the plugin directory into `include/plugins`
- Copying the packaged bridge files to their documented locations
- Adding one include line to the client header
- Adding one include line to the staff header
- Installing, configuring, and enabling the plugin from the osTicket Admin Panel
- Configuring a working osTicket cron job

Detailed installation, upgrade, rollback, configuration, and testing instructions are included with the official release package.

**Always back up the helpdesk database and affected files before installation.**

---

## Screenshots

Screenshots and product demonstrations will be added to this repository.

---

## Purchase / Official Release

The official Incident Banner release package, documentation, eligible updates, and purchaser support are distributed by **Duster Tech Solutions**.

**Purchase/download:** Patreon link coming soon.

The complete plugin source is included with the purchased release package. This public repository is currently used for project information, compatibility details, screenshots, changelogs, and issue tracking rather than distribution of the release archive.

---

## Support

Limited purchaser support is available for installation questions and issues reasonably determined to be specific to the unmodified Incident Banner Plugin.

**Email:** dustertechsolutions@gmail.com

General server administration, osTicket repair, web-server configuration, PHP/database administration, unrelated third-party plugins, custom themes, and custom development are outside the included plugin support scope.

---

## License

Copyright © 2026 Dustin Burson d/b/a Duster Tech Solutions.

Incident Banner is licensed under the **GNU General Public License, version 2 (GPLv2)**.

GPLv2 permits use, study, modification, and redistribution under its terms. Payment for an official release provides convenient access to the verified release package, documentation, eligible updates, and limited purchaser support; it does not remove rights granted by GPLv2.

---

## Third-Party Notice

Incident Banner is independently developed for use with osTicket.

Dustin Burson and Duster Tech Solutions are not affiliated with, sponsored by, authorized by, or endorsed by osTicket or its developers. osTicket and related names and marks belong to their respective owners.

---

## Security / Privacy Reminder

Do not place passwords, protected health information, confidential records, private customer information, or other sensitive information inside a public incident banner.

---

## About Duster Tech Solutions

Duster Tech Solutions develops practical plugins, tools, and enhancements for osTicket and self-hosted IT environments.

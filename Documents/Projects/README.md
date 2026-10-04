# Awesome-Appointment-Scheduling-Software

# Awesome Appointment Scheduling Software



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Self-Hosted Booking Pages, Group Polling & Calendar Synchronization*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Appointment Scheduling**. These tools help professionals, service businesses, and teams manage bookings, share availability, and synchronize with existing calendars.



**Examples** include Microsoft Bookings, Calendly, Acuity Scheduling, YouCanBookMe, Doodle, Setmore, Appointlet, SimplyBook.me, Chili Piper, and HubSpot Meetings (the category leaders).



**Open-source emphasis**: The self-hosted scheduling ecosystem has matured significantly. **Cal.com** is the flagship open-source Calendly alternative with 30k+ GitHub stars and enterprise-grade features . **Easy!Appointments** offers the lightest self-hosted option, running comfortably on a 1 GB VPS with just two containers . **Rallly** provides a focused Doodle-style group polling tool that handles the "when can everyone meet?" problem without accounts for participants . This section documents these production-grade solutions.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Calendly](https://calendly.com/)**

  The dominant scheduling platform with free tier for one event type. Connects to Google, Outlook, and Apple calendars. Paid plans start at $10/user/month for unlimited event types and workflows.



- **[Microsoft Bookings](https://www.microsoft.com/en-us/microsoft-365/business/scheduling-and-booking-app)**

  Scheduling tool integrated with Microsoft 365. Creates a booking page, syncs with Outlook calendars, and supports Teams meetings. Included with Microsoft 365 Business subscriptions.



- **[Acuity Scheduling](https://acuityscheduling.com/)**

  Scheduling platform popular with service businesses. Supports client self-scheduling, payments via Stripe/PayPal, and automated email/SMS reminders.



- **[YouCanBookMe](https://youcanbook.me/)**

  Booking page tool for teams. Provides custom booking forms, calendar sync, and Zapier integration for workflows.



- **[Doodle](https://doodle.com/)**

  Group scheduling pioneer. Creates polls to find common meeting times across participants without requiring accounts for voters.



- **[Setmore](https://www.setmore.com/)**

  Free appointment scheduling for small businesses. Supports booking pages, calendar sync, and staff management.



- **[Appointlet](https://www.appointlet.com/)**

  Scheduling tool with Salesforce, HubSpot, and Slack integrations. Focuses on sales teams and lead routing.



- **[SimplyBook.me](https://simplybook.me/)**

  Scheduling platform for service businesses with customizable booking sites and payment processing.



- **[Chili Piper](https://www.chilipiper.com/)**

  Scheduling and lead routing for revenue teams. Automatically qualifies leads and books meetings during conversion.



- **[HubSpot Meetings](https://www.hubspot.com/products/sales/meetings)**

  Meeting scheduling built into HubSpot CRM. Shares availability, syncs calendars, and logs meetings to contact records.



## Open-Source GitHub Projects



### Full-Featured Scheduling Platforms



- **[Cal.com](https://github.com/calcom/cal.com)**

  **The most complete open-source Calendly alternative.** **AGPLv3 licensed** (with enterprise features under commercial license), **30,000+ GitHub stars** . **Key features**: **Calendar sync** — Google, Outlook, CalDAV, Apple Calendar ; **Booking types** — one-on-one, round-robin, collective (all must attend), managed events ; **Workflows** — automated emails/SMS before and after meetings ; **Payments** — Stripe integration for paid consultations ; **Embedding** — embed booking widget on any website ; **REST API** for custom integrations ; **Team scheduling** — shared availability, routing, managed event types . **Resource requirements**: Node.js + PostgreSQL + Prisma, ~500 MB+ RAM . **Tradeoffs**: Complex Docker setup with multiple environment variables ; some integrations require external API keys; self-hosted may lag cloud on latest features . **Best for**: Professionals and businesses needing a full scheduling platform with feature parity to Calendly's paid tiers .



- **[Easy!Appointments](https://github.com/alextselegidis/easyappointments)**

  **The lightest self-hosted appointment scheduler, ideal for service businesses.** **GPLv3 licensed**, PHP + MySQL . **Key features**: **Service catalog** with durations and pricing ; **Provider availability** management ; **Customer self-booking** ; **Google Calendar bidirectional sync** ; **Email notifications** ; **Multi-provider support** ; **Customizable booking form fields** . **Resource requirements**: Apache/Nginx, PHP 8.2+, MySQL; **two containers** (app + MySQL) run comfortably on **1 GB VPS** . **Installation**: Use published Docker image `alextselegidis/easyappointments`; the repository's `docker-compose.yml` is a development environment requiring manual `npm install && composer install` . **Tradeoffs**: Google Calendar is the only calendar backend ; no workflow automation or payment integration in open-source version ; no team scheduling (round-robin, collective) ; limited API . **Best for**: Service businesses (clinics, salons, consultancies) needing online booking without complexity .



### Group Polling & Meeting Coordination



- **[Rallly](https://github.com/lukevella/rallly)**

  **The self-hosted Doodle alternative for group scheduling polls.** **AGPLv3 licensed** . **Key features**: **Create scheduling polls** with multiple date/time options ; **Share a link** — no account required for voters ; **See availability at a glance** ; **Finalize and notify** when a time is chosen ; **Guest comments** on polls . **Resource requirements**: **At least 2 GB RAM** ; Docker 19.03+ with Compose v2; ports 80 and 443 free; domain pointing to server . **Bundled stack**: Traefik (HTTPS), web application, PostgreSQL, and Garage (S3-compatible object storage) — **four containers** . **Configuration**: `DOMAIN`, `SECRET_PASSWORD` (32+ chars), `SUPPORT_EMAIL`, `INITIAL_ADMIN_EMAIL` . **Critical requirement**: **SMTP is not optional** — sign-in is via magic link; without working relay, nobody can log in . **Tradeoffs**: Only handles group scheduling polls, not booking pages ; no calendar integrations ; no recurring scheduling . **Best for**: Teams needing to coordinate meeting times among multiple people .



### Additional Strong Open-Source Options



- **Full Scheduling**: **Cal.com** (full Calendly replacement, 30k+ stars) .

- **Simple Booking**: **Easy!Appointments** (lightweight, 1 GB VPS, Google Calendar sync) .

- **Group Polling**: **Rallly** (Doodle alternative, no participant accounts) .

- **Resource Scheduling**: **LibreBooking** (flexible resource reservations) .

- **Event Ticketing**: **Hi.Events** (event management and ticketing) , **Alf.io** (ticket reservation system) .

- **Nextcloud Users**: **Nextcloud Appointments** (AGPLv3, integrates with Nextcloud Calendar) .

- **Helpdesk Integration**: **Zammad** includes calendar and appointment features within its helpdesk platform .



**Frameworks for building custom systems**: Combine **Cal.com** for a full-featured Calendly replacement with team scheduling and workflows, **Easy!Appointments** for lightweight service booking on minimal hardware, **Rallly** for group meeting polls, and **LibreBooking** for resource scheduling. For Nextcloud users, **Nextcloud Appointments** integrates directly with existing calendar infrastructure . Add **PostgreSQL** for Cal.com/Rallly persistence and **MySQL** for Easy!Appointments .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Scheduling platforms handle sensitive contact and calendar data; ensure compliance with GDPR, CCPA, and applicable data protection regulations.

- **Open-source reality**: The self-hosted scheduling ecosystem is **mature and production-proven**. **Cal.com** offers feature parity with Calendly's paid tiers, including workflows, team scheduling, and payment integration . **Easy!Appointments** runs on the lightest hardware of any option here — just two containers on a 1 GB VPS . **Rallly** provides a focused solution for group meeting coordination without requiring participant accounts . However, **commercial platforms** (Calendly, Acuity, Chili Piper) provide **managed infrastructure, deeper CRM integrations, and enterprise support** that open-source alternatives require additional configuration to match. The open-source path is **genuinely viable** for professionals and businesses wanting full control over their booking data.



---



**Made for consultants, service businesses, sales teams, and self-hosting enthusiasts.**

Let's make appointment scheduling more open, transparent, and self-hosted.

---
title: Privacy Policy
permalink: /privacy/
---

# Privacy Policy

**Last updated: 20 November 2026**

## 1. About this project

Personal Finance Aggregator is a personal project operated by Adam Walsh for his own financial overview. It is not offered as a public service to customers.

**Controller / operator:** Adam Walsh  
**Privacy contact:** walsha480@gmail.com

## 2. Current status

The backend infrastructure has been created, but the bank API credentials and account-authorisation flows have not yet been activated. As of the date above, this application has not retrieved or stored bank account data or transaction history, and automated synchronisation is not running.

The finance database is hosted in a Supabase project in Frankfurt, Germany (EU region). A server-side integration endpoint has been deployed, but it is not yet configured to retrieve financial data. The separate policy website is hosted by GitHub Pages. GitHub states that it logs and stores visitors' IP addresses for security purposes when a Pages site is visited, and may process other technical information as part of its hosting service. See [GitHub's Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-privacy-statement).

## 3. Intended use and data

When activated, the application is intended to bring together information from financial accounts chosen by the account holder.

Depending on the financial institution and the permissions granted, the application may process:
- account names, account identifiers returned by the provider, account type and currency;
- balances and balance timestamps;
- transaction amounts, currencies, descriptions, booking and value dates, and available counterparty or merchant details; and
- technical information needed to authorise sessions, refresh data, prevent duplicate imports and diagnose synchronisation errors.

The integration is designed for read-only account-information access (AIS). It is not designed to initiate payments, transfer funds, or change bank account settings.

## 4. Purposes

The intended purposes are to display a consolidated view of the account holder's own finances, review spending, reconcile transactions, and support personal budgeting and analysis. Data is not intended for advertising, sale, profiling of other people, or use by other users.

## 5. Financial institutions and service providers

The project is being built to use Enable Banking for account-information connectivity. Enable Banking acts as the intermediary for authorised account-information requests, and each connected bank or payment institution may separately process information under its own terms and privacy notices.

Supabase provides the project's database and server-side function hosting. The database is deployed in the Frankfurt, Germany EU region. GitHub Pages hosts this separate policy website. These providers process information under their own terms and privacy notices.

## 6. Sharing

The project does not intend to sell personal or financial information or share it for advertising. When operational, financial information may be processed by Enable Banking, the connected financial institutions and Supabase strictly as needed to provide the account-information service and operate the private database. Information may also be disclosed where required by law.

## 7. Storage, security and retention

No bank data is currently stored by this application. The project has a separate private database schema for connection metadata, accounts, balance snapshots, transactions and synchronisation records. Row-level security is enabled, and ordinary anonymous and authenticated client roles are not granted access to that schema. Bank API credentials have not yet been configured in the server-side environment, and no bank-data sync has been run.

The planned controls include keeping the Enable Banking private key and a separate administrative token in server-side secrets, using read-only account-information permissions, masking IBANs in account records, and avoiding retention of full raw API responses. These describe the current design and configuration; they are not a claim that every control has been independently audited or penetration-tested.

A fixed retention period, automated deletion workflow and backup-retention policy have not yet been finalised. Before live bank data is imported, these arrangements will be reviewed and this notice updated if they materially change.

## 8. Your choices and data protection rights

When account-information sessions are activated, the account holder can stop future access by revoking the relevant consent or session through Enable Banking or the financial institution, where supported. Revoking access does not necessarily delete data previously retrieved into the database.

A self-service deletion workflow for stored financial data has not yet been implemented. Requests about access, correction, deletion or other applicable data protection rights can be sent to the privacy contact above. Depending on applicable law and the circumstances, data protection rights may include access, correction, deletion, restriction, objection and data portability.

## 9. Changes

This notice will be revised when bank-data processing begins and when material changes are made. The date at the top indicates the latest revision.

---

This document describes a personal project in development. It does not represent that bank-data processing or automated synchronisation is already active.

---
title: Privacy Policy
permalink: /privacy/
---

# Privacy Policy

**Last updated: 21 November 2026**

## 1. About this project

Personal Finance Aggregator is a personal project operated by Adam Walsh for his own financial overview. It is not offered as a public service to customers.

**Controller / operator:** Adam Walsh  
**Privacy contact:** walsha480@gmail.com

## 2. Current status

Read-only account-information processing is now active for financial accounts authorised by the account holder. The current connections are for ING Netherlands, bunq and Revolut Ireland. The application has retrieved and stored account information, balance snapshots and transaction history for the account holder's connected accounts.

The current operating process supports manual synchronisation. A scheduled daily synchronisation has not yet been configured. Sync results can be partial if a bank, account-information provider or technical service is temporarily unavailable.

The finance database is hosted in a Supabase project in Frankfurt, Germany (EU region). Supabase also hosts the server-side integration function. Enable Banking is used for account-information connectivity. The separate policy website and static administration interface are hosted by GitHub Pages. The administration page's source code is public, but the page does not contain bank credentials or the administrative token. The token is entered by the operator, held in page memory for that visit, and sent directly to the Supabase endpoint over HTTPS; the page does not save it in browser storage.

GitHub states that it logs and stores visitors' IP addresses for security purposes when a Pages site is visited, and may process other technical information as part of its hosting service. See [GitHub's Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-privacy-statement).

## 3. Data processed

Depending on the information returned by the institution and the permissions granted, the application processes:
- account names, account identifiers and technical identifiers returned by the provider, account type and currency;
- masked account identifiers, such as partially masked IBANs;
- available balances, balance types and balance timestamps;
- transaction amounts, currencies, descriptions or remittance information, booking and value dates, transaction references, and available counterparty or merchant details; and
- connection and session metadata, consent-validity information, synchronisation timestamps, and technical error records needed to operate the service and prevent duplicate imports.

The database stores normalised account, balance and transaction records. It is not intended to retain complete raw API responses. The exact fields available can vary by bank and account.

The integration is designed for read-only account-information access (AIS). It is not designed to initiate payments, transfer funds, or change bank account settings.

## 4. Purposes

The purposes are to provide the account holder with a consolidated view of their own finances, review balances and spending, reconcile transactions, and support personal budgeting and analysis. Data is not intended for advertising, sale, or use by other users.

## 5. Financial institutions and service providers

The project uses Enable Banking for account-information connectivity. Enable Banking acts as the intermediary for authorised account-information requests, and each connected bank or payment institution may separately process information under its own terms and privacy notices.

Supabase provides the private database and server-side function hosting. The database is deployed in the Frankfurt, Germany EU region. GitHub Pages serves the static administration interface and this policy website. The administration page calls the Supabase endpoint directly; bank records are not stored in the GitHub repository. These providers process technical or financial information as needed to provide and operate the service, under their own terms and privacy notices.

## 6. Sharing

The project does not sell personal or financial information or share it for advertising. Financial information is processed by Enable Banking, the connected financial institutions and Supabase as needed to provide the account-information service and operate the private database. GitHub Pages hosts the static interface and policy pages and may process visitor technical information as described above. Information may also be disclosed where required by law.

## 7. Storage, security and retention

Retrieved account, balance and transaction information is stored in a private `finance` schema in the Supabase database in Frankfurt, Germany. Row-level security is enabled on the finance tables, and ordinary anonymous and authenticated client roles are not granted access to that schema. The browser-based administration page accesses the server-side endpoint using a separate administrative token; that token is not embedded in the public page source or saved in browser storage.

The Enable Banking signing key and administrative credentials are kept in server-side Supabase secrets / Vault rather than in the public GitHub repository. Account identifiers are masked for display where applicable. The integration is designed to use read-only account-information permissions and to store normalised records rather than full raw provider responses.

These are implemented technical controls, not a claim that the system has undergone an independent security audit or penetration test.

A fixed retention period, automated deletion workflow and backup-retention policy have not yet been finalised. There is currently no self-service deletion control. Revoking an account-information consent or session stops or limits future access where supported; it does not automatically delete information already imported into the database. Stored data must be deleted separately.

## 8. Your choices and data protection rights

The account holder can stop future access by revoking the relevant consent or session through Enable Banking or the financial institution, where supported. Revoking access does not delete data already retrieved into the database.

Requests about access, correction, deletion or other applicable data protection rights can be sent to the privacy contact above. Depending on applicable law and the circumstances, data protection rights may include access, correction, deletion, restriction, objection and data portability. Requests for deletion currently require manual handling; an automated deletion workflow has not yet been implemented.

## 9. Changes

This notice will be revised when material changes are made to the data processed, providers, purposes or technical arrangements. The date at the top indicates the latest revision.

---

This document describes the current operation of a personal project. It is not a substitute for the separate privacy notices of the banks, Enable Banking, Supabase or GitHub.

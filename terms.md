---
title: Terms of Use
permalink: /terms/
---

# Terms of Use

**Last updated: 21 November 2026**

## 1. About the project

Personal Finance Aggregator is a personal project operated by Adam Walsh to view and analyse his own financial-account information. It is not offered as a public service to customers.

## 2. Current status

The account-information integration is operational for the account holder's authorised accounts at ING Netherlands, bunq and Revolut Ireland. It retrieves account details, balances and transaction history using read-only account-information access (AIS).

Manual synchronisation is available, and a daily scheduled synchronisation is configured for 03:00 UTC. The first scheduled execution has not yet been observed, and scheduled runs should be monitored for failures. Features, supported institutions and availability may change. Synchronisation can be delayed, incomplete or partially unsuccessful because of bank, provider or technical limitations.

## 3. Intended use

The intended use is personal financial organisation and analysis by the account holder. You must not use the project to access accounts or data without authorisation, or to violate any law or another person's rights.

The integration is designed for read-only account-information permissions. It is not designed to make payments, transfer funds, place orders, or alter information held by a bank.

## 4. No financial, tax or legal advice

Information displayed by the project is provided for personal information and organisational purposes only. It is not financial, investment, tax, accounting or legal advice, and is not a recommendation to make any financial decision. You remain responsible for checking information against your bank's own records and obtaining qualified advice where appropriate.

## 5. Accuracy and availability

No guarantee is made that information will be complete, current, accurate, available at any particular time, or synchronised without delay or error. A bank or account-information provider may restrict, change or discontinue access. A successful synchronisation does not guarantee that every institution has supplied all information available for an account or period.

Do not rely on the project as the sole record of account balances, transactions, payment obligations or financial position. The relevant bank's own records remain the authoritative source for its accounts.

## 6. Third-party services

The project uses Enable Banking for account-information connectivity and Supabase for the private database and server-side hosting. GitHub Pages hosts the static administration interface and policy website. Use of these services, banks and other providers may be subject to their separate terms and privacy notices. The project operator does not control the availability or operation of those services.

## 7. Security, access and data handling

The project is designed for private use and read-only account-information access. Do not share access tokens, credentials, the Enable Banking private key, administrative tokens, or financial information publicly. Server-side credentials are stored in Supabase secrets / Vault and are not included in the public GitHub Pages source. The finance database is in the Frankfurt, Germany EU region and access is restricted to the server-side integration.

The developing system has not undergone an independent security audit or penetration test. A fixed data-retention period and automated deletion workflow have not yet been implemented. Revoking bank consent stops or limits future access where supported but does not automatically remove data previously imported into the database.

## 8. Changes and discontinuation

The project may be changed, suspended or discontinued. These terms may also be updated; the revision date above will be changed when they are.

## 9. Mandatory law

These terms do not limit rights or remedies that cannot lawfully be excluded or restricted under applicable mandatory law.

## 10. Contact

For questions about these terms, contact the project operator using the privacy contact details in the project's privacy policy.

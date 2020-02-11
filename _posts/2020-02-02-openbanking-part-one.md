---
title: "Open Banking Explained - Part 1"
layout: single
date: "2020-02-11"
permalink: /open-banking-explained-part-one/
tags: [security, open banking]
excerpt: "Security, Open Banking"
classes: wide
header:
  overlay_color: "#333"
---

# Open Banking Explained - Part One

## What is Open Banking?

<p class="text-justify">Open Banking is a set of rules which objective is to standardize the access to the financial APIs provided by banks to third party providers. It is a subset of the Payments Services Directive (PSD2) which was created to regulate and open the access to banking data.</p>

<p class="text-justify">Currently, Open Banking is only implemented by UK banks (such as Barclays, Bank of Ireland, Royal Bank of Scotland, etc.).</p>

<p class="text-justify">Previously, before Open Banking was implemented, any mobile application that offered statistics about where you spent your money and aggregated several of your bank accounts would ask for your credentials to be inputted directly. After Open Banking was implemented, the applications that are verified as trusted third parties redirect users to an specific bank login portal and after the user logs in successfully, the application gets a token to access the user's data for a set period of time.</p>

![Open Banking Schema](/assets/images/02-02-2020/ob-token-process.png)
*Source: https://blog.truelayer.com/scas-not-too-far-away-switch-to-ob-now-33d8b3693af5*

<p class="text-justify">Keep in mind that the Open Banking ecosystem is still under development and new revisions are released every other month with changes based on the bank community feedback.</p>

## Actors involved

<p class="text-justify">There are several actors involved in the Open Banking ecosystem and each one has been given a specific name. The most important ones are the following:</p>

- **PSU: Payment Services User**
  - A natural or legal person making use of payment services as a payee, payer or both.
  - In simplified terms: Clients
- **ASPSP: Account Servicing Payment Service Provider**
  - Provide and maintain a payment account for a payer. These are entities that publish Read/Write APIs to permit, with customer consent, payment initiated by third party providers or make their customers' account transactions data available.
  - In simplified terms: Banks
- **TPP: Third Party Provider**
  - Organisations or natural persons that use APIs developed to access customer's accounts, in order to provide account information services and/or to initiate payments.
  - TPPs can be AISPs and/or PISPs.
- **AISP: Account Information Service Provider**
  - Provides account information services on one or more payment accounts held by a PSU with one or more PSP.
  - For example: Account aggregators like Fintonic.
- **PISP: Payment Initiation Services Provider**
  - Provides an online service to initiate a payment order at the request of the PSU with respect to a payment account held at another payment service provider.
  - For example: Transferwise, Paysera, etc.
- **CBPII: Card Based Payment Instrument Issuer**
  - Payment Services Provider that issues card-based payment instruments that can be used to initiate a payment transaction from a payment account hold with another payment service provider.
  - For example: Monzo, Revolut, etc. 

## In the next post...

In the next post of the **Open Banking Explained** series, I will describe the different user journeys that are implemented at the moment.
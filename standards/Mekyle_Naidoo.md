---
EIP: 948
Title: ERC-948 - A Standard For Subscriptions
Author: Mekyle Logen Naidoo
Yype: Standards Track
Category: ERC
Status: Draft
Created: 2018-06-19
---

## Simple Summary

A standard method to accept timed recurring payments.

## Abstract

This standard helps merchants to accept recurring timed payments from customers using smart contracts.

This standard will help initiate a timed transaction that will recur until a subscriber cancels. The contract has three main functions, the first is to initiate a timed transaction. The second is to manage transactions, with this users can identify merchants and merchants can identify subscribers, this allows both a subscriber and a merchant to block each other if need be and manage their balance. The third is to pause or cancel a subscription. Merchants will set the recurring time, for example, the first of every month. Subscribers can accept these terms and the transaction will recur until they cancel or pause their subscription.

We aim to standardize the following:

1. Approve recurring transactions.
2.

## Motivation

Currently there is no way to "Subscribe" to a merchant with crypto-currency. This creates problems for the future as users cannot create an automated subscription to get a product or service and have the payment for said product or service automatically be sent every term. This leads to negatives for merchants as well as users. Merchants can benefit from the continuous payments as a stable source of income as well as help make the barrier of entry (Price) for a product or service lower due to a user not owning said service or product but renting it as long as the subscription is active. For users the benefit is a reduced price, instead of one large lump sum payment, users can test out the full product at an affordable rate.

Subscriptions as an alternative to ICO's. Currently in the industry ICO's are the standard for generating enough funding to develop their projects but this has many problems. While ICO's allow companies to generate a huge amounts of funding at once, it isn't a stable source of income and due to the nature of crypto-currencies value not being stable it creates many issues in the long term. Subscriptions solve this by giving developers and companies a sustainable long term income, this allows companies and developers to overcome the problem with getting long term support for their development.

## Specification

## Definitions
Merchant: Users that accept funds for a product and/or service.
Subscriber: A user that pays for a product and/or service.

## Features

1. The ability to approve a subscription to a specific address for a specific amount.
2.

## Methods

deposit

This is called by the subscriber/developer to send funds to the contract.

* Makes the sender of the funds the owner of the contract.

Struct DateNow

* @param currentYear : Gets the current year from the timestamp and converts it to the current year.
* @param currentMonth : Gets the current month from the timestamp and converts it to the current month.
* @param currentDay : Gets the current day from the timestamp and converts it to the current day.

Struct PaymentDate

* @param nextYear : Gets the current year and adds one to it to get the next year.
* @param nextMonth : Gets the current month and adds one to it to get the next year.
* @param nextDay :

Struct SubscriptionInfo

* @param merchant : Gets the merchants address and stores it in an array.
* @param price : Gets the static recurring payment price and stores in an array.
* @param periodType : Gets the uint period type, 1 = Yearly payment, 2 = Monthly payment, 3 = Daily payment.
* @param currentDate : Gets the current year, month and day from the timestamp and returns it in a human readable format "YYYYMMDD".
* @param nextPaymentDate :

* @param subContractActive : Checks if the 

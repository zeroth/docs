---
title: Connect Apps to Dwolla
connection: Dwolla
image: /media/connections/dwolla.png
seo_alias: dwolla
description: Learn how to add login functionality to your app with Dwolla. You will need to obtain a Client Id and Client Secret for Dwolla.
toc: true
index: 9
topics:
  - connections
  - social
  - dwolla
contentType: how-to
useCase:
    - customize-connections
    - add-idp
---

# Connect Apps to Dwolla

You can add functionality to your web app that allows your users to log in with Dwolla. 

## Prerequisites

Before you connect your Auth0 app to Dwolla, you must have a [Dwolla Developer](https://accounts-sandbox.dwolla.com/login) account.

## Steps

To connect your app to Dwolla, you will:

1. [Set up your app in Dwolla](#set-up-your-app-in-dwolla)
2. [Create and enable a connection in Auth0](#create-and-enable-a-connection-in-auth0)
3. [Test the connection](#test-the-connection)

### Set up your app in Dwolla

Set up an app in Dwolla using Dwolla's [OAuth: Creating an Application](https://developers.dwolla.com/guides/auth#creating-an-application) doc. During this process, Dwolla will generate a **Key** and **Secret** for your application; make note of these.

While setting up your app, make sure you use the following settings:

| Field | Value to Provide |
| - | - |
| OAuth Redirect URL | `https://${account.namespace}/login/callback` |

<%= include('../_find-auth0-domain-redirects') %>

### Create and enable a connection in Auth0

[Set up the Dwolla social connection](/dashboard/guides/connections/set-up-connections-social) in Auth0. Make sure you have the generated **Key** and **Secret**.

### Test the connection

You're ready to [test your connection](/dashboard/guides/connections/test-connections-social). After logging in, you'll be prompted to allow your app access. To do so, click **Install unlisted app**.

<%= include('../_quickstart-links.md') %>
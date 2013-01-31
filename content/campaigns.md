---
title: Campaigns
---

The Campaigns API allows you to list and view campaigns.

* TOC
{:toc}

## List all Campaigns

    GET /campaigns

### Visibility

Public.

### Parameters

charity_id
: _Optional_ **string**. Retrieve only the campaigns that the specified
charity is participating in.

### Response

<%= json :campaigns %>

## View a single Campaign

    GET /campaigns/:id

### Visibility

Public.

### Response

<%= json :campaign %>
---
title: Registration Integration
---

Through the API we allow campaign builders to extend the functionality
of the everydayhero platform. We do this by allowing your chosen
registration solution to hook into the supporter page creation process.

## How Does it Work?

The everydayhero platform supports two kinds of supporter pages:
[Individuals pages](/glossary/) and [Team
pages](/overview#glossary/). In order to create an Individual Page
through the API you will be required to authenticate the user through
the everydayhero [Giving Passport](/oauth-integration/#how-to-authenticate-with-edh-passport) and store the
returned `uid` - this `uid` is our way of tracking that user within our
platform and yours.

Once you have a `uid` you will be able to [Create an Individual
Page](/pages#create-an-individual-page) for your campaign.

## Registering for Third Party Integration

Please email
[professionalservices@everydayhero.com.au](mailto:professionalservices@everydayhero.com.au), you will be
asked to provide two registration urls, one for individuals and one for
teams. These are used by the everydayhero platform to redirect to the
third party before creating a supporter page.

## Primary Registrant

[Create an Individual Page](/pages#create-an-individual-page)

## Secondary Registrants

[Create Individual Page
Invitation](/invitations#create-individual-page-invitation)

## Team Page Creation

[Create an Individual Page](/pages#create-an-individual-page)

[Create a Team](/teams#create-a-team)

## Joining an Exising Team

[Create Join a Team
Invitation](/invitations#create-join-a-team-invitation)

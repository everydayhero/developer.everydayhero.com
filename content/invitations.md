---
title: Invitations
body_id: page_teams
---
## Create Individual Page Invitation

<p class='info'><strong>Authentication types</strong>: Registered Application Token</p>

Send an invitation to create an individual supporter page to an email
address.

    POST https://everydayhero.com/api/v2/individual-pages/invitations

### Payload

email : _required_ **string**<br/>
The email address you would like the invitation sent to. We do not tie this email address to the user's EDH account in any way, it is only used to deliver the invitation.

phone : _optional_ **string**<br/>
The phone number of the person you want to invite to create a supporter page.

full_name : _optional_ **string**<br/>
The full name of the person you want to invite to create a supporter page.

charity_id : _optional_ **string**<br/>
The `id` of the charity that you want set for this supporter page. If no charity is supplied the user will be prompted to select a charity. Defaults to none.

target : _optional_ **decimal**<br/>
The amount of money this page is aiming to raise. Defaults to a predetermined value.

### Example

<%= json \
  email: 'api@everydayhero.com',
  phone: '1300798768',
  full_name: 'everydayhero Support',
  charity_id: 'au-1',
  target: 705.5
%>

### Response

<%= json :create_individual_page_invitation %>

## Create Join a Team Invitation

<p class='info'><strong>Authentication types</strong>: Registered Application Token</p>

Send an invitation to create an individual supporter page for a team to
an email address.

    POST https://everydayhero.com/api/v2/team-pages/:team_page_id/invitations

### Payload

email : _required_ **string**<br/>
The email address you would like the invitation sent to. We do not tie this email address to the user's EDH account in any way, it is only used to deliver the invitation.

full_name : _optional_ **string**<br/>
The full name of the person you want to invite to create a supporter page.

charity_id : _optional_ **string**<br/>
The `id` of the charity that you want set for this supporter page. If no charity is supplied the user will be prompted to select a charity. Defaults to none.

target : _optional_ **decimal**<br/>
The amount of money this page is aiming to raise. Defaults to a predetermined value.

### Example

<%= json \
  email: 'api@everydayhero.com',
  full_name: 'everydayhero Support',
  charity_id: 'au-1',
  target: 705.5
%>

### Response

<%= json :join_team_invitation %>

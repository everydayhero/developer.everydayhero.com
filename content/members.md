---
title: Members
body_id: page_teams
---
## Add a Team Member

<p class='info'><strong>Authentication types</strong>: Registered Application Token or OAuth User Token</p>

Add an existing page to an existing team.

    POST https://everydayhero.com/api/v2/teams/:id/members

### Payload

individual_page_id : _required_ **integer**<br/>
The `id` of the page you want to join a team with.

<p class='info'>If using Registered Application authentication, any team in the application's campaign can be used. If using OAuth User authentication the affiliated user must own the team.</p>

### Example

<%= json \
  individual_page_id: 1
%>

### Response

<%= json :team %>

## Remove a Team Member <small>(requires authentication)</small>

Remove a member from an existing team, the leader can not be the team leader.
The page id must be a member of a campaign you are authenticated with.

    DELETE https://everydayhero.com/api/v2/teams/:team_id/members/:page_id

### Response

`204` no content, for success

`404` for invalid team or page

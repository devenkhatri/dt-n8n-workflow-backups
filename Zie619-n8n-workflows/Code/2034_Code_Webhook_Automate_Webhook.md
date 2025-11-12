# Workflow Analysis for OIDC client workflow

## Description
This workflow implements an OpenID Connect (OIDC) client that handles user authentication via an identity provider. It supports both PKCE and non-PKCE flows, retrieves user information after login, and displays either a welcome page with the user's email or a login form if the user is not authenticated.

## Input Details
The workflow is triggered by an HTTP webhook request, which may include query parameters (like an authorization code) and cookies (like an access token).

## Process Summary
The workflow starts by receiving a webhook request. It parses cookies to check for an existing access token. If no token is present but an authorization code exists (and PKCE is disabled), it exchanges the code for an access token using the identity provider’s token endpoint. If a valid access token is available, it fetches user info from the userinfo endpoint. Based on whether user info (specifically email) is successfully retrieved, it either returns a welcome page with the user's email or serves a login form that initiates the OIDC authorization flow using configured identity provider endpoints and client credentials.

## Output Details
The workflow returns an HTML response to the original webhook request—either a welcome page for authenticated users or a login form for unauthenticated users.

## Tags
OIDC, authentication, identity provider, OAuth2, PKCE, login flow, HTML response, webhook, userinfo, access token

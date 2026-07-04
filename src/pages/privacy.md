---
layout: ../layouts/MarkdownLayout.astro
---
[← back](/)

# Privacy Policy

_Last updated: 04.07.2026_

This site (`girnghuber.dev`) and the services hosted under it are operated privately by Patrick Girnghuber. This page describes what data is processed when you interact with them.

## Hosting and infrastructure

The static website is hosted on a virtual server provided by Hetzner Online GmbH (Industriestr. 25, 91710 Gunzenhausen, Germany), located in a data center in Helsinki, Finland, within the European Economic Area (EEA).

The Matrix homeserver and the web-based chat clients run on self-hosted hardware operated privately by Patrick Girnghuber. They are made reachable from the internet through the Hetzner server, which acts only as an **encrypted relay**: traffic is forwarded to the home server over an encrypted tunnel and is **not decrypted, inspected, or stored in content form** by the relay. TLS is terminated on the home server, which means the hosting provider cannot read the content of your connections to the Matrix homeserver or the chat clients. The relay may process connection metadata (such as IP addresses and timing) at the network level solely in order to forward traffic.

## Static website (girnghuber.dev)

The site is a static page. No cookies, no analytics, no third-party trackers. The webserver does not record per-request access logs. Only error-level events (e.g. failed requests, server errors) are logged for troubleshooting purposes and retained for up to 30 days. These logs may incidentally contain IP addresses associated with connection failures.

## Matrix homeserver (matrix.girnghuber.dev)

The Matrix homeserver runs [Synapse](https://element-hq.github.io/synapse/) on self-hosted hardware (see “Hosting and infrastructure” above). When you have an account here or communicate with users on this server, the following is processed:

- **Account data:** username, hashed password, display name, avatar, devices, and encryption keys.
- **Messages and media:** end-to-end encrypted messages are stored in encrypted form; unencrypted messages (e.g. in public rooms) are stored as-is. Media files you send or receive are cached on the server.
- **Server logs:** connection logs containing IP addresses, timestamps, and API endpoints. Retained up to 30 days.
- **Federation:** Matrix is a federated protocol. When you participate in rooms with users on other homeservers, your messages, profile, and presence are transmitted to those servers, which are operated by independent third parties under their own privacy policies. Once shared via federation, data cannot be recalled.

## Chat client (chat.girnghuber.dev)

The chat client (Cinny) is a static web application served from this domain. It stores your session, encryption keys, and preferences in your browser's local storage. No data is transmitted to this site beyond what is needed to load the client; all chat traffic goes directly from your browser to the Matrix homeserver.

## Chat client (element.girnghuber.dev)

The chat client (Element) is a static web application served from this domain. It stores your session, encryption keys, and preferences in your browser's local storage. No data is transmitted to this site beyond what is needed to load the client; all chat traffic goes directly from your browser to the Matrix homeserver.

## Identity server

This deployment does not operate its own identity server. If you choose to add an email address or phone number to your Matrix account, your client may publish a hashed mapping to a third-party identity server (by default `vector.im`, operated by Element). You can disable this in your client settings.

## Backups

Encrypted backups of the homeserver database are retained for up to 14 days before being overwritten. Data within the backup retention window may persist after deletion from the live system.

## Domain name resolution (Cloudflare)

Authoritative DNS for `girnghuber.dev` and its subdomains is provided by Cloudflare, Inc. (101 Townsend Street, San Francisco, CA 94107, USA), acting solely as a DNS provider. Cloudflare is configured in **DNS-only mode**: traffic to this site and its services is not proxied through Cloudflare's network, and Cloudflare does not terminate TLS, inspect, cache, or route your connections. Cloudflare processes only the DNS queries necessary to resolve the domain. Such queries may be handled on servers outside the EEA, including in the United States. More information: https://www.cloudflare.com/privacypolicy/.

## International data transfers

The website, the relay, and the homeserver are all hosted within the European Economic Area (Finland and Germany). Some third parties may nonetheless process data outside the EEA — in particular Cloudflare (DNS resolution), any identity server you opt into, and any federated homeservers you communicate with. Where such transfers occur, they rely on appropriate safeguards such as the EU-U.S. Data Privacy Framework and Standard Contractual Clauses, as applicable.

## Your rights

You may request access to, correction of, or deletion of your account and data at any time by contacting [hello@girnghuber.dev](mailto:hello@girnghuber.dev). Note that messages already federated to other homeservers cannot be deleted from those servers by this site's operator. Under the GDPR you also have the right to lodge a complaint with your local data protection authority.

## Contact

Patrick Girnghuber  
Address available on request via email  
[admin@girnghuber.dev](mailto:admin@girnghuber.dev)

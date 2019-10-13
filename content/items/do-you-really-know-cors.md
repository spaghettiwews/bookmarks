---
title: "Do you really know CORS?"
date: 2019-10-12T11:10:45+02:00
itemurl: "http://performantcode.com/web/do-you-really-know-cors"
sites: "performantcode.com"
tags: ["cors","sop","frontend"]
draft: false
---

## Same Origin Policy & CORS

- SOP prevents documents or scripts loaded from one origin (e.g. a domain) to access resources from other origins
- for all requests, browsers always and automatically attach any cookies bounded for the destination domain.
- exceptions - img, script, iframe. why? tags are in the the control of the browser whereas javascript is in full control and as such a AJAX call is potentially more dangerous.
- two origins are equal if they have the same protocol, host, and port. known as the "scheme/host/port" tuple
- CORS is not a security mechanism but a way to relax security. makes it possible to access resources from foreign origins
- SOP doesn’t apply to server-to-server communication, only to browser-to-server comms. Because of this you can use a proxy server to circumvent the SOP protections
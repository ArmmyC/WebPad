<!-- prettier-ignore -->
<div align="center">
  <img src="https://freedomain.kamolpop.dev/brand/webpad-mark-v2.png" alt="WebPad mark" width="96" height="96" />

  <h1>WebPad</h1>
  <p><strong>Your place, free on the web.</strong></p>
  <p>A calm DNS-only control plane for memorable, shareable web namespaces.</p>

  <p>
    <a href="https://freedomain.kamolpop.dev/"><strong>Live site</strong></a>
    &middot;
    <a href="#overview">Overview</a>
    &middot;
    <a href="#how-it-works">How it works</a>
    &middot;
    <a href="#resources">Resources</a>
  </p>

  <p>
    <a href="https://freedomain.kamolpop.dev/"><img src="https://img.shields.io/website?url=https%3A%2F%2Ffreedomain.kamolpop.dev&label=live%20website&style=flat-square" alt="Live website" /></a>
    <img src="https://img.shields.io/badge/DNS--only-control%20plane-635bff?style=flat-square" alt="DNS-only control plane" />
    <img src="https://img.shields.io/badge/Next.js-App%20Router-20242c?style=flat-square" alt="Next.js App Router" />
  </p>
</div>

WebPad gives people a memorable address under `webpad.page`, a clear place to manage DNS records, and a safer path to connect that address to the hosting platform they already trust.

> [!IMPORTANT]
> WebPad manages namespace ownership and DNS records. It does not host website files, provide website hosting, issue destination certificates, or guarantee that a destination platform recognizes and serves a hostname.

## Overview

WebPad is designed for students, hobbyists, and small projects that need a simple web address without taking on a hosting platform.

| WebPad helps you | What that means |
| --- | --- |
| Choose an address | Claim a memorable namespace such as `yourname.webpad.page`. |
| Manage DNS | Add the records your destination platform provides. |
| Connect a destination | Point the namespace to an HTTPS-capable platform or server. |
| Stay in control | Review lifecycle state, quota, and safe account activity in one place. |

The interface is designed to be calm and understandable on both mobile and desktop. DNS-only means the control plane stays focused: your hosting platform remains responsible for serving the site.

## How it works

1. **Choose a namespace.** Create an account and claim an available `webpad.page` address.
2. **Copy the destination records.** Use the A, AAAA, CNAME, or TXT values provided by the platform hosting your site.
3. **Add the records in WebPad.** Keep the relative name, value, and TTL aligned with the destination instructions.
4. **Connect the address at your platform.** Add the full hostname to Vercel, Cloudflare Pages, GitHub Pages, or another HTTPS-capable destination.
5. **Allow time for readiness.** DNS propagation and HTTPS/site readiness are separate states. A valid DNS record alone does not prove that the destination recognizes the hostname.

## Product boundaries

- WebPad manages the namespace and its DNS control plane.
- Your platform serves the website files and application.
- Your platform or server is responsible for certificate setup for the exact hostname.
- DNS records stored by a mock-backed environment are not publicly resolvable.
- Reports submitted through the public safety form are reviewed by administrators; anonymous reports never suspend a namespace automatically.
- The public repository contains project documentation and community guidance. Application implementation and operational deployment configuration are maintained separately.

## Safety and privacy

WebPad keeps protected operations server-authorized and treats browser input as untrusted. The public product does not expose provider credentials, internal database controls, or raw operational state.

When reporting a safety issue, include only the information needed to describe the hostname and concern. Never post passwords, API tokens, private keys, verification codes, or personal data in a public issue.

## Resources

- [WebPad live site](https://freedomain.kamolpop.dev/)
- [Sitemap](https://freedomain.kamolpop.dev/sitemap.xml)
- [Robots](https://freedomain.kamolpop.dev/robots.txt)
- [AI-readable product summary](https://freedomain.kamolpop.dev/llms.txt)
- [Public issue tracker](https://github.com/ArmmyC/WebPad/issues)

## License

Original documentation, community guidance, and repository configuration are available under [CC BY 4.0](./LICENSE). See [NOTICE](./NOTICE) for the scope of that license.

Built for people who want a clear address and a hosting platform they can trust.

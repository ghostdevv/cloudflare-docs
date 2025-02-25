---
title: Limitations
pcx_content_type: reference
weight: 5
meta:
  title: Limitations for Universal SSL
---

# Limitations for Universal SSL

Universal SSL certificates are limited by the hostnames they cover and the browsers they support.

## Hostname coverage

### Full setup

Universal SSL certificates only support SSL for the root or first-level subdomains such as `example.com` and `www.example.com`. To enable SSL support on second, third, and fourth-level subdomains such as `dev.www.example.com` or `app3.dev.www.example.com`, you can:

- Purchase [Advanced Certificate Manager](/ssl/edge-certificates/advanced-certificate-manager/) to order advanced certificates.
- Upgrade to a Business or Enterprise plan to [upload custom certificates](/ssl/edge-certificates/custom-certificates/).

### CNAME setup

On a CNAME setup zone, each subdomain has its own Universal SSL certificate and does not require additional features or purchases.

## Browser support

For more on browser support, see [Browser compatibility](/ssl/reference/browser-compatibility/).

## Spectrum

Universal SSL is not compatible with [Cloudflare Spectrum](/spectrum/). If you are trying to use Spectrum, use either [an advanced certificate](/ssl/edge-certificates/advanced-certificate-manager/) or [a custom certificate](/ssl/edge-certificates/custom-certificates/).

## Certificate authority

For Universal SSL certificates, Cloudflare chooses the {{<glossary-tooltip term_id="Certificate Authority (CA)">}}certificate authority (CA){{</glossary-tooltip>}} used for your certificate.

Cloudflare can change the [certificate authority](/ssl/reference/certificate-authorities/) without prior notification, and will not send any notification as the change happens.

If you want to choose the issuing certificate authority, [order an advanced certificate](/ssl/edge-certificates/advanced-certificate-manager/).

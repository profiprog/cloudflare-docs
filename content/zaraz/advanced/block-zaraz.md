---
pcx-content-type: how-to
title: Block Zaraz
weight: 0
meta:
  title: Block Zaraz on specific pages or domains
---

# Block Zaraz on specific pages or domains

You can use Cloudflare Page Rules to prevent Zaraz from loading on specific URLs of your website. This can be useful if you want to block Zaraz from loading on the admin URL of your website, for example.

1. Log in to the [Cloudflare dashboard](https://dash.cloudflare.com/login), and select your account and website.
2. Go to **Rules**.
3. Click **Create Page Rule**.
4. Create a URL pattern that matches the page, domain or subdomain you want to exclude Zaraz from loading on.
5. Choose _Disable Zaraz_ from the **Then the settings are** dropdown menu.
6. Click **Save and deploy**.

Refer to [Understanding and configuring Cloudflare Page Rules](https://support.cloudflare.com/hc/articles/218411427) for more information about how Page Rules work.

{{<Aside type="note">}}

If you need to block just one or more events from firing in a tool, we recommend you use [Blocking Triggers](/zaraz/get-started/create-trigger/#blocking-triggers).

{{</Aside>}}
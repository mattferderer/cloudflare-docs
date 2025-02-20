---
title: Flow-based monitoring
pcx-content-type: how-to
weight: 0
---

# Flow-based monitoring

Flow-based monitoring works with [Magic Transit on demand](/magic-transit/on-demand/) to detect and notify you about attacks based on traffic flows from your data centers. You can configure your routers to continuously send NetFlow data to Cloudflare where the flow data is ingested and analyzed for volumetric DDoS attacks. When an attack is detected, Cloudflare automatically notifies you by email, [webhook](/fundamentals/notifications/create-notifications/configure-webhooks), or [PagerDuty](/fundamentals/notifications/create-notifications/create-pagerduty) with information about the attack.

You can choose to activate IP advertisement via the Cloudflare dashboard or API. After Magic Transit is activated and your traffic is flowing through Cloudflare, you only receive the clean traffic back to your network over your GRE tunnels.

To activate IP advertisement via the Cloudflare dashboard, refer to [​using the IP Prefixes page to configure dynamic advertisement](/byoip/dynamic-advertisement/configure-dynamic-advertisement#use-the-ip-prefixes-page-to-configure-dynamic-advertisement).

To activate IP advertisement via the API, refer to the [IP Address Management Dynamic Advertisement API](https://api.cloudflare.com/#ip-address-management-dynamic-advertisement-properties).

## Enable Flow-based monitoring alerts

1.  Log in to your [Cloudflare dashboard](https://dash.cloudflare.com/login) and select **Notifications**.
2.  From **Notifications**, click **Add**.
3.  Locate **Magic Transit** in the list and click **Select** to add a Flow-based Monitoring: Volumetric Attack notification.
4.  Enter a name and description for the notification.
5.  Add an email address for the person who should receive the notification.
6.  Click **Create** when you are done.

For more information on receiving notifications via PagerDuty or using webhooks, refer to [create a notification](/fundamentals/notifications/create-notifications).

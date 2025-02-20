---
'[ // ]': null
title: Firewall events
---

# Firewall events

The descriptions below detail the fields available for `firewall_events`.

{{<table-wrap>}}

| Field                  | Value                                                                                                                                                                     | Type             |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | --------------------- | ------------------ | -------------------------- | ---------------------- | ------------------------ | ------------------------ | ------------------------ | -------------------------- | -------------------------- | -------------------------- | ---------------------------- | --------------- | ------------------------- | -------------------------------- | --------------------------------------------- | ------------------------------------------ | --------------------------------- | ------------------------ | ----------------------- | ------ |
| Action                 | The code of the first-class action the Cloudflare Firewall took on this request. <br />Possible actions are <em>unknown</em>                                              | <em>allow</em>   | <em>block</em>        | <em>challenge</em> | <em>jschallenge</em>       | <em>log</em>           | <em>connectionclose</em> | <em>challengesolved</em> | <em>challengefailed</em> | <em>challengebypassed</em> | <em>jschallengesolved</em> | <em>jschallengefailed</em> | <em>jschallengebypassed</em> | <em>bypass</em> | <em>managedchallenge</em> | <em>managedchallengeskipped</em> | <em>managedchallengenoninteractivesolved</em> | <em>managedchallengeinteractivesolved</em> | <em>managedchallengebypassed</em> | string                   |
| ClientASN              | The ASN number of the visitor                                                                                                                                             | int              |
| ClientASNDescription   | The ASN of the visitor as string                                                                                                                                          | string           |
| ClientCountry          | Country from which request originated                                                                                                                                     | string           |
| ClientIP               | The visitor's IP address (IPv4 or IPv6)                                                                                                                                   | string           |
| ClientIPClass          | The classification of the visitor's IP address, possible values are: <em>unknown</em>                                                                                     | <em>badHost</em> | <em>searchEngine</em> | <em>allowlist</em> | <em>monitoringService</em> | <em>noRecord</em>      | <em>scan</em>            | <em>tor</em>             | string                   |
| ClientRefererHost      | The referer host                                                                                                                                                          | string           |
| ClientRefererPath      | The referer path requested by visitor                                                                                                                                     | string           |
| ClientRefererQuery     | The referer query-string was requested by the visitor                                                                                                                     | string           |
| ClientRefererScheme    | The referer URL scheme requested by the visitor                                                                                                                           | string           |
| ClientRequestHost      | The HTTP hostname requested by the visitor                                                                                                                                | string           |
| ClientRequestMethod    | The HTTP method used by the visitor                                                                                                                                       | string           |
| ClientRequestPath      | The path requested by visitor                                                                                                                                             | string           |
| ClientRequestProtocol  | The version of HTTP protocol requested by the visitor                                                                                                                     | string           |
| ClientRequestQuery     | The query-string was requested by the visitor                                                                                                                             | string           |
| ClientRequestScheme    | The URL scheme requested by the visitor                                                                                                                                   | string           |
| ClientRequestUserAgent | Visitor's user-agent string                                                                                                                                               | string           |
| Datetime               | The date and time the event occurred at the edge                                                                                                                          | int or string    |
| EdgeColoCode           | The airport code of the Cloudflare datacenter that served this request                                                                                                    | string           |
| EdgeResponseStatus     | HTTP response status code returned to browser                                                                                                                             | int              |
| Kind                   | The kind of event, currently only possible values are: <em>firewall</em>                                                                                                  | string           |
| MatchIndex             | Rules match index in the chain                                                                                                                                            | int              |
| Metadata               | Additional product-specific information. Metadata is organized in key:value pairs. Key and Value formats can vary by Cloudflare security product and can change over time | object           |
| OriginResponseStatus   | HTTP origin response status code returned to browser                                                                                                                      | int              |
| OriginatorRayID        | The RayID of the request that issued the challenge/jschallenge                                                                                                            | string           |
| RayID                  | The RayID of the request                                                                                                                                                  | string           |
| RuleID                 | The Cloudflare security product-specific RuleID triggered by this request                                                                                                 | string           |
| Source                 | The Cloudflare security product triggered by this request. <br />Possible sources are <em>unknown</em>                                                                    | <em>asn</em>     | <em>country</em>      | <em>ip</em>        | <em>iprange</em>           | <em>securitylevel</em> | <em>zonelockdown</em>    | <em>waf</em>             | <em>firewallrules</em>   | <em>uablock</em>           | <em>ratelimit</em>         | <em>bic</em>               | <em>hot</em>                 | <em>l7ddos</em> | <em>validation</em>       | <em>botfight</em>                | <em>apishield</em>                            | <em>botmanagement</em>                     | <em>dlp</em>                      | <em>firewallmanaged</em> | <em>firewallcustom</em> | string |

{{</table-wrap>}}

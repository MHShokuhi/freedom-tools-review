# Introduction
- This repo contains the list of tools I've tested for bypassing the IR GFW and my results.

- This list and these reviews are not exhaustive and your experience might differ; I'm just documenting my experience and writing these with somewhat less tech-savvy people in mind.

- **Last Update: 5 February 2026**

<br />

# ⚡ Circumvention Tools

## [3x-ui](https://github.com/MHSanaei/3x-ui)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|Xray-core|3️⃣Hard|1️⃣Easy|v2.8.9|✅|

> Extremely useful and powerful tool but don't use it unless you have some knowledge of working with these kinds of advanced circumvention tools. Most guides are out of date and unless you have some knowledge for tricking GFW, your inbounds won't work or get blocked soon.

## [Amnezia Self-hosted](https://amnezia.org/starter-guide)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|AmneziaWG<br />IKEv2<br />OpenVPN (+ Cloak)<br />Wireguard<br />REALITY|1️⃣Easy|1️⃣Easy|v4.8.12.9|❌|

> Very easy to set up but unless you are sure about your direct IP range or using a whitelisted range for server (from Gcore for example), it won't work for current GFW since it's only using **REALITY** from **Xray-core**. The other methods didn't work either.

## [BPB-Worker-Panel](https://github.com/bia-pain-bache/BPB-Worker-Panel)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|Trojan<br />VLESS<br />WARP<br />WARP Pro|1️⃣Easy|1️⃣Easy|v4.1.10|✅|

> Easy enough to setup using Cloudflare free account resources with a great guide and support for many kinds of clients out of box. You can use it to its 100k requests/day limit (enough for 1-2 people) as long as there are Cloudflare clean IPs or your Fragment settings work.

## [CompassVPN](https://www.compassvpn.org/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|VLESS|2️⃣Medium|1️⃣Easy|v27/1/2026|❌|

> None of the configs (direct or behind Cloudflare) would bypass GFW for me on the same server/ip/domain that I could bypass with other tools like **3x-ui** or **Hiddify-Manager**. It has a nice dashboard though.

## [dnstm](https://github.com/net2share/dnstm)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />Slipstream|1️⃣Easy|2️⃣Medium|v0.6.2|✅|

> Robust and powerful with many options to use **dnstt** or **Slipstream-rust** methods. You need to find a working DNS resolver for it to work but currently it's one of the few ways to bypass total internet blackouts IR puts in place for normal people.

⚠️ Multi-Tunnel mode is a bit buggy and SSH hardening removes all ciphers that HTTP Injector supports. Add one like aes256-ctr manually (or whatever the log in that app says and you thinks is safe) after applying hardening by the script to make that app work again.

## [dnstt](https://www.bamsoftware.com/software/dnstt/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt|4️⃣Very Hard|2️⃣Medium|v20241021|✅|

> One of the cornerstones of bypassing total internet shutdowns IR GFW applies to this date. During those times you need a working DNS resolver though which might not work for everyone. The project itself is not easy to deploy since you have to do everything manually but you will have more options to configure your tunnel. There are other tools that make deploying this kind of server much easier, use them instead like above or below entry.

## [dnstt-deploy](https://github.com/bugfloyd/dnstt-deploy)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt|1️⃣Easy|2️⃣Medium|v25/6/2025|✅|

> The easiest, safest and the best way to deploy **dnstt** if you are going to use that method. You need to find a working DNS resolver though (by chance or with many tools available on the internet).

## [Hiddify-Manager](https://github.com/hiddify/Hiddify-Manager/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|MTProto<br />SSH Proxy<br />sing-box<br />Xray-core|1️⃣Easy|1️⃣Easy|v11.0.17|✅|

> If you want to have many protocols in one place with the least headache for their maintenance, this is the solution for you. It has many interesting and powerful features to help you bypass IR GFW with great guides which you can follow without having much technical knowledge (a bit outdated but doable). Supports many clients too. One of my favorite tools in this list.

⚠️ A bit outdated and not updated much, it has some major and minor bugs but using apply settings button for a couple of times and using v2rayN(G) client will fix most of these problems. Don't use their own app or anything that you can't override and force `allowinsecure=false` for the configs the panel gives you because as of latest version, it wrongfully  to `allowinsecure=true` which is not ideal and can compromise the security of the connection.

## [MoaV](https://github.com/shayanb/MoaV)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />sing-box<br />WireGuard<br />wstunnel<br />|1️⃣Easy|1️⃣Easy|v1.2.2|✅|

> An interesting mix of everything for most situations. Easy to setup and share with different people. Not an advanced sing-box solution like **s-ui** but it has extra features and does almost everything itself. You can setup Conduit or Snowflake to donate your bandwidth and help others bypass censorship too but beware if you have low amount of bandwidth available on your server since these services can eat a lot of it.

## [paqet](https://github.com/hanselime/paqet)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|paqet|4️⃣Very Hard|4️⃣Very Hard|v1.0.0-alpha.13|✅|

> Very powerful and very interesting method, it even bypasses blocked IPs by IR GFW! But it's currently very experimental and unstable and because of how it works, you can't use it on normal phones (needs root access) or systems without admin/root privilege. It seems this method doesn't play that well with carriers and providers that put you behind a NAT and don't give you a public IP directly, but with tweaks to server and client configs you might get good results.

## [reality-ezpz](https://github.com/aleskxyz/reality-ezpz)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|sing-box<br />Xray-core|1️⃣Easy|1️⃣Easy|v6/1/2026|✅|

> An easy way of managing **REALITY** with some other stuff from sing-box & **Xray-core** which might help you bypass IR GFW, especially if you use its CDN-related features. You can pair it with a Telegram bot for easier user/config management.

## [RealityGhost](https://github.com/ghostmcf/RealityGhost/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|REALITY|1️⃣Easy|1️⃣Easy|v3/2/2026|❌|

> An interesting way of making **REALITY** less prone to GFW detection and interference. Hope it pays off and you need a clean IP for it to work.

⚠️ Core issue in script logic, it's not working (for now).

## [slipstream](https://github.com/EndPositive/slipstream)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream|2️⃣Medium|4️⃣Very Hard|v0.1.0|✅|

> Cousin of **dnstt** but faster and more advanced! not for general use because it lacks clients.

## [slipstream-rust](https://github.com/EndPositive/slipstream)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream|4️⃣Very Hard|3️⃣Hard|bc772dd|✅|

> Rewrite of **slipstream** in Rust with even faster speed and some new cool features which adds to its setup complexity since it doesn't have an easy installer or even pre-compiled binaries (you have to build it yourself if you want to use this repo or see the solution below). There are good clients for it so using it is easier than its original implementation in C.

## [slipstream-rust-deploy](https://github.com/AliRezaBeigy/slipstream-rust-deploy)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream|1️⃣Easy|3️⃣Hard|bc772dd|✅|

> An easy way to deploy **slipstream-rust**, get binaries for different clients and very good guide in general.

## [s-ui](https://github.com/alireza0/s-ui)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|sing-box|3️⃣Hard|1️⃣Easy|v1.3.7|✅|

> Don't use it unless you have some knowledge of working with these kinds of advanced circumvention tools. Most guides are out of date and unless you have some knowledge for tricking GFW, your inbounds won't work or get blocked soon.

## [TrustTunnel](https://github.com/TrustTunnel/TrustTunnel)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|TrustTunnel|3️⃣Hard|3️⃣Hard|v0.9.125|❌|

> After reading every document they published and testing it on different server regions and providers (all IPs tested and seemed clean), it's safe to say that TrustTunnel is not very useful for Iran (in its current state). It has some interesting ideas, a big team behind it (AdGuard VPN) but all their methods are nothing that IR GFW can't handle, it's miles behind **REALITY** and GFW can even break that. I could make the connection with the CLI client, get a nice ping to the server but GFW would detect it after couple of seconds and keep disconnecting me again and again (I didn't play with its settings though, all buffers and such were left default). It's also in very early stages of development, very unstable, lacks many things (even documentation) and sadly, can't make the Flutter app work and connect it to the same server I was successfully connecting for couple of seconds via CLI.

## [Xray-core](https://github.com/XTLS/Xray-core)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|Xray-core|4️⃣Very Hard|4️⃣Very Hard|v26.2.4|✅|

> If you don't mind reading walls of Chinese text, experimenting like someone stuck in a dark room that tries to get out or using command line, this is the tool for you. You have almost limitless possibilities when using the core directly and it has some good examples in another repo which you can use or get inspired. Unless you want to be cutting edge with maximum freedom and experiment with stuff or test something fast, stay away from this solution and use other things like **3x-ui** or **Hiddify-Manager**.

<br />

# ✨ Complementary Tools

TBA

<br />

# 🚀 Clients

TBA

<br />

# 📝 Changelog

5/2/2026

> Initial Publication


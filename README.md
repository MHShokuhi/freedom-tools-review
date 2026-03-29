# Introduction
- This repo contains the list of tools I've tested for bypassing the IR GFW and my results.

- This list and these reviews are not exhaustive and your experience might differ; I'm just documenting my experience and writing these with somewhat less tech-savvy people in mind.

- **Last Update: 29 March 2026**

<br />

# ⚡ Circumvention Tools

## [3x-ui](https://github.com/MHSanaei/3x-ui)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|Xray-core|3️⃣Hard|1️⃣Easy|v2.8.11|✅|

> If you can utilize xDNS & FinalMask feature, you can make it work, else traditional ways is ineffective without a whitelisted IR IP.

## [Amnezia Self-hosted](https://amnezia.org/starter-guide)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|AmneziaWG<br />IKEv2<br />OpenVPN (+ Cloak)<br />Wireguard<br />REALITY|1️⃣Easy|1️⃣Easy|v4.8.14.5|❌|

> Useless in current situation.

## [BPB-Worker-Panel](https://github.com/bia-pain-bache/BPB-Worker-Panel)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|Trojan<br />VLESS<br />WARP<br />WARP Pro|1️⃣Easy|1️⃣Easy|v4.1.13|❌|

> If you can chain-proxy or something, it can be useful, else you can't use it directly since CF is blocked.

## [CompassVPN](https://www.compassvpn.org/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|VLESS|2️⃣Medium|1️⃣Easy|v27/1/2026|❌|

> It wasn't working much before and useless now.

## [dnstm](https://github.com/net2share/dnstm)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />Slipstream|1️⃣Easy|2️⃣Medium|v0.6.8|✅|

> The best way to run DNS tunnels right now and it's the most stable script with the least system load. soon it will have another promising protocol (**vaydns**).

## [dnstm-setup](https://github.com/SamNet-dev/dnstm-setup)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />slipstream<br />NoizDNS|1️⃣Easy|2️⃣Medium|v1.3.1|✅|

> Like the above tool but it has **NoizDNS** (another good DNS tunneling protocol) with a bit more overhead on server but robust and awesome.

## [dnstt](https://www.bamsoftware.com/software/dnstt/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt|4️⃣Very Hard|2️⃣Medium|v20241021|✅|

> One of the cornerstones of bypassing total internet shutdowns IR GFW applies to this date. During those times you need a working DNS resolver though which might not work for everyone. The project itself is not easy to deploy since you have to do everything manually but you will have more options to configure your tunnel. There are other tools that make deploying this kind of server much easier, use them instead like above or below entry.

## [dnstt-deploy](https://github.com/bugfloyd/dnstt-deploy)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt|1️⃣Easy|2️⃣Medium|v25/6/2025|✅|

> Easy to setup, hard to remove. Use other tools to deploy **dnstt** since the script is not updated for a long time.

## [dns-tun-lb](https://github.com/aleskxyz/dns-tun-lb)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />NoizDNS<br />slipstream|2️⃣Medium|2️⃣Medium|v0.3.0|✅|

> DNS tunnel load balancer which supports **dnstt**, **NoizDNS** and **slipstream**. Haven't tested under high load so don't know how effective it is. It works though.

## [Hiddify-Manager](https://github.com/hiddify/Hiddify-Manager/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />MTProto<br />SSH Proxy<br />sing-box<br />vaydns<br />Xray-core|1️⃣Easy|1️⃣Easy|v12.1.0b9|✅|

> You must the beta version to utilize **dnstt** and **vaydns** features. Other ways to connect is a bonus but you can't use other things directly.

## [MasterDnsVPN](https://github.com/masterking32/MasterDnsVPN)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|MasterDnsVPN|3️⃣Hard|3️⃣Hard|v2026.03.28.182835-ee0bcf8|✅|

> A new DNS tunneling method, in active development and lacks client but results are promising and worth using in current situation.

## [MoaV](https://github.com/shayanb/MoaV)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />sing-box<br />WireGuard<br />wstunnel<br />xDNS|1️⃣Easy|1️⃣Easy|v1.7.4|✅|

> The only tool that setups xDNS without a hassle, but you have to choose between which DNS tunneling tool you want.

## [paqet](https://github.com/hanselime/paqet)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|paqet|4️⃣Very Hard|4️⃣Very Hard|v1.0.0-alpha.19|❌|

> Doesn't work.

## [reality-ezpz](https://github.com/aleskxyz/reality-ezpz)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|sing-box<br />Xray-core|1️⃣Easy|1️⃣Easy|v6/1/2026|❌|

> Doesn't work.

## [slipgate](https://github.com/anonvector/slipgate)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|dnstt<br />SSH Tunnel<br />slipstream<br />SOCKS5 Proxy<br />NaïveProxy<br />NoizDNS|1️⃣Easy|1️⃣Easy|v1.3.1|✅|

> Made by the dev of SlipNet, the best Android client to use most of DNS tunnels. It has some memory leaks so keep an eye on server resources. Only use DNS tunnel stuff for now, rest is useless. You can use an advanced and fast DNS resolver scan though which is only possible with this script.

⚠️ The SOCKS5 way of connection doesn't work very well it seems. **dnstm** is fine, but not this script. SSH is better for current condition though.

## [slipstream](https://github.com/EndPositive/slipstream)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream|2️⃣Medium|4️⃣Very Hard|v0.1.0|✅|

> Cousin of **dnstt** but faster and more advanced! not for general use because it lacks client. Read below.

## [slipstream-rust](https://github.com/Mygod/slipstream-rust/)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream|4️⃣Very Hard|3️⃣Hard|efd78e3|✅|

> Rewrite of **slipstream** in Rust with even faster speed and some new cool features which adds to its setup complexity since it doesn't have an easy installer or even pre-compiled binaries (you have to build it yourself if you want to use this repo or see the solution below). There are good clients for it so using it is easier than its original implementation in C. Currently it doesn't work on all the ISPs.

## [slipstream-rust-deploy](https://github.com/AliRezaBeigy/slipstream-rust-deploy)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream|1️⃣Easy|3️⃣Hard|efd78e3|✅|

> An easy way to deploy **slipstream-rust**, get binaries for different clients and very good guide in general. Currently it doesn't work on all the ISPs.

## [slipstream-rust-plus](https://github.com/Fox-Fig/slipstream-rust-plus)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream-rust-plus|3️⃣Hard|4️⃣Very Hard|5af5198|❌|

> Too fast for its own good, GFW slays it. Lacks client.

## [slipstream-rust-plus-deploy](https://github.com/Fox-Fig/slipstream-rust-plus-deploy)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|slipstream-rust-plus|1️⃣Easy|4️⃣Very Hard|a2db384|❌|

> Script to setup above method, not useful currently. Lacks client.

## [s-ui](https://github.com/alireza0/s-ui)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|sing-box|3️⃣Hard|1️⃣Easy|v1.4.0|❌|

> Can't work directly in current condition. Needs a whitelisted IR IP.

## [TrustTunnel](https://github.com/TrustTunnel/TrustTunnel)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|TrustTunnel|3️⃣Hard|3️⃣Hard|v1.0.17|❌|

> Doesn't work.

## [vaydns](https://github.com/net2share/vaydns)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|vaydns|3️⃣Hard|3️⃣Hard|v0.2.5|✅|

> Another new DNS tunneling tool with very interesting results. soon to be added to **dnstm**. lacks client but can be made to work with **dnstt** clients, with its own client it's very good, with compability-mode, it varies.

## [Xray-core](https://github.com/XTLS/Xray-core)
|Type|Deployment|Usage|Tested|Result|
|:-|:-|:-|:-|:-|
|Xray-core|4️⃣Very Hard|4️⃣Very Hard|v26.3.27|✅|

> If you can utilize xDNS & FinalMask feature, you can make it work, else traditional ways are ineffective without a whitelisted IR IP. Very cutting-edge though and flexible. have to RTFM.

<br />

# ✨ Complementary Tools

- [dnst-scanner](https://github.com/net2share/dnst-scanner)
- [findns](github.com/SamNet-dev/findns/)
- [range-scout](https://github.com/iampedii/range-scout)

<br />

# 🚀 Clients

- [SlipNet](https://github.com/anonvector/SlipNet)

<br />

# 📝 Changelog

29/3/2026

> Updated info based on current internet shutdown in Iran

5/2/2026

> Initial Publication

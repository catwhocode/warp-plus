# Warp-Plus

Warp-Plus is an open-source implementation of Cloudflare's Warp, enhanced with Psiphon integration for circumventing censorship. This project aims to provide a robust and cross-platform VPN solution that can use psiphon on top of warp and warp-in-warp for changing the user virtual nat location.

## Features

- **Warp Integration**: Leverages Cloudflare's Warp to provide a fast and secure VPN service.
- **Psiphon Chaining**: Integrates with Psiphon for censorship circumvention, allowing seamless access to the internet in restrictive environments.
- **Warp in Warp Chaining**: Chaning two instances of warp together to bypass location restrictions.
- **SOCKS5 Proxy Support**: Includes a SOCKS5 proxy for secure and private browsing.

## Getting Started

### Prerequisites

- [Download the latest version from the releases page](https://github.com/bepass-org/warp-plus/releases)
- Basic understanding of VPN and proxy configurations

### Usage

```
NAME
  warp-plus

FLAGS
  -4                       only use IPv4 for random warp endpoint
  -6                       only use IPv6 for random warp endpoint
  -v, --verbose            enable verbose logging
  -b, --bind STRING        socks bind address (default: 127.0.0.1:8086)
  -e, --endpoint STRING    warp endpoint
  -k, --key STRING         warp key
      --dns STRING         DNS address (default: 1.1.1.1)
      --gool               enable gool mode (warp in warp)
      --cfon               enable psiphon mode (must provide country as well)
      --country STRING     psiphon country code (valid values: [AT AU BE BG CA CH CZ DE DK EE ES FI FR GB HR HU IE IN IT JP LV NL NO PL PT RO RS SE SG SK US]) (default: AT)
      --scan               enable warp scanning
      --rtt DURATION       scanner rtt limit (default: 1s)
      --cache-dir STRING   directory to store generated profiles
      --fwmark UINT        set linux firewall mark for tun mode (requires sudo/root/CAP_NET_ADMIN) (default: 0)
      --reserved STRING    override wireguard reserved value (format: '1,2,3')
      --wgconf STRING      path to a normal wireguard config
      --test-url STRING    connectivity test url (default: http://connectivity.cloudflareclient.com/cdn-cgi/trace)
  -c, --config STRING      path to config file
      --version            displays version number
```

### Country Codes for Psiphon

- Austria (AT)
- Australia (AU)
- Belgium (BE)
- Bulgaria (BG)
- Canada (CA)
- Switzerland (CH)
- Czech Republic (CZ)
- Germany (DE)
- Denmark (DK)
- Estonia (EE)
- Spain (ES)
- Finland (FI)
- France (FR)
- United Kingdom (GB)
- Croatia (HR)
- Hungary (HU)
- Ireland (IE)
- India (IN)
- Italy (IT)
- Japan (JP)
- Latvia (LV)
- Netherlands (NL)
- Norway (NO)
- Poland (PL)
- Portugal (PT)
- Romania (RO)
- Serbia (RS)
- Sweden (SE)
- Singapore (SG)
- Slovakia (SK)
- United States (US)
![0](https://raw.githubusercontent.com/Ptechgithub/configs/main/media/line.gif)
### Termux

```
bash <(curl -fsSL https://raw.githubusercontent.com/bepass-org/warp-plus/master/termux.sh)
```
![1](https://github.com/Ptechgithub/configs/blob/main/media/18.jpg?raw=true)

## Acknowledgements

- Cloudflare Warp
- Psiphon
- All contributors and supporters of this project

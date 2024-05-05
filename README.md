# EDTEXT

<p align="center">
  <img src="https://cloudflare-ipfs.com/ipfs/bafybeigd6i5aavwpr6wvnwuyayklq3omonggta4x2q7kpmgafj357nkcky" alt="EDtunnel" style="margin-bottom: -50px;">
</p>

GitHub Repository for [https://github.com/3Kmfi6HP/EDtunnel](https://github.com/3Kmfi6HP/EDtunnel)

ask question and cloudflare ips: [https://t.me/edtunnel](https://t.me/edtunnel)

[![Repository](https://img.shields.io/badge/View%20on-GitHub-blue.svg)](https://github.com/3Kmfi6HP/EDtunnel)

## available branches and explain

| Branch Name   | Description                                                   |
| ------------- | ------------------------------------------------------------- |
| main          | Main branch for the project                                   |

## Deploy in pages.dev


1. Clone this repository deploy in cloudflare pages.

## Deploy in worker.dev

1. Copy `_worker.js` code from [here](https://github.com/WTNLXTBL/EDTEXT/blob/main/_worker.js).

2. Alternatively, you can click the button below to deploy directly.

   [![Deploy to Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/WTNLXTBL/EDTEXT)

## Lazy to deploy

`aHR0cHM6Ly9vc3MudjJyYXlzZS5jb20vcHJveGllcy9kYXRhLzIwMjMtMDctMzAvRnJFS1lvQS50eHQ=` (free clash.meta subscribe config)

## UID Setting (Optional)

1. When deploy in cloudflare pages, you can set uuid in `wrangler.toml` file. variable name is `UID`. `wrangler.toml` file is also supported. (recommended) in case deploy in webpages, you can not set uuid in `wrangler.toml` file.

2. When deploy in worker.dev, you can set uuid in `_worker.js` file. variable name is `UserID`. `wrangler.toml` file is also supported. (recommended) in case deploy in webpages, you can not set uuid in `wrangler.toml` file. in this case, you can also set uuid in `UUID` enviroment variable.

Note: `UID` is the uuid you want to set. pages.dev and worker.dev all of them method supported, but depend on your deploy method.

### UID Setting Example

1. single uuid environment variable

   ```.environment
   UID = "uuid here your want to set"
   ```

2. multiple uuid environment variable

   ```.environment
   UID = "uuid1,uuid2,uuid3"
   ```

   note: uuid1, uuid2, uuid3 are separated by commas`,`.
   when you set multiple uuid, you can use `https://edtunnel.pages.dev/config/user/uuid1` to get the clash config and vless:// link.

## subscribe vless:// link (Optional)

1. visit `https://edtunnel.pages.dev/config/user/uuid your set` to get the subscribe link.

2. visit `https://edtunnel.pages.dev/sub/uuid your set` to get the subscribe content with `uuid your set` path.

   note: `uuid your set` is the uuid you set in UID enviroment or `wrangler.toml`, `_worker.js` file.
   when you set multiple uuid, you can use `https://edtunnel.pages.dev/sub/uuid1` to get the subscribe content with `uuid1` path.(only support first uuid in multiple uuid set)

3. visit `https://edtunnel.pages.dev/sub/uuid your set/?format=clash` to get the subscribe content with `uuid your set` path and `clash` format. content will return with base64 encode.

   note: `uuid your set` is the uuid you set in UID enviroment or `wrangler.toml`, `_worker.js` file.
   when you set multiple uuid, you can will use `https://edtunnel.pages.dev/sub/uuid1/?format=clash` to get the subscribe content with `uuid1` path and `clash` format.(only support first uuid in multiple uuid set)

## subscribe Cloudflare bestip(pure ip) link

1. visit `https://edtunnel.pages.dev/bestip/uuid your set` to get subscribe info.

2. cpoy subscribe url link `https://edtunnel.pages.dev/bestip/uuid your set` to any clients(clash/v2rayN/v2rayNG) you want to use.

3. done. if have any questions please join [@edtunnel](https://t.me/edtunnel)

## multiple port support (Optional)

   <!-- let portArray_http = [80, 8080, 8880, 2052, 2086, 2095];
	let portArray_https = [443, 8443, 2053, 2096, 2087, 2083]; -->

For a list of Cloudflare supported ports, please refer to the [official documentation](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/ports).

By default, the port is 80 and 443. If you want to add more ports, you can use the following ports:

```text
80, 8080, 8880, 2052, 2086, 2095, 443, 8443, 2053, 2096, 2087, 2083
http port: 80, 8080, 8880, 2052, 2086, 2095
https port: 443, 8443, 2053, 2096, 2087, 2083
```

if you deploy in cloudflare pages, https port is not supported. Simply add multiple ports node drictly use subscribe link, subscribe content will return all Cloudflare supported ports.

## RelayIP (Optional)

1. When deploy in cloudflare pages, you can set RelayIP in `wrangler.toml` file. variable name is `RelayIP`.

2. When deploy in worker.dev, you can set RelayIP in `_worker.js` file. variable name is `RelayIP`.

note: `RelayIP` is the ip or domain you want to set. this means that the RelayIP is used to route traffic through a proxy rather than directly to a website that is using Cloudflare's (CDN). if you don't set this variable, connection to the Cloudflare IP will be cancelled (or blocked)...

resons: Outbound TCP sockets to Cloudflare IP ranges are temporarily blocked, please refer to the [tcp-sockets documentation](https://developers.cloudflare.com/workers/runtime-apis/tcp-sockets/#considerations)

## Usage

frist, open your pages.dev domain `https://edtunnel.pages.dev/` in your browser, then you can see the following page:
The path `/uuid your seetting` to get the clash config and vless:// link.

## Star History

<a href="https://star-history.com/#WTNLXTBL/EDTEXT&Date">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=WTNLXTBL/EDTEXT&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=WTNLXTBL/EDTEXT&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=
    WTNLXTBL/EDTEXT&type=Date" />
  </picture>
</a>

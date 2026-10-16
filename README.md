# GP-Simulator 2 — API Documentation

Official documentation for the **GP-Simulator 2 Local HTTP API**, maintained by **GPSPATRON Sp. z o. o.**

The API allows customers and integrators to discover configured SDR channels, read and update simulation settings, start and stop generation, apply LLA shifts, and retrieve generation logs.

**[View the interactive API reference](https://gpspatron.github.io/GP-Simulator-2-API/)**

## Contents

| File | Purpose |
| --- | --- |
| [`openapi.yaml`](openapi.yaml) | OpenAPI 3.0.3 specification, including parameters, responses, and examples |
| [`index.html`](index.html) | Static API reference viewer using Scalar |
| [`COPYRIGHT.md`](COPYRIGHT.md) | Copyright and documentation usage notice |
| [`SECURITY.md`](SECURITY.md) | Private vulnerability reporting and credential-handling guidelines |
| [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md) | Attribution for the API reference viewer |

## Getting started

1. Launch GP-Simulator 2 with administrator privileges, as required by its local API server.
2. In the application, open **API** and enable **Enable API Server**.
3. Select a listening port (default **5000**) and enable **API key** authorization. Click **APPLY**.
4. Keep **Allow Remote Access** disabled unless required for an explicitly secured deployment.
5. Obtain the API key from the application's API settings when using API-key authentication.
6. Get the available SDR channels with `GET /gp-simulator-2/api/v1/sdrs` and use a returned `genAlias` for channel-specific requests.

The default API base URL is `http://localhost:5000`. For detailed requests, parameters, authentication modes and responses, see [`openapi.yaml`](openapi.yaml) or the interactive reference.

## Security and privacy

The API controls local simulation equipment. **Do not expose an unauthenticated API server to untrusted networks.** The documented server uses HTTP, so take additional network security measures before enabling remote access. Do not commit API keys, local configuration files, production logs, personal data, or confidential customer information to this public repository.

The public API reference is **documentation only**; interactive `Test Request` execution is intentionally disabled on the hosted reference page. Use your own API client against an authorized GP-Simulator 2 installation.

Report security vulnerabilities privately as described in [`SECURITY.md`](SECURITY.md).

## Support

- Product website: https://gpspatron.com/
- Support portal: https://support.gpspatron.com/
- Email: support@gpspatron.com

## Intellectual property

Copyright © 2026 **GPSPATRON Sp. z o. o.** All rights reserved.

This repository publishes interface documentation, **not the source code or license of GP-Simulator 2**. Public availability of these files does not make the commercial software open source or grant any software license. See [`COPYRIGHT.md`](COPYRIGHT.md) for further information. Third-party viewer software remains subject to its own license.

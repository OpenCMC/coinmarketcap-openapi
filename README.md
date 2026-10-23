# CoinMarketCap OpenAPI

The official OpenAPI 3.1 definitions of the CoinMarketCap APIs, generated from the same source as the [API documentation](https://coinmarketcap.com/api/documentation/pro-api-reference/endpoint-overview).

Point an SDK generator at them to get a typed client in your language, import them into Postman or Insomnia to try requests, or load them into an AI agent so it knows every endpoint, parameter and response field.

| File | API | Base URL | Auth | Docs |
|---|---|---|---|---|
| [`openapi.json`](openapi.json) | Pro API | `https://pro-api.coinmarketcap.com` | API key in the `X-CMC_PRO_API_KEY` header | [Pro API reference](https://coinmarketcap.com/api/documentation/pro-api-reference/endpoint-overview) |
| [`openapi-keyless.json`](openapi-keyless.json) | Keyless Public API | `https://pro-api.coinmarketcap.com/public-api` | None | [Keyless Public API](https://coinmarketcap.com/api/documentation/pro-api-reference/keyless-public-api) |

Each file is complete on its own, with the right base URL and auth for its API. `openapi-keyless.json` contains only the endpoints you can call without an API key. To use the full Pro API, get a free key at [coinmarketcap.com/api](https://coinmarketcap.com/api/).

## Official SDKs

Both SDKs are generated from `openapi.json`:

- TypeScript / JavaScript: [`@coinmarketcap/sdk`](https://www.npmjs.com/package/@coinmarketcap/sdk) ([source](https://github.com/OpenCMC/coinmarketcap-api-typescript))
- Python: [`coinmarketcap-sdk`](https://pypi.org/project/coinmarketcap-sdk/) ([source](https://github.com/OpenCMC/coinmarketcap-api-python))

## Updates

The same files are published with the documentation at [`/api/documentation/openapi.json`](https://coinmarketcap.com/api/documentation/openapi.json) and [`/api/documentation/openapi-keyless.json`](https://coinmarketcap.com/api/documentation/openapi-keyless.json). API changes land there first, and this repo is updated to match. If a spec doesn't match what the API returns, please [open an issue](https://github.com/OpenCMC/coinmarketcap-openapi/issues).

## License

[MIT](LICENSE)

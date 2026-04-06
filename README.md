# @shoppexio/storefront

Official JavaScript storefront SDK for Shoppex.

Use this SDK when you want to embed Shoppex products, cart behavior, and hosted checkout into a custom frontend.

## Install

```bash
npm install @shoppexio/storefront
```

## Quick Start

```ts
import shoppex from "@shoppexio/storefront";

shoppex.init("my-store");

const products = await shoppex.getProducts();
shoppex.addToCart(products.data?.[0]?.uniqid ?? "", "default", 1);
await shoppex.checkout();
```

## Good Fit

Use this package for:

- custom storefronts
- cart state
- hosted checkout redirects
- product and store data loading

## Not This Package

If you want the authenticated Developer API wrapper for backend integrations, use `@shoppexio/sdk` instead.

## Docs

- Storefront docs: [docs.shoppex.io/sdk/introduction](https://docs.shoppex.io/sdk/introduction)
- Installation: [docs.shoppex.io/sdk/installation](https://docs.shoppex.io/sdk/installation)

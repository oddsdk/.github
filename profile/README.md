# Welcome to ODD SDK!

ODD SDK is [Fission](https://fission.codes)'s true local-first, edge computing stack. ODD SDK empowers you to build fully distributed web applications with auth and storage without needing a complex backend. To learn more, check out the [ODD SDK docs](https://docs.odd.dev/).

In this organization, you'll find the ODD SDK library and templates for quickly getting started with ODD SDK and reference examples of apps built using the ODD SDK.

## ODD App Templates: Build a new ODD app

The ODD App Template repositories are clone-and-go templates for building a web application using the ODD SDK, fast. The templates are "batteries included", and include user accounts, authorization, encrypted file storage, and key management through device linking.

The templates come in two authentication flavors and are implemented in two different front-end frameworks:

**WebCrypto-based Auth**

The base [ODD authentication scheme](https://docs.odd.dev/authentication-strategies) uses private keys stored using the browser's [WebCrypto API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API).

- [`odd-app-template`](https://github.com/oddsdk/odd-app-template) - An ODD App Template written in Svelte + TypeScript.
- [`odd-app-template-react`](https://github.com/oddsdk/odd-app-template-react) - An ODD App Template written in React + TypeScript.

**WalletAuth**

WalletAuth is for building apps where the user will log in with MetaMask or another in-browser crypto wallet.

- [`walletauth`](https://github.com/oddsdk/walletauth) - A WalletAuth template, written in Svelte + TypeScript.
- [`walletauth-react`](https://github.com/oddsdk/walletauth-react) - A WalletAuth template, written in React + TypeScript.

## Create ODD App: Generate an app from the CLI

[`create-odd-app`](https://github.com/oddsdk/create-odd-app) is a CLI generator that allows you to spin either React or SvelteKit flavours of the ODD App Template and ODD WalletAuth repos.

You can find other examples of ODD applications in [the Fission organization](https://github.com/fission-codes).

## React TodoMVC

The classic [TodoMVC](https://todomvc.com/) app implemented with the ODD SDK. This example demonstrates authorization through the [Fission Auth Lobby](https://auth.fission.codes/) which allows users to share a filesystem across apps.

## Stored Wasm example

This app demonstrates a simple approach to storing Wasm modules and computations in a user's filesystem. Computation and binaries performing computation can be available across a user's devices! This example also authorizes through the [Fission Auth Lobby](https://auth.fission.codes/).

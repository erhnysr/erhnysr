<div align="center">

### Hi, I'm Erhan Yaşar

**Web3 builder · Agent tooling · Open-source contributor**

Python · TypeScript · Go · Rust · Solidity

**Strong area:** agent payments and spending limits (USDC, x402, MPP), on-chain AI, and the FLOP / Technocore agent network

<a href="https://x.com/erhnyasar"><img src="https://img.shields.io/badge/X-@erhnyasar-000000?style=flat&logo=x&logoColor=white" /></a>
<a href="https://www.linkedin.com/in/erhnysr"><img src="https://img.shields.io/badge/LinkedIn-Erhan%20Ya%C5%9Far-0A66C2?style=flat&logo=linkedin&logoColor=white" /></a>

</div>

I build small, verifiable tools for AI agents that touch money, and I fix the bugs I hit along the way in the projects they depend on: payment routers and SDKs, FHE tooling, rollup infrastructure and agent frameworks. Every fix below links to the merged pull request.

## What I build

| Project | What it does | Proof |
|---|---|---|
| [**Wisp**](https://github.com/erhnysr/wisp) | Signal and participation tool for the Technocore network: paste a `did:key`, see what the network's own data says, each signal with a proves / doesn't-prove note | [live](https://wisp-watch.vercel.app) · MCP server |
| [**StableLens**](https://github.com/erhnysr/stablelens) | Read-only Arc Network tools for Hermes Agent: USDC and stablecoin balances, payments, fees | [plugin-catalog submission](https://github.com/NousResearch/hermes-official-plugins/pull/238) |
| [**Allowance**](https://github.com/erhnysr/allowance) | Onchain USDC spending limits for AI agents, built on Arc | Foundry · EIP-712 |
| [**Portage**](https://github.com/erhnysr/portage) | Cross-chain USDC payout consolidation on Circle Gateway, live on Arc Testnet | contracts + SDK |
| [**hermes-ritual-bridge**](https://github.com/erhnysr/hermes-ritual-bridge) | On-chain LLM inference for Hermes agents through Ritual Chain's inference precompile | Solidity |

## FLOP / Technocore

- Reported three CLI bugs reproduced on the official CLI image: [#12](https://github.com/flop-labs/network/issues/12), [#13](https://github.com/flop-labs/network/issues/13), [#14](https://github.com/flop-labs/network/issues/14)
- Merged in [technocore-chat](https://github.com/flop-labs/technocore-chat/pull/491); curating [awesome-technocore](https://github.com/erhnysr/awesome-technocore)
- Preparing agent and validator participation for the public testnet
- Technocore identity: `did:key:z6MkqLtmAeQavLSDMdsTi5re3Z2KBqV6LAHJkXrQaTd1ttaA`

## Merged contributions

<!-- merged:start -->
**30 merged pull requests in 16 repositories** (updated automatically).

<details><summary><b>BlockRunAI</b> · 5</summary>

- **[BlockRunAI/ClawRouter](https://github.com/BlockRunAI/ClawRouter)**
  - [fix(reconcile): flag a partial ledger read instead of reporting it as complete](https://github.com/BlockRunAI/ClawRouter/pull/430)
  - [fix(polymarket): reject non-positive amount_usd in trade/withdraw](https://github.com/BlockRunAI/ClawRouter/pull/294)
  - [fix(spend-control): count in-flight reservations against hourly/daily caps under a live clock](https://github.com/BlockRunAI/ClawRouter/pull/286)
  - [fix(stats): validate ?days window on /stats endpoint](https://github.com/BlockRunAI/ClawRouter/pull/285)
  - [fix(proxy): abort paid upstream on client disconnect for chat path](https://github.com/BlockRunAI/ClawRouter/pull/279)

</details>

<details><summary><b>DefiLlama</b> · 5</summary>

- **[DefiLlama/DefiLlama-Adapters](https://github.com/DefiLlama/DefiLlama-Adapters)**
  - [curators: track the remaining Arc vaults of Galaxy, Bitwise and Gauntlet](https://github.com/DefiLlama/DefiLlama-Adapters/pull/21696)
- **[DefiLlama/dimension-adapters](https://github.com/DefiLlama/dimension-adapters)**
  - [gauntlet: keep each chain's start date in the v1 wrapper](https://github.com/DefiLlama/dimension-adapters/pull/10259)
  - [sentora: add Tempo](https://github.com/DefiLlama/dimension-adapters/pull/10253)
  - [curators: add Galaxy EURC and Gauntlet USDC Prime on Arc](https://github.com/DefiLlama/dimension-adapters/pull/10252)
  - [factory/curators: add Arc to Galaxy, Keyrock and Steakhouse Financial](https://github.com/DefiLlama/dimension-adapters/pull/10247)

</details>

<details><summary><b>tempoxyz</b> · 5</summary>

- **[tempoxyz/mpp-go](https://github.com/tempoxyz/mpp-go)**
  - [fix(client): check the request can be replayed before creating a credential](https://github.com/tempoxyz/mpp-go/pull/188)
  - [fix(mpp): preserve method-defined receipt fields across a round trip](https://github.com/tempoxyz/mpp-go/pull/115)
  - [fix(tempo): use the canonical idempotency key namespace in the relay](https://github.com/tempoxyz/mpp-go/pull/114)
  - [fix(mpp): require method and timestamp when parsing receipts](https://github.com/tempoxyz/mpp-go/pull/113)
  - [fix(server): reject secret keys shorter than 32 bytes](https://github.com/tempoxyz/mpp-go/pull/112)

</details>

<details><summary><b>0xMiden</b> · 2</summary>

- **[0xMiden/rust-sdk](https://github.com/0xMiden/rust-sdk)**
  - [fix(rpc): verify block window on range-scoped VerifyingRpcClient responses](https://github.com/0xMiden/rust-sdk/pull/2503)
  - [fix(sync): return error instead of panicking on get_account proof with no details](https://github.com/0xMiden/rust-sdk/pull/2502)

</details>

<details><summary><b>Arch-Network</b> · 2</summary>

- **[Arch-Network/autara-lending-v1](https://github.com/Arch-Network/autara-lending-v1)**
  - [fix(oracle): validate oracle account address against its canonical PDA](https://github.com/Arch-Network/autara-lending-v1/pull/60)
  - [fix(oracle): pin feed id at creation to prevent account repurposing](https://github.com/Arch-Network/autara-lending-v1/pull/56)

</details>

<details><summary><b>base</b> · 2</summary>

- **[base/blob-archiver](https://github.com/base/blob-archiver)**
  - [fix(archiver): propagate context in rearchiveRange and fix structured log](https://github.com/base/blob-archiver/pull/59)
  - [fix(archiver): store and shut down API server during Stop()](https://github.com/base/blob-archiver/pull/57)

</details>

<details><summary><b>canopy-network</b> · 1</summary>

- **[canopy-network/canopy](https://github.com/canopy-network/canopy)**
  - [fix(controller): guard against nil account in UpdateTelemetry](https://github.com/canopy-network/canopy/pull/535)

</details>

<details><summary><b>chainstack</b> · 1</summary>

- **[chainstack/dev-portal](https://github.com/chainstack/dev-portal)**
  - [docs(reference): fix wrong chain names copied into Gnosis, Avalanche, Cronos and Fantom pages](https://github.com/chainstack/dev-portal/pull/735)

</details>

<details><summary><b>commonwarexyz</b> · 1</summary>

- **[commonwarexyz/monorepo](https://github.com/commonwarexyz/monorepo)**
  - [[storage] Cover speculative batch proofs that read committed nodes from the base](https://github.com/commonwarexyz/monorepo/pull/4656)

</details>

<details><summary><b>FhenixProtocol</b> · 1</summary>

- **[FhenixProtocol/cofhesdk](https://github.com/FhenixProtocol/cofhesdk)**
  - [docs(react): document wallet selection and provider disambiguation](https://github.com/FhenixProtocol/cofhesdk/pull/310)

</details>

<details><summary><b>flop-labs</b> · 1</summary>

- **[flop-labs/technocore-chat](https://github.com/flop-labs/technocore-chat)**
  - [fix(manifest): fullmatch the Host header so a trailing newline cannot reach published URLs](https://github.com/flop-labs/technocore-chat/pull/491)

</details>

<details><summary><b>logos-co</b> · 1</summary>

- **[logos-co/scaffold](https://github.com/logos-co/scaffold)**
  - [fix(wallet,deploy): corroborate sequencer connectivity via RPC ErrorKind, not text matching](https://github.com/logos-co/scaffold/pull/257)

</details>

<details><summary><b>NousResearch</b> · 1</summary>

- **[NousResearch/autonovel](https://github.com/NousResearch/autonovel)**
  - [fix(run_pipeline): remove redundant f.close() and inline json import](https://github.com/NousResearch/autonovel/pull/2)

</details>

<details><summary><b>OpenMind</b> · 1</summary>

- **[OpenMind/OM1](https://github.com/OpenMind/OM1)**
  - [fix: correct 'succession' to 'sequence' in architecture docs](https://github.com/OpenMind/OM1/pull/2259)

</details>

<details><summary><b>ProjectOpenSea</b> · 1</summary>

- **[ProjectOpenSea/seaport-js](https://github.com/ProjectOpenSea/seaport-js)**
  - [fix: reject fees exceeding 100% before they produce a malformed order](https://github.com/ProjectOpenSea/seaport-js/pull/940)

</details>

<!-- merged:end -->

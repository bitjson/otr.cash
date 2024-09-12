# New Listing: `SYMBOL`

<!-- Replace the `PROVIDE...` fields below to add context to this PR: -->

- Identity Name: `PROVIDE_NAME_OF_ASSET`
- Authbase: `PROVIDE_TXID`

## Evidence Linking Authbase to Identity

<!-- First, we need to prove that the authbase believes itself to be the submitted identity. This prevents an attacker from publicly claiming to control an authbase they do not control. -->

- [ ] **Direct**: a [chain-resolved registry](https://cashtokens.org/docs/bcmr/chip#chain-resolved-registries) at the authhead of the matching identity. Authhead TXID is provided below.
- [ ] **Indirect**: the identity is [burned](https://cashtokens.org/docs/bcmr/chip#burned-identities) and the authbase is equal to the latest `category`, so the authbase can safely be linked via indirect evidence.

Authbase TXID or Archived URLs:

<!-- If Direct is checked, provide the Authhead TXID. If "Indirect" is checked, provide at least two URLs to third-party archived links (archive.org, archive.is, etc.) of reputable sources vouching for this association. If the archiving service does not include the original URL in the archived URLs (i.e. it also shortens URLs), please also provide the full URL. -->

## Evidence Linking Identity to Authbase

<!-- Next, we need to prove that the identity believes itself to be the submitted authbase. This protects known identities from being associated with an attacker-controlled authbase in this registry. -->

Archived URLs:

<!-- Provide a third-party archived URL to a statement by the represented identity claiming the submitted authbase. -->

## Evidence Linking Authbase to Categories

<!-- If they differ, we need to prove that all submitted token categories are/were issued or controlled by the authbase.

As with linking the authbase to this identity, we'll need to demonstrate that each claimed category believes itself to be associated with the authbase via either direct or indirect evidence. -->

- [ ] Token `category` is equal to the authbase for all [Identity Snapshots](https://cashtokens.org/docs/bcmr/chip#identity-snapshots)
- [ ] Evidence is provided for differing `category` values below:

<!-- List each `category` value claimed in the historical timeline of the identity which to not match the identity's authbase. For each, provide either:

- Direct evidence: an authhead TXID of the category's identity.
- Indirect evidence: at least two URLs to third-party archived links of reputable sources vouching for this association.

Uncomment and duplicate the below section as needed: -->

<!--

- Differing `category`: `PROVIDE_CATEGORY_ID`
  - [ ] **Direct evidence** – category's authhead TXID with a corroborating chain-resolved registry:
  - [ ] **Indirect evidence** – the category's identity is [burned](https://cashtokens.org/docs/bcmr/chip#burned-identities) or widely understood to be lost, compromised, or destroyed; two or more archived URLs of reputable sources vouching for this association:

[Provide evidence here]

-->

## Substantiation of Other Claims

<!-- Finally, if the submitted `description` makes any claims about the behavior of tokens, please submit any additional information to help reviewers to corroborate statements of fact in your `description` or other fields. -->

- [ ] The submission (esp. the `description`) includes no claims requiring substantiation.
- [ ] The claims in this submission can be corroborated with the following evidence:

<!-- Please provide third-party archived URLs to security reviews, attestations, audits, and other resources that substantiate this submission. -->

# Checklist

- [ ] I have reviewed the [OpenTokenRegistry inclusion criteria](https://otr.cash/docs/list#inclusion-criteria), and this listing can be included in the registry.
- [ ] The listing completes all required fields:
  - **`name`**
    - [ ] No longer than 20 characters
    - [ ] Objective, authoritative, and neutral tone
  - **`description`**
    - [ ] Objective, authoritative, and neutral tone
    - [ ] Descriptions is appropriate for use in user interfaces by unaffiliated, neutral, third parties (wallets, block explorers, exchanges, etc.) without a disclaimer; no exclamations, calls to action, or disputable statements.
    - [ ] All claims are substantiated above.
  - **`token` information**
    - [ ] Token `category` is defined.
    - [ ] If fungible tokens exist for the `category`, `decimals` is defined.
    - [ ] **`symbol`**
      - [ ] Globally-unique base symbol, including among assets not listed in OpenTokenRegistry.
      - [ ] Valid symbol (regular expression: `/^[A-Z0-9]+[-A-Z0-9]*$/`)
      - [ ] Appropriate minimum length (for new assets: 4 or more characters for primarily fungible base symbols, 6 or more characters for primarily non-fungible base symbols)
      - [ ] No longer than 13 characters for base symbols
      - [ ] No longer than 26 characters for full symbols
  - [ ] **`uris.icon`**
    - [ ] Uses IPFS (`ipfs://`)
    - [ ] Either `SVG` format OR 400px by 400px `AVIF`, `WebP`, or `PNG`
  - [ ] **`uris.web`**
    - [ ] Domain name is owned by the issuing project or organization
    - [ ] Either `HTTPS` protocol OR ongoing activity demonstrated via optional URI identifiers (described in [Substantiation of Other Claims](#substantiation-of-other-claims))
  - [ ] Includes relevant historical information in previous snapshots OR this token has never been rebranded, redenominated, or reissued
- [ ] All static data (images, animations, videos, binary files, etc.) uses `IPFS` to ensure file integrity (`ipfs://...`)

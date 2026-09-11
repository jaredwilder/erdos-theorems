# Erdős–Gyárfás power-cycle forge — open TG targets

> These 25 cards are **UNPROVED_CHECKABLE_TARGET** objects from the 2026-08-04 source packet. They are published as explicit remaining obligations, not theorems. Novelty was UNRUN.

## TG01 — Power-safe cubic bridge elimination
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every minimum-order cubic counterexample is bridgeless, or every bridge side admits a smaller cubic completion whose dyadic cycles lift to the original graph.

**Claim hash:** `c01d96f49c073b51641ca65374fcbe75765f3adf682bcdb825d289d8ebdeb2cb`

## TG02 — Universal-root dyadic return theorem
**Status:** `UNPROVED_CHECKABLE_TARGET`

If delta(G)>=3 and G-v is 2-degenerate for every v, then some v has neighbors x,y joined in G-v by a path of length 2^k-2.

**Dependencies:** MC03, CY05

**Claim hash:** `f167737c4a39d55a54dbdc9f57af0605b83f8406919879b46d31834e920715c5`

## TG03 — Dyadic Laman-circuit theorem
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every graph with m=2n-2, delta>=3, and e(S)<=2|S|-3 for every proper S contains a power-of-two cycle.

**Dependencies:** MC04, MC05

**Claim hash:** `26e1a6684dac63230e323e4824840b38e4bc50f408cb4591ba7c7c5ddf0d839b`

## TG04 — Power-safe Henneberg reduction
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every dense-branch sparse circuit contains a degree-3 reduction whose smaller dyadic cycle lifts to a dyadic cycle in the original graph.

**Dependencies:** TG03

**Claim hash:** `a6c1ec054539e6959382751d112cc24ea4d529cd02543b90503f0bc0105204e7`

## TG05 — Slack discharge theorem
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every slack-branch minimum candidate with |A|-D>=6 contains a finite reducible cubic configuration or a power-of-two cycle.

**Dependencies:** MC12

**Claim hash:** `917cf2e0752b2410a0a7ad06305d1ffd0eb3b14a4db6da475c74ac9e0e39e96d`

## TG06 — Two-forest dyadic fundamental-cycle theorem
**Status:** `UNPROVED_CHECKABLE_TARGET`

For every minimum counterexample two-forest decomposition F0 union F1, some cross-forest edge has fundamental-cycle length a power of two in one direction, or after swapping the forests.

**Dependencies:** MC08

**Claim hash:** `8e0ee26f8661e7f3615b61dc3490b23da7ad8902999c583564a12cd92d215e72`

## TG07 — Concentrated selected-radius expansion
**Status:** `UNPROVED_CHECKABLE_TARGET`

The concentrated vertex from DS16 cannot sustain pairwise separated branches through every connector radius 2^k-2 in a finite minimum-degree-3 graph.

**Dependencies:** DS16, DS19, DS20, CY05

**Claim hash:** `c0096704867828824daaf29f93ea1f257af539f348446a8a9ee960a0ccef1a75`

## TG08 — Power-safe defect absorption
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every noncubic minimum candidate admits a quotient or state expansion eliminating branching cubic defects while multiplying all lifted cycle lengths by a fixed power of two.

**Dependencies:** DS10, DS16

**Claim hash:** `15f5b361ef602ee7b50ab83b6ad6b0512585366482ff46bd8017a8fac200be9b`

## TG09 — Matching-choice odd-lock destruction
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every bridgeless cubic graph has a perfect matching M for which g(M) has no odd prime divisor.

**Dependencies:** TR09, TR11

**Claim hash:** `01cc1043a0a0483ca4dd76389a126c581d9de7984b65d010959b2fd02e73d7c5`

## TG10 — Three-matching coprimality theorem
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every bridgeless cubic graph has perfect matchings M,M1,M2 such that the odd part of gcd(|M\M1|,|M\M2|) is 1.

**Dependencies:** TR09

**Claim hash:** `a96ff74612b3d99cc400e8ea6c2f958e5be7077e2ad89c63f85b8eee4cd64d8a`

## TG11 — Modular matching-lattice theorem
**Status:** `UNPROVED_CHECKABLE_TARGET`

Classify F_p-valued edge weights on matching-covered cubic graphs that have constant total on every perfect matching, with explicit tight-cut and brick/brace alternatives.

**Dependencies:** TR10

**Claim hash:** `45cc000b4251e23d07c32df122b32d5240d8b5215e0bbd79255fbe039288263c`

## TG12 — Tight-cut exchange synthesis
**Status:** `UNPROVED_CHECKABLE_TARGET`

Across a tight-cut decomposition, compatible local perfect-matching exchanges synthesize global exchange distances d1,d2,d1+d2, forcing any odd lock to descend to an active factor.

**Dependencies:** TG11

**Claim hash:** `e2cdc39b3de4cbce2d6ae8ad31ffae40df77fcd75d2a3cb15fc738e5ab567be9`

## TG13 — Brick/brace indicator exclusion
**Status:** `UNPROVED_CHECKABLE_TARGET`

In a minimal matching block, the indicator of a perfect matching cannot be a nontrivial constant modular perfect-matching weight in odd characteristic.

**Dependencies:** TG11, TG12

**Claim hash:** `9fed9d98d3002547e66e69d34dda3e1368f1df933b6107b98c728a1304e6fdfe`

## TG14 — Primitive dyadic member realization
**Status:** `UNPROVED_CHECKABLE_TARGET`

If the gcd of M-alternating half-lengths is a power of two, then for some suitable perfect matching representation an actual alternating half-length is a power of two.

**Dependencies:** TR09

**Claim hash:** `8211ae3dd84d53affd4b0429f5179b743fad042e11aead375549d31b9499df75`

## TG15 — Odd shortest-cycle dyadic steering
**Status:** `UNPROVED_CHECKABLE_TARGET`

For an odd shortest switching cycle C of length r, some exterior transition pairing has an opposite-sign route P whose compatible arc A satisfies |P|+|A|=2^ceil(log2 r).

**Dependencies:** BR03, BR05, BR06, BR07

**Claim hash:** `93de847bbace9e300d00ed4e2ef875450b4dc1cdfa9bc8d754dacbc27ea2b647`

## TG16 — Residue-preserving descent
**Status:** `UNPROVED_CHECKABLE_TARGET`

For a shortest switching cycle of length 2^s u with u odd and greater than 1, some exterior pairing yields a shorter switching cycle whose length remains divisible by 2^s.

**Dependencies:** BR09, BR10

**Claim hash:** `f4e479c06189f4a303240959755a4f10bcc08aec5962a32db154e47493bc62a4`

## TG17 — Length-displacement exchange theorem
**Status:** `UNPROVED_CHECKABLE_TARGET`

In the exterior pairing-exchange graph around a shortest switching cycle, either some route label (length, displacement) closes to a dyadic cycle, a local switch creates a shorter switching cycle, or the routing lies in an explicitly classifiable rigid family.

**Dependencies:** BR06, BR07, BR08

**Claim hash:** `525e7924582cff997de28dbb1e2994e8e7edb915b85cb75c6829ec41a371b904`

## TG18 — Exchange-rigid periodicity classification
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every exterior routing rigid under all local pairing switches is a periodic cover of the boundary cycle and admits either a smaller quotient or an arithmetic progression of switching-cycle lengths.

**Dependencies:** TG17

**Claim hash:** `0c2403808a69e672e622bb47c2b17da27f6c641f0aeb866eaefa970002ddde39`

## TG19 — Flat plateau impossibility
**Status:** `UNPROVED_CHECKABLE_TARGET`

A shortest switching cycle cannot be surrounded by a completely flat positive-error plateau in the exterior pairing-exchange graph unless TG18 periodicity holds.

**Dependencies:** TG17, TG18

**Claim hash:** `b0d2d1a91a2902ecf6a3674dbe75ec1e7ca1c9b17f70eed35d6cd6c8ce1c5c6e`

## TG20 — Finite transition hostile-system classification
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every minimal 4-regular 2+2 transition system hostile to TG15-TG17 belongs to a finite catalog of exchange-rigid templates.

**Dependencies:** TG15, TG16, TG17

**Claim hash:** `b7dc3195aef437fab9cc74f14b1656614916dc8b788c6247c4b89ec385fd800f`

## TG21 — Bounded-surplus defect-core classification
**Status:** `UNPROVED_CHECKABLE_TARGET`

For each fixed t, all noncubic minimum candidates with |A|=2|B|+t reduce to finitely many defect-core topologies of size at most 6t attached to an ordinary quotient on B.

**Dependencies:** DS10, DS15

**Claim hash:** `50f87c80954d29541d5e49f49050f20d3592aebe9bb819699593ad27799e2f81`

## TG22 — Defect-core cycle-lifting dichotomy
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every bounded defect core either admits a power-safe quotient to a smaller minimum-degree-3 graph or forces a power-of-two cycle locally.

**Dependencies:** TG21

**Claim hash:** `36017f7cd6ebeab62bfbece041fcbcf40714d7afacb1e2364e0e9fb4bee2e207`

## TG23 — Cubic-edge C4/C8 extension classification
**Status:** `UNPROVED_CHECKABLE_TARGET`

For adjacent cubic vertices u,v, every legal radius-3 extension avoiding C4 and C8 belongs to a finite list, each reducible or forcing a longer dyadic connector.

**Dependencies:** CY01, CY05

**Claim hash:** `bfb0da4bf468bd67903df683fd1c5ab27ea29440bae0f19ed5c6596b0d02fe03`

## TG24 — Induced-path contact-to-dyadic compiler
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every sufficiently long induced path in a minimum counterexample has an outside contact pattern producing a dyadic cycle or a reducible configuration.

**Claim hash:** `fb107b8fe6d8f31af45284ba1955b26f9eca82c7b05d4b0f20b64b5119dc2c5a`

## TG25 — Full flagship closure program
**Status:** `UNPROVED_CHECKABLE_TARGET`

Every finite simple graph of minimum degree at least 3 contains a cycle whose length is a power of two.

**Dependencies:** TG01, TG15, TG16, TG17, TG18, TG21, TG22

**Claim hash:** `b3ea46ec487573aa064d10c6b951a2175d43121a78e80149adc46eecb78c2aea`

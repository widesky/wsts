# Changelog

## [4.0.0](https://github.com/widesky/wsts/compare/v3.1.0...v4.0.0) (2024-09-10)


### ⚠ BREAKING CHANGES

* Upgrade to node 14 as the minimum version ([#771](https://github.com/widesky/wsts/issues/771))
* drop support for node.js 10.x ([#686](https://github.com/widesky/wsts/issues/686))
* change default `check` to `lint` ([#570](https://github.com/widesky/wsts/issues/570))
* **deps:** require TypeScript 4.x ([#565](https://github.com/widesky/wsts/issues/565))
* prefer single quotes if possible ([#475](https://github.com/widesky/wsts/issues/475))
* drop support for node 8 ([#422](https://github.com/widesky/wsts/issues/422))
* add the eol-last rule ([#425](https://github.com/widesky/wsts/issues/425))
* Switch from tslint to eslint. This will impact all lint rules, and tslint specific configuration.
* lint enforce trailing commas ([#296](https://github.com/widesky/wsts/issues/296))
* a few semver major changes ([#265](https://github.com/widesky/wsts/issues/265))
* Switch to prettier as the code formatter.
* With Node 6 going EoL in April 2019, we can change the TypeScript output target to es2017. Node 8 implements all of es2017 except for shared memory and atomics which are not common.
* Similar to #183, also disable synthetic imports.
* esModuleInterop causes synthetic imports to leak from libraries to their users. Users must compile with allowSyntheticImports as well if they use a library that uses this flag.

### fea

* a few semver major changes ([#265](https://github.com/widesky/wsts/issues/265)) ([75fb461](https://github.com/widesky/wsts/commit/75fb4610321409216dcb91c38ae9783a4eedb89e))


### Features

* add jsdocs rules ([77a8f02](https://github.com/widesky/wsts/commit/77a8f0207237d8f1dd4f2faef2c533ba0e3c2b58))
* add stylistic plugin and rules ([3fc5b14](https://github.com/widesky/wsts/commit/3fc5b14beaf2b95d9d5e48303a027c5d5121499c))
* add the eol-last rule ([#425](https://github.com/widesky/wsts/issues/425)) ([50ebd4d](https://github.com/widesky/wsts/commit/50ebd4dbaf063615f4c025f567ca28076a734223))
* Add TypeScript v4 support ([#551](https://github.com/widesky/wsts/issues/551)) ([0883956](https://github.com/widesky/wsts/commit/08839565a1d2b4b39d532c9b0b596f01b18856fe))
* adding pre-commit-hooks.yaml ([#858](https://github.com/widesky/wsts/issues/858)) ([b17994d](https://github.com/widesky/wsts/commit/b17994d2f26f0cacaf3e7956dc01bc644a32b5ae))
* allow eslintrc to run over tsx files ([#469](https://github.com/widesky/wsts/issues/469)) ([a21db94](https://github.com/widesky/wsts/commit/a21db94601def563952d677cb0980a12b6730f4c))
* change default `check` to `lint` ([#570](https://github.com/widesky/wsts/issues/570)) ([c527b66](https://github.com/widesky/wsts/commit/c527b66be1ef6a78ea14b3d29225a8d7fb7097bd))
* change output target to es2017 ([#255](https://github.com/widesky/wsts/issues/255)) ([e33db48](https://github.com/widesky/wsts/commit/e33db48d9e32b430790868a7eb59250474256a41))
* disable global rule for checking TODO comments ([#459](https://github.com/widesky/wsts/issues/459)) ([96aa84a](https://github.com/widesky/wsts/commit/96aa84a0a42181046daa248750cc8fef0c320619))
* generate .clang-format ([#163](https://github.com/widesky/wsts/issues/163)) ([9689211](https://github.com/widesky/wsts/commit/9689211df7b2cc190977fab5f84e94342d3c7714))
* generate .editorconfig ([#500](https://github.com/widesky/wsts/issues/500)) ([81397e0](https://github.com/widesky/wsts/commit/81397e0fd9a7f141c00b52f47c3c5d9a921292ad))
* generate .eslintignore when running init ([#521](https://github.com/widesky/wsts/issues/521)) ([8bce036](https://github.com/widesky/wsts/commit/8bce0368767f0c2ad7d0700deb839962bc928d16))
* install a default src template ([#340](https://github.com/widesky/wsts/issues/340)) ([4a3c511](https://github.com/widesky/wsts/commit/4a3c51143856b462804b318a5fce6baa2784e549))
* no-floating-promises ([#756](https://github.com/widesky/wsts/issues/756)) ([c93e733](https://github.com/widesky/wsts/commit/c93e73316164137e29daa7bea8a48083f7d7c1da))
* override require-atomic-updates ([#468](https://github.com/widesky/wsts/issues/468)) ([8105c93](https://github.com/widesky/wsts/commit/8105c9334ee5104b05f6b1b2f150e51419637262))
* prefer single quotes if possible ([#475](https://github.com/widesky/wsts/issues/475)) ([39a2705](https://github.com/widesky/wsts/commit/39a2705e51b4b6329a70f91f8293a2d7a363bf5d))
* print clang-format output  ([#186](https://github.com/widesky/wsts/issues/186)) ([f7c75ee](https://github.com/widesky/wsts/commit/f7c75ee67c534a2f980922d93463ca637546c0ad))
* support comments in JSON ([#571](https://github.com/widesky/wsts/issues/571)) ([cb6d2ca](https://github.com/widesky/wsts/commit/cb6d2cacb5de7bcc9c8e82dd47e14fc5bf9596a3))
* support yarn ([#285](https://github.com/widesky/wsts/issues/285)) ([f6ffe7c](https://github.com/widesky/wsts/commit/f6ffe7c8644fef31dcf3fd1d0ecd99884fb3824d)), closes [#281](https://github.com/widesky/wsts/issues/281)
* switch to prettier for formatting ([#259](https://github.com/widesky/wsts/issues/259)) ([5f35e09](https://github.com/widesky/wsts/commit/5f35e0919ddfc89e27479b90e188cbc97446e9b1))
* use eslint instead of tslint ([#400](https://github.com/widesky/wsts/issues/400)) ([b3096fb](https://github.com/widesky/wsts/commit/b3096fbd5076d302d93c2307bf627e12c423e726))
* warn for ts-ignore comments for ESM ([#810](https://github.com/widesky/wsts/issues/810)) ([350fbf0](https://github.com/widesky/wsts/commit/350fbf0486c7470123eef19a8ab1816d1d05a6ee))


### Bug Fixes

* add build/.eslintrc.json to files field ([#553](https://github.com/widesky/wsts/issues/553)) ([3b516ad](https://github.com/widesky/wsts/commit/3b516ad5e9f0d58201dde469461db7c6ed1c1b78))
* add Code of Conduct ([#262](https://github.com/widesky/wsts/issues/262)) ([e9874d6](https://github.com/widesky/wsts/commit/e9874d68ef5d0c64bb5f6a95f3c4c3229bc52562))
* address post-landing comments ([#251](https://github.com/widesky/wsts/issues/251)) ([7738ba5](https://github.com/widesky/wsts/commit/7738ba58c8d011056a998849c0473e54e611f750)), closes [#76](https://github.com/widesky/wsts/issues/76)
* align back to the google style guide ([#440](https://github.com/widesky/wsts/issues/440)) ([8bd78c4](https://github.com/widesky/wsts/commit/8bd78c4c78526a72400f618a95a987d2a7c1a8db))
* allow 'gts clean' to follow tsconfig.json dependency chain ([#185](https://github.com/widesky/wsts/issues/185)) ([d0d430d](https://github.com/widesky/wsts/commit/d0d430d0e77848c7bb8dc333f4145d7bef2acf1b))
* also disable allowSyntheticDefaultImports ([#184](https://github.com/widesky/wsts/issues/184)) ([d92f876](https://github.com/widesky/wsts/commit/d92f876627a167b0c436d091253f591447133d73))
* avoid conflicts between prettier and tslint ([#348](https://github.com/widesky/wsts/issues/348)) ([83cb107](https://github.com/widesky/wsts/commit/83cb107010f7a956bb008291066304a9f26a0f34))
* better error message for broken tsconfig.json ([#501](https://github.com/widesky/wsts/issues/501)) ([0c17a76](https://github.com/widesky/wsts/commit/0c17a76c6650eee1d8abaff11a897a432eeaa65f))
* **deps:** bump json5 from 2.2.1 to 2.2.2 addressing CVE-2022-46175 ([2a1fd61](https://github.com/widesky/wsts/commit/2a1fd614620f0dc26cc6f12c3b05a3088409b923))
* **deps:** loosen ts peer dependency ([#589](https://github.com/widesky/wsts/issues/589)) ([8f1d381](https://github.com/widesky/wsts/commit/8f1d381d7b166a510c42786c4a337e81b7222c84))
* **deps:** pin release of eslint-typescript ([#508](https://github.com/widesky/wsts/issues/508)) ([bd86b42](https://github.com/widesky/wsts/commit/bd86b42e2bb904d3765dee82262e4691a11b9958))
* **deps:** replace dependency eslint-plugin-node with eslint-plugin-n ([#865](https://github.com/widesky/wsts/issues/865)) ([efbe3a8](https://github.com/widesky/wsts/commit/efbe3a838f40959188190dc04b4f11f45dd1aa87))
* **deps:** require TypeScript 4.x ([#565](https://github.com/widesky/wsts/issues/565)) ([cbc5267](https://github.com/widesky/wsts/commit/cbc5267579ef24e8c8ceaa2ef794df3ef54ea56a))
* **deps:** update dependency chalk to v3 ([#389](https://github.com/widesky/wsts/issues/389)) ([1ce0f45](https://github.com/widesky/wsts/commit/1ce0f450677e143a27efc39def617d13c66503e8))
* **deps:** update dependency chalk to v4 ([#477](https://github.com/widesky/wsts/issues/477)) ([061d64e](https://github.com/widesky/wsts/commit/061d64e29d37b93ce55228937cc100e05ddef352))
* **deps:** update dependency diff to v4 ([#243](https://github.com/widesky/wsts/issues/243)) ([70833db](https://github.com/widesky/wsts/commit/70833dbe81cfabfd5fd44709bd8f2140a8839299))
* **deps:** update dependency eslint to v7 ([#504](https://github.com/widesky/wsts/issues/504)) ([6aee159](https://github.com/widesky/wsts/commit/6aee1595d0486ae2c7fd68d16b1b59c4c4015753))
* **deps:** update dependency eslint to v8.49.0 ([#784](https://github.com/widesky/wsts/issues/784)) ([5e2a05c](https://github.com/widesky/wsts/commit/5e2a05c12886dc63a60219e0c0830846de7c24b9))
* **deps:** update dependency eslint to v8.50.0 ([#802](https://github.com/widesky/wsts/issues/802)) ([794abf3](https://github.com/widesky/wsts/commit/794abf30e4ee1d4655436ad9efa11ee031027993))
* **deps:** update dependency eslint to v8.51.0 ([#812](https://github.com/widesky/wsts/issues/812)) ([ae913c1](https://github.com/widesky/wsts/commit/ae913c17ae4460d0f76aad16b96cb3e1f23a5b89))
* **deps:** update dependency eslint to v8.52.0 ([#821](https://github.com/widesky/wsts/issues/821)) ([50b3ce5](https://github.com/widesky/wsts/commit/50b3ce56190a5f785c52b00b8da56769255caaa1))
* **deps:** update dependency eslint to v8.53.0 ([#829](https://github.com/widesky/wsts/issues/829)) ([7d9ffed](https://github.com/widesky/wsts/commit/7d9ffed35d0ee076bda063e5189573eeba82ac0a))
* **deps:** update dependency eslint to v8.57.0 ([#833](https://github.com/widesky/wsts/issues/833)) ([0c0a45c](https://github.com/widesky/wsts/commit/0c0a45c83832034ed96c19c0f7956180587991ed))
* **deps:** update dependency eslint-config-prettier to v7 ([#601](https://github.com/widesky/wsts/issues/601)) ([6e26681](https://github.com/widesky/wsts/commit/6e266812da4b90b18e2abead9b2b5a1ca0c6654b))
* **deps:** update dependency eslint-config-prettier to v8 ([#624](https://github.com/widesky/wsts/issues/624)) ([23a4abb](https://github.com/widesky/wsts/commit/23a4abb50a539a93a7d1043669b2e42a887415fa))
* **deps:** update dependency eslint-config-prettier to v8.10.0 ([#785](https://github.com/widesky/wsts/issues/785)) ([5391d89](https://github.com/widesky/wsts/commit/5391d89de2b8af68b63954b01b90f88015258406))
* **deps:** update dependency eslint-config-prettier to v9 ([#777](https://github.com/widesky/wsts/issues/777)) ([470977a](https://github.com/widesky/wsts/commit/470977a2bc7b29db0e4abb36c362920ec16381c5))
* **deps:** update dependency eslint-config-prettier to v9.1.0 ([#836](https://github.com/widesky/wsts/issues/836)) ([9105ebb](https://github.com/widesky/wsts/commit/9105ebb83516746503f8714914fc62da0e7fe1a6))
* **deps:** update dependency eslint-plugin-node to v11 ([#426](https://github.com/widesky/wsts/issues/426)) ([a394b7c](https://github.com/widesky/wsts/commit/a394b7c1f80437f25017ca5c500b968ebb789ece))
* **deps:** update dependency eslint-plugin-prettier to v4 ([#657](https://github.com/widesky/wsts/issues/657)) ([5408bfe](https://github.com/widesky/wsts/commit/5408bfeda4eb9cc22fb948442cda4fb6da631ed7))
* **deps:** update dependency eslint-plugin-prettier to v5.0.1 ([#817](https://github.com/widesky/wsts/issues/817)) ([89b8955](https://github.com/widesky/wsts/commit/89b8955576d1997d2bc587b79bf57d3c4d07cdda))
* **deps:** update dependency eslint-plugin-prettier to v5.1.2 ([#839](https://github.com/widesky/wsts/issues/839)) ([b5ab5c4](https://github.com/widesky/wsts/commit/b5ab5c495e6da286ac57dc285586806f612913b8))
* **deps:** update dependency eslint-plugin-prettier to v5.1.3 ([#845](https://github.com/widesky/wsts/issues/845)) ([6e13e12](https://github.com/widesky/wsts/commit/6e13e12b9d4f82fc43ef015980d5345fb47b9a41))
* **deps:** update dependency eslint-plugin-prettier to v5.2.1 ([a3a7d20](https://github.com/widesky/wsts/commit/a3a7d2038f7244b7d36dc9eb12d5e5a0af2784a2))
* **deps:** update dependency execa to v4 ([#427](https://github.com/widesky/wsts/issues/427)) ([f42ef36](https://github.com/widesky/wsts/commit/f42ef36709251553342e655e287e889df72ee3e3))
* **deps:** update dependency execa to v5 ([#600](https://github.com/widesky/wsts/issues/600)) ([4e5f1e5](https://github.com/widesky/wsts/commit/4e5f1e54facf53588bbb3b025b5240edbd7f3c8a))
* **deps:** update dependency inquirer to v7 ([#377](https://github.com/widesky/wsts/issues/377)) ([bf2c349](https://github.com/widesky/wsts/commit/bf2c349b2208ac63e551542599ac9cd27b461338))
* **deps:** update dependency meow to v7 ([#502](https://github.com/widesky/wsts/issues/502)) ([cf91cda](https://github.com/widesky/wsts/commit/cf91cda1afab25759427511d3c97d0037d61c649))
* **deps:** update dependency meow to v8 ([#591](https://github.com/widesky/wsts/issues/591)) ([c7e223e](https://github.com/widesky/wsts/commit/c7e223e6a2ff605fabad2f8359a0385033f8de66))
* **deps:** update dependency pify to v4 ([#196](https://github.com/widesky/wsts/issues/196)) ([0989560](https://github.com/widesky/wsts/commit/0989560184522ccd65ea142ecd1727910583b932))
* **deps:** update dependency prettier to ~2.5.0 ([#660](https://github.com/widesky/wsts/issues/660)) ([8789fd4](https://github.com/widesky/wsts/commit/8789fd42388aead5cb572a543ae218563b21ac94))
* **deps:** update dependency prettier to ~2.6.0 ([#670](https://github.com/widesky/wsts/issues/670)) ([2feba2c](https://github.com/widesky/wsts/commit/2feba2cdf8884420349256420c8b5ccc9cb858c8))
* **deps:** update dependency prettier to ~2.7.0 ([#696](https://github.com/widesky/wsts/issues/696)) ([3c677fd](https://github.com/widesky/wsts/commit/3c677fdbad4772aea0be25c1cdd8149a88b0d735))
* **deps:** update dependency prettier to ~2.8.0 ([#743](https://github.com/widesky/wsts/issues/743)) ([7582516](https://github.com/widesky/wsts/commit/75825165ea32bb9bcd5013223d5e5dff2efa731c))
* **deps:** update dependency prettier to v2 ([#464](https://github.com/widesky/wsts/issues/464)) ([20ef43d](https://github.com/widesky/wsts/commit/20ef43d566df17d3c93949ef7db3b72ee9123ca3))
* **deps:** update dependency prettier to v3.0.3 ([#782](https://github.com/widesky/wsts/issues/782)) ([5a04e76](https://github.com/widesky/wsts/commit/5a04e76c74cb4984cbf9c7f7fbee4e800b33ca52))
* **deps:** update dependency prettier to v3.1.0 ([#832](https://github.com/widesky/wsts/issues/832)) ([faf6d7e](https://github.com/widesky/wsts/commit/faf6d7e60e7a382077de8fd7c8c5a9ec065259a5))
* **deps:** update dependency prettier to v3.1.1 ([#837](https://github.com/widesky/wsts/issues/837)) ([6de3e3b](https://github.com/widesky/wsts/commit/6de3e3b9a741e6ff0e34996848a2ac1f8957bb32))
* **deps:** update dependency prettier to v3.2.5 ([#846](https://github.com/widesky/wsts/issues/846)) ([7e60e38](https://github.com/widesky/wsts/commit/7e60e3878b877865b3536ea66dc3607d9243cee4))
* **deps:** update dependency prettier to v3.3.3 ([65a168f](https://github.com/widesky/wsts/commit/65a168fc6bf7e735836c06860404f96c50c85c91))
* **deps:** update dependency rimraf to v3 ([#374](https://github.com/widesky/wsts/issues/374)) ([2058eaa](https://github.com/widesky/wsts/commit/2058eaa682f4baae978b469fd708d1f866e7da74))
* **deps:** update dependency update-notifier to v3 ([#339](https://github.com/widesky/wsts/issues/339)) ([a6f9cfa](https://github.com/widesky/wsts/commit/a6f9cfa9c658229f030222b254efa71df513a3ba))
* **deps:** update dependency update-notifier to v4 ([#403](https://github.com/widesky/wsts/issues/403)) ([57393b7](https://github.com/widesky/wsts/commit/57393b74c6cf299e8ae09311f0382226b8baa3e3))
* **deps:** update dependency update-notifier to v5 ([#574](https://github.com/widesky/wsts/issues/574)) ([9a882bf](https://github.com/widesky/wsts/commit/9a882bf4ac30ad06e7b91a65ad5721d8e8b41c4b))
* **deps:** update dependency write-file-atomic to v3 ([#353](https://github.com/widesky/wsts/issues/353)) ([59e6aa8](https://github.com/widesky/wsts/commit/59e6aa8580a2f8e9457d2d2b6fa9e18e86347592))
* **deps:** update dependency write-file-atomic to v4 ([#687](https://github.com/widesky/wsts/issues/687)) ([f16a3e1](https://github.com/widesky/wsts/commit/f16a3e1a1101bc5dab90ac3ab1437dd7758adf4e))
* **deps:** update to newest prettier (with support for optional chain) ([#396](https://github.com/widesky/wsts/issues/396)) ([ce8ad06](https://github.com/widesky/wsts/commit/ce8ad06c8489c44a9e2ed5292382637b3ebb7601))
* **deps:** update typescript-eslint monorepo to v2.34.0 ([#509](https://github.com/widesky/wsts/issues/509)) ([998a4ac](https://github.com/widesky/wsts/commit/998a4ac9b75c97f04d8e5db37563f32d31652f23))
* **deps:** update typescript-eslint monorepo to v3 (major) ([#528](https://github.com/widesky/wsts/issues/528)) ([e22e173](https://github.com/widesky/wsts/commit/e22e17338db2ddb7eb829c821037c2f4e77ff869))
* **deps:** update typescript-eslint monorepo to v4 ([#556](https://github.com/widesky/wsts/issues/556)) ([54148df](https://github.com/widesky/wsts/commit/54148dfbd8b5f8b36a0f44f901c5db933393a661))
* **deps:** update typescript-eslint monorepo to v5 ([#688](https://github.com/widesky/wsts/issues/688)) ([ed2fd0c](https://github.com/widesky/wsts/commit/ed2fd0ce1be4826239b97bc1c8fdae5c61c50e62))
* **deps:** upgrade to eslint 8.x ([#693](https://github.com/widesky/wsts/issues/693)) ([7ae5c8b](https://github.com/widesky/wsts/commit/7ae5c8b827abb41844ba6f533821bf3d0a7f302b))
* **deps:** upgrade to latest version of meow ([#616](https://github.com/widesky/wsts/issues/616)) ([634bad9](https://github.com/widesky/wsts/commit/634bad9bbbdb4d397bba101dc38ab14881172a30))
* **deps:** upgrade to meow 6.x ([#423](https://github.com/widesky/wsts/issues/423)) ([8f93d00](https://github.com/widesky/wsts/commit/8f93d0049337a832d9a22b6ae4e86fd41140ec56))
* disable empty-function check ([#467](https://github.com/widesky/wsts/issues/467)) ([6455d7a](https://github.com/widesky/wsts/commit/6455d7a9d227320d3ffe1b00c9c739b846f339a8))
* disable esModuleInterop ([#183](https://github.com/widesky/wsts/issues/183)) ([94360af](https://github.com/widesky/wsts/commit/94360af86794e06cbf93c442b62c0e5756bf391e))
* disable no-use-before-define ([#431](https://github.com/widesky/wsts/issues/431)) ([dea2c22](https://github.com/widesky/wsts/commit/dea2c223d1d3a60a1786aa820eebb93be27016a7))
* do not allow deprecated methods ([#233](https://github.com/widesky/wsts/issues/233)) ([8f81766](https://github.com/widesky/wsts/commit/8f81766c1a0d7f26f2c6b8f740848aa89cafbe92))
* do not fix format errors with --dry-run ([#171](https://github.com/widesky/wsts/issues/171)) ([f8a8cb5](https://github.com/widesky/wsts/commit/f8a8cb57ce819bb09eb4ebaaa44c80ae3d94f94c))
* drop support for node 8 ([#422](https://github.com/widesky/wsts/issues/422)) ([888c686](https://github.com/widesky/wsts/commit/888c68692079065f38ce66ec84472f1f3311a050))
* drop update notifier ([#706](https://github.com/widesky/wsts/issues/706)) ([cab7704](https://github.com/widesky/wsts/commit/cab7704389c2ba7e8e426da08397af47991d8596))
* emit .prettierrc.js with init ([#462](https://github.com/widesky/wsts/issues/462)) ([b114614](https://github.com/widesky/wsts/commit/b114614d22ab5560d2d1dd5cb6695968cc80027b))
* enable trailing comma ([#470](https://github.com/widesky/wsts/issues/470)) ([6518f58](https://github.com/widesky/wsts/commit/6518f5843d3093e3beb7d3371b56d9aecedf3924))
* fix with --dry-run should not modify files ([#169](https://github.com/widesky/wsts/issues/169)) ([9a1bfdd](https://github.com/widesky/wsts/commit/9a1bfdd980e9c0495286d2ab9542b14cf8f45b91))
* fixed typos ([#231](https://github.com/widesky/wsts/issues/231)) ([e29fc14](https://github.com/widesky/wsts/commit/e29fc14cf493cb35eed39db0b9f2962bce5e3219))
* **format:** deal with absent .clang-format ([#176](https://github.com/widesky/wsts/issues/176)) ([074a377](https://github.com/widesky/wsts/commit/074a377566ff4b5c4e1be852f63cdc2bd9cc99ea))
* include *.tsx and *.jsx in default fix command ([#473](https://github.com/widesky/wsts/issues/473)) ([0509780](https://github.com/widesky/wsts/commit/050978005ad089d9b3b5d8895b25ea1175d75db2))
* **init:** init package with better main, types ([#179](https://github.com/widesky/wsts/issues/179)) ([122fe81](https://github.com/widesky/wsts/commit/122fe81ab6a1f55c4ad5d62e6aa7e40c2d191605))
* line up linting with owlbot post-processing linting ([#778](https://github.com/widesky/wsts/issues/778)) ([a731fe9](https://github.com/widesky/wsts/commit/a731fe9aef6d0003fe229627522ab8250a9222d9))
* lint enforce trailing commas ([#296](https://github.com/widesky/wsts/issues/296)) ([aca4b13](https://github.com/widesky/wsts/commit/aca4b137aa647f5288de0ef505a480d19fbbffd1))
* **lint:** skip lint on json files ([#220](https://github.com/widesky/wsts/issues/220)) ([1c938eb](https://github.com/widesky/wsts/commit/1c938ebdd10445fe86a291f1f6266d200eaf2d1b))
* npx command on Windows and make sure build/test work on Windows too ([#306](https://github.com/widesky/wsts/issues/306)) ([458be26](https://github.com/widesky/wsts/commit/458be26f5e7b19327f8123d031622d72568333e6))
* pin prettier to 2.3.x ([#641](https://github.com/widesky/wsts/issues/641)) ([323fb4a](https://github.com/widesky/wsts/commit/323fb4acacc9bfc1fcba06b27135a77acc54b15a))
* point to correct node_module directory ([b331f23](https://github.com/widesky/wsts/commit/b331f23433d375d74a3eed55987eef98f20049d3))
* process less files in parallel preventing OOM errors ([#369](https://github.com/widesky/wsts/issues/369)) ([b48196d](https://github.com/widesky/wsts/commit/b48196d714bd0c685878b20cd8aef81f4639a48a))
* prohibit calls for it.only and describe.only ([#499](https://github.com/widesky/wsts/issues/499)) ([071c33c](https://github.com/widesky/wsts/commit/071c33ceef0e3765166aaebf6ed4698167ac0f98))
* properly specify cmdline flags to meow ([#166](https://github.com/widesky/wsts/issues/166)) ([2cebae4](https://github.com/widesky/wsts/commit/2cebae4424f6af5bc251353c737ee8314f48a767))
* provide filepath to prettier ([#273](https://github.com/widesky/wsts/issues/273)) ([02e0772](https://github.com/widesky/wsts/commit/02e07728557737685b73de2b1a1fb4f7fcee6e64))
* Remove manual package.json interface ([#294](https://github.com/widesky/wsts/issues/294)) ([24e5918](https://github.com/widesky/wsts/commit/24e591845a5b3e45ecf3182d60633e4340e88ec1))
* Remove redundant glob pattern ([#293](https://github.com/widesky/wsts/issues/293)) ([0d4cc6c](https://github.com/widesky/wsts/commit/0d4cc6cbc91f0c5d01fe507755f001c9357ca1bd))
* Removed redundant escape characters from RegExps ([#230](https://github.com/widesky/wsts/issues/230)) ([e067218](https://github.com/widesky/wsts/commit/e0672185f48a0c90b5568141c14e1784214990b7))
* Revert 'update dependency eslint to v7'" ([#507](https://github.com/widesky/wsts/issues/507)) ([0f9950b](https://github.com/widesky/wsts/commit/0f9950b273329dbcce5f3cc20864c3dcd076f08c))
* revert feat: no-floating-promises ([44de7f7](https://github.com/widesky/wsts/commit/44de7f705cea94d4781e4eb4b2d71a4ee4f0e89d))
* **rule:** turn off @typescript-eslint/no-var-requires ([#578](https://github.com/widesky/wsts/issues/578)) ([3b37229](https://github.com/widesky/wsts/commit/3b37229c45969a3c53af123c69bb749578ee6b0b))
* run eslint from PATH ([#654](https://github.com/widesky/wsts/issues/654)) ([5dc2a76](https://github.com/widesky/wsts/commit/5dc2a76aae06e5e46b6b623447837c77b58cd757))
* throw an error if running with an unsupported version of nodejs ([#493](https://github.com/widesky/wsts/issues/493)) ([94fdf1e](https://github.com/widesky/wsts/commit/94fdf1eaed634aa73c3e44c7a3d9f1325f773b07))
* update eslint-prettier ([43d4a06](https://github.com/widesky/wsts/commit/43d4a06a27565b7d3839432c6f8267d254f6a002))
* upgrade init'ed and allowed versions of TypeScript ([#208](https://github.com/widesky/wsts/issues/208)) ([66da7ec](https://github.com/widesky/wsts/commit/66da7ec44c9423d05fc964a788e44d82377b0c67))
* use .prettierrc.js ([#437](https://github.com/widesky/wsts/issues/437)) ([06efa84](https://github.com/widesky/wsts/commit/06efa8444cdf1064b64f3e8d61ebd04f45d90b4c))
* use correct lint config for individual files ([#167](https://github.com/widesky/wsts/issues/167)) ([09ca073](https://github.com/widesky/wsts/commit/09ca073be502965b4f07815251038b141bb00c29))


### Performance Improvements

* Supercharge Performance & Efficiency: Leveraging `Promise.all` for Resource-Friendly Tasks 🚤 ([#838](https://github.com/widesky/wsts/issues/838)) ([7424fe1](https://github.com/widesky/wsts/commit/7424fe19f822dc152315c1b1eb5f874512a88b55))


### Miscellaneous Chores

* Upgrade to node 14 as the minimum version ([#771](https://github.com/widesky/wsts/issues/771)) ([6301178](https://github.com/widesky/wsts/commit/6301178c859361ddf8dfd678f94fc80ad5b7e38f))


### Build System

* drop support for node.js 10.x ([#686](https://github.com/widesky/wsts/issues/686)) ([12cd913](https://github.com/widesky/wsts/commit/12cd913b6e9eb97e52b1cf3a275aadfa4517fdcb))

## [5.3.0](https://github.com/google/gts/compare/v5.2.0...v5.3.0) (2024-03-21)


### Features

* adding pre-commit-hooks.yaml ([#858](https://github.com/google/gts/issues/858)) ([b17994d](https://github.com/google/gts/commit/b17994d2f26f0cacaf3e7956dc01bc644a32b5ae))


### Bug Fixes

* **deps:** update dependency eslint to v8.51.0 ([#812](https://github.com/google/gts/issues/812)) ([ae913c1](https://github.com/google/gts/commit/ae913c17ae4460d0f76aad16b96cb3e1f23a5b89))
* **deps:** update dependency eslint to v8.52.0 ([#821](https://github.com/google/gts/issues/821)) ([50b3ce5](https://github.com/google/gts/commit/50b3ce56190a5f785c52b00b8da56769255caaa1))
* **deps:** update dependency eslint to v8.53.0 ([#829](https://github.com/google/gts/issues/829)) ([7d9ffed](https://github.com/google/gts/commit/7d9ffed35d0ee076bda063e5189573eeba82ac0a))
* **deps:** update dependency eslint-config-prettier to v9.1.0 ([#836](https://github.com/google/gts/issues/836)) ([9105ebb](https://github.com/google/gts/commit/9105ebb83516746503f8714914fc62da0e7fe1a6))
* **deps:** update dependency eslint-plugin-prettier to v5.0.1 ([#817](https://github.com/google/gts/issues/817)) ([89b8955](https://github.com/google/gts/commit/89b8955576d1997d2bc587b79bf57d3c4d07cdda))
* **deps:** update dependency eslint-plugin-prettier to v5.1.2 ([#839](https://github.com/google/gts/issues/839)) ([b5ab5c4](https://github.com/google/gts/commit/b5ab5c495e6da286ac57dc285586806f612913b8))
* **deps:** update dependency eslint-plugin-prettier to v5.1.3 ([#845](https://github.com/google/gts/issues/845)) ([6e13e12](https://github.com/google/gts/commit/6e13e12b9d4f82fc43ef015980d5345fb47b9a41))
* **deps:** update dependency prettier to v3.1.0 ([#832](https://github.com/google/gts/issues/832)) ([faf6d7e](https://github.com/google/gts/commit/faf6d7e60e7a382077de8fd7c8c5a9ec065259a5))
* **deps:** update dependency prettier to v3.1.1 ([#837](https://github.com/google/gts/issues/837)) ([6de3e3b](https://github.com/google/gts/commit/6de3e3b9a741e6ff0e34996848a2ac1f8957bb32))

## [5.2.0](https://github.com/google/gts/compare/v5.1.1...v5.2.0) (2023-10-04)


### Features

* warn for ts-ignore comments for ESM ([#810](https://github.com/google/gts/issues/810)) ([350fbf0](https://github.com/google/gts/commit/350fbf0486c7470123eef19a8ab1816d1d05a6ee))

## [5.1.1](https://github.com/google/gts/compare/v5.1.0...v5.1.1) (2023-10-04)


### Bug Fixes

* revert feat: no-floating-promises ([44de7f7](https://github.com/google/gts/commit/44de7f705cea94d4781e4eb4b2d71a4ee4f0e89d))

## [5.1.0](https://github.com/google/gts/compare/v5.0.1...v5.1.0) (2023-09-29)


### Features

* no-floating-promises ([#756](https://github.com/google/gts/issues/756)) ([c93e733](https://github.com/google/gts/commit/c93e73316164137e29daa7bea8a48083f7d7c1da))


### Bug Fixes

* **deps:** update dependency eslint to v8.49.0 ([#784](https://github.com/google/gts/issues/784)) ([5e2a05c](https://github.com/google/gts/commit/5e2a05c12886dc63a60219e0c0830846de7c24b9))
* **deps:** update dependency eslint to v8.50.0 ([#802](https://github.com/google/gts/issues/802)) ([794abf3](https://github.com/google/gts/commit/794abf30e4ee1d4655436ad9efa11ee031027993))
* **deps:** update dependency eslint-config-prettier to v8.10.0 ([#785](https://github.com/google/gts/issues/785)) ([5391d89](https://github.com/google/gts/commit/5391d89de2b8af68b63954b01b90f88015258406))
* **deps:** update dependency eslint-config-prettier to v9 ([#777](https://github.com/google/gts/issues/777)) ([470977a](https://github.com/google/gts/commit/470977a2bc7b29db0e4abb36c362920ec16381c5))
* **deps:** update dependency prettier to v3.0.3 ([#782](https://github.com/google/gts/issues/782)) ([5a04e76](https://github.com/google/gts/commit/5a04e76c74cb4984cbf9c7f7fbee4e800b33ca52))
* run eslint from PATH ([#654](https://github.com/google/gts/issues/654)) ([5dc2a76](https://github.com/google/gts/commit/5dc2a76aae06e5e46b6b623447837c77b58cd757))

## [5.0.1](https://github.com/google/gts/compare/v5.0.0...v5.0.1) (2023-08-21)


### Bug Fixes

* line up linting with owlbot post-processing linting ([#778](https://github.com/google/gts/issues/778)) ([a731fe9](https://github.com/google/gts/commit/a731fe9aef6d0003fe229627522ab8250a9222d9))

## [5.0.0](https://github.com/google/gts/compare/v4.0.1...v5.0.0) (2023-07-26)


### ⚠ BREAKING CHANGES

* Upgrade to node 14 as the minimum version ([#771](https://github.com/google/gts/issues/771))

### Bug Fixes

* **deps:** update dependency prettier to ~2.8.0 ([#743](https://github.com/google/gts/issues/743)) ([7582516](https://github.com/google/gts/commit/75825165ea32bb9bcd5013223d5e5dff2efa731c))
* update eslint-prettier ([43d4a06](https://github.com/google/gts/commit/43d4a06a27565b7d3839432c6f8267d254f6a002))


### Miscellaneous Chores

* Upgrade to node 14 as the minimum version ([#771](https://github.com/google/gts/issues/771)) ([6301178](https://github.com/google/gts/commit/6301178c859361ddf8dfd678f94fc80ad5b7e38f))

## [4.0.1](https://github.com/google/gts/compare/v4.0.0...v4.0.1) (2023-01-09)


### Bug Fixes

* **deps:** bump json5 from 2.2.1 to 2.2.2 addressing CVE-2022-46175 ([2a1fd61](https://github.com/google/gts/commit/2a1fd614620f0dc26cc6f12c3b05a3088409b923))

## [4.0.0](https://github.com/google/gts/compare/v3.1.0...v4.0.0) (2022-07-04)


### ⚠ BREAKING CHANGES

* drop support for node.js 10.x (#686)

### Features

* generate .editorconfig ([#500](https://github.com/google/gts/issues/500)) ([81397e0](https://github.com/google/gts/commit/81397e0fd9a7f141c00b52f47c3c5d9a921292ad))


### Bug Fixes

* **deps:** update dependency eslint-config-prettier to v8 ([#624](https://github.com/google/gts/issues/624)) ([23a4abb](https://github.com/google/gts/commit/23a4abb50a539a93a7d1043669b2e42a887415fa))
* **deps:** update dependency eslint-plugin-prettier to v4 ([#657](https://github.com/google/gts/issues/657)) ([5408bfe](https://github.com/google/gts/commit/5408bfeda4eb9cc22fb948442cda4fb6da631ed7))
* **deps:** update dependency prettier to ~2.5.0 ([#660](https://github.com/google/gts/issues/660)) ([8789fd4](https://github.com/google/gts/commit/8789fd42388aead5cb572a543ae218563b21ac94))
* **deps:** update dependency prettier to ~2.6.0 ([#670](https://github.com/google/gts/issues/670)) ([2feba2c](https://github.com/google/gts/commit/2feba2cdf8884420349256420c8b5ccc9cb858c8))
* **deps:** update dependency prettier to ~2.7.0 ([#696](https://github.com/google/gts/issues/696)) ([3c677fd](https://github.com/google/gts/commit/3c677fdbad4772aea0be25c1cdd8149a88b0d735))
* **deps:** update dependency write-file-atomic to v4 ([#687](https://github.com/google/gts/issues/687)) ([f16a3e1](https://github.com/google/gts/commit/f16a3e1a1101bc5dab90ac3ab1437dd7758adf4e))
* **deps:** update typescript-eslint monorepo to v5 ([#688](https://github.com/google/gts/issues/688)) ([ed2fd0c](https://github.com/google/gts/commit/ed2fd0ce1be4826239b97bc1c8fdae5c61c50e62))
* **deps:** upgrade to eslint 8.x ([#693](https://github.com/google/gts/issues/693)) ([7ae5c8b](https://github.com/google/gts/commit/7ae5c8b827abb41844ba6f533821bf3d0a7f302b))
* drop update notifier ([#706](https://github.com/google/gts/issues/706)) ([cab7704](https://github.com/google/gts/commit/cab7704389c2ba7e8e426da08397af47991d8596))
* pin prettier to 2.3.x ([#641](https://github.com/google/gts/issues/641)) ([323fb4a](https://github.com/google/gts/commit/323fb4acacc9bfc1fcba06b27135a77acc54b15a))


### Build System

* drop support for node.js 10.x ([#686](https://github.com/google/gts/issues/686)) ([12cd913](https://github.com/google/gts/commit/12cd913b6e9eb97e52b1cf3a275aadfa4517fdcb))

## [3.1.0](https://www.github.com/google/gts/compare/v3.0.3...v3.1.0) (2021-01-11)


### Features

* support comments in JSON ([#571](https://www.github.com/google/gts/issues/571)) ([cb6d2ca](https://www.github.com/google/gts/commit/cb6d2cacb5de7bcc9c8e82dd47e14fc5bf9596a3))


### Bug Fixes

* **deps:** update dependency eslint-config-prettier to v7 ([#601](https://www.github.com/google/gts/issues/601)) ([6e26681](https://www.github.com/google/gts/commit/6e266812da4b90b18e2abead9b2b5a1ca0c6654b))
* **deps:** upgrade to latest version of meow ([#616](https://www.github.com/google/gts/issues/616)) ([634bad9](https://www.github.com/google/gts/commit/634bad9bbbdb4d397bba101dc38ab14881172a30))

### [3.0.3](https://www.github.com/google/gts/compare/v3.0.2...v3.0.3) (2020-12-03)


### Bug Fixes

* **deps:** update dependency execa to v5 ([#600](https://www.github.com/google/gts/issues/600)) ([4e5f1e5](https://www.github.com/google/gts/commit/4e5f1e54facf53588bbb3b025b5240edbd7f3c8a))
* **deps:** update dependency meow to v8 ([#591](https://www.github.com/google/gts/issues/591)) ([c7e223e](https://www.github.com/google/gts/commit/c7e223e6a2ff605fabad2f8359a0385033f8de66))

### [3.0.2](https://www.github.com/google/gts/compare/v3.0.1...v3.0.2) (2020-10-26)


### Bug Fixes

* **deps:** loosen ts peer dependency ([#589](https://www.github.com/google/gts/issues/589)) ([8f1d381](https://www.github.com/google/gts/commit/8f1d381d7b166a510c42786c4a337e81b7222c84))

### [3.0.1](https://www.github.com/google/gts/compare/v3.0.0...v3.0.1) (2020-10-12)


### Bug Fixes

* **rule:** turn off @typescript-eslint/no-var-requires ([#578](https://www.github.com/google/gts/issues/578)) ([3b37229](https://www.github.com/google/gts/commit/3b37229c45969a3c53af123c69bb749578ee6b0b))

## [3.0.0](https://www.github.com/google/gts/compare/v2.0.2...v3.0.0) (2020-10-08)


### ⚠ BREAKING CHANGES

* change default `check` to `lint` (#570)
* **deps:** require TypeScript 4.x (#565)

### Features

* Add TypeScript v4 support ([#551](https://www.github.com/google/gts/issues/551)) ([0883956](https://www.github.com/google/gts/commit/08839565a1d2b4b39d532c9b0b596f01b18856fe))
* change default `check` to `lint` ([#570](https://www.github.com/google/gts/issues/570)) ([c527b66](https://www.github.com/google/gts/commit/c527b66be1ef6a78ea14b3d29225a8d7fb7097bd))
* generate .eslintignore when running init ([#521](https://www.github.com/google/gts/issues/521)) ([8bce036](https://www.github.com/google/gts/commit/8bce0368767f0c2ad7d0700deb839962bc928d16))


### Bug Fixes

* add build/.eslintrc.json to files field ([#553](https://www.github.com/google/gts/issues/553)) ([3b516ad](https://www.github.com/google/gts/commit/3b516ad5e9f0d58201dde469461db7c6ed1c1b78))
* **deps:** require TypeScript 4.x ([#565](https://www.github.com/google/gts/issues/565)) ([cbc5267](https://www.github.com/google/gts/commit/cbc5267579ef24e8c8ceaa2ef794df3ef54ea56a))
* **deps:** update dependency update-notifier to v5 ([#574](https://www.github.com/google/gts/issues/574)) ([9a882bf](https://www.github.com/google/gts/commit/9a882bf4ac30ad06e7b91a65ad5721d8e8b41c4b))
* **deps:** update typescript-eslint monorepo to v2.34.0 ([#509](https://www.github.com/google/gts/issues/509)) ([998a4ac](https://www.github.com/google/gts/commit/998a4ac9b75c97f04d8e5db37563f32d31652f23))
* **deps:** update typescript-eslint monorepo to v3 (major) ([#528](https://www.github.com/google/gts/issues/528)) ([e22e173](https://www.github.com/google/gts/commit/e22e17338db2ddb7eb829c821037c2f4e77ff869))
* **deps:** update typescript-eslint monorepo to v4 ([#556](https://www.github.com/google/gts/issues/556)) ([54148df](https://www.github.com/google/gts/commit/54148dfbd8b5f8b36a0f44f901c5db933393a661))
* better error message for broken tsconfig.json ([#501](https://www.github.com/google/gts/issues/501)) ([0c17a76](https://www.github.com/google/gts/commit/0c17a76c6650eee1d8abaff11a897a432eeaa65f))
* prohibit calls for it.only and describe.only ([#499](https://www.github.com/google/gts/issues/499)) ([071c33c](https://www.github.com/google/gts/commit/071c33ceef0e3765166aaebf6ed4698167ac0f98))

### [2.0.2](https://www.github.com/google/gts/compare/v2.0.1...v2.0.2) (2020-05-11)


### Bug Fixes

* Revert 'update dependency eslint to v7'" ([#507](https://www.github.com/google/gts/issues/507)) ([0f9950b](https://www.github.com/google/gts/commit/0f9950b273329dbcce5f3cc20864c3dcd076f08c))
* **deps:** pin release of eslint-typescript ([#508](https://www.github.com/google/gts/issues/508)) ([bd86b42](https://www.github.com/google/gts/commit/bd86b42e2bb904d3765dee82262e4691a11b9958))
* **deps:** update dependency eslint to v7 ([#504](https://www.github.com/google/gts/issues/504)) ([6aee159](https://www.github.com/google/gts/commit/6aee1595d0486ae2c7fd68d16b1b59c4c4015753))

### [2.0.1](https://www.github.com/google/gts/compare/v2.0.0...v2.0.1) (2020-05-07)


### Bug Fixes

* throw an error if running with an unsupported version of nodejs ([#493](https://www.github.com/google/gts/issues/493)) ([94fdf1e](https://www.github.com/google/gts/commit/94fdf1eaed634aa73c3e44c7a3d9f1325f773b07))
* **deps:** update dependency meow to v7 ([#502](https://www.github.com/google/gts/issues/502)) ([cf91cda](https://www.github.com/google/gts/commit/cf91cda1afab25759427511d3c97d0037d61c649))

## [2.0.0](https://www.github.com/google/gts/compare/v1.1.2...v2.0.0) (2020-04-02)

### ⚠ BREAKING CHANGES ⚠
This is a major rewrite of the tool.  Based on community guidance, we've switched from using [tslint](https://palantir.github.io/tslint/) to [eslint](https://eslint.org/).  *Please read all of the steps below to upgrade*.

#### Configuring `eslint`
With the shift to `eslint`, `gts` now will format and lint JavaScript *as well* as TypeScript. Upgrading will require a number of manual steps.  To format JavaScript and TypeScript, you can run:

```
$ npx gts fix
```

To specify only TypeScript:

```
$ npx gts fix '**/*.ts'
```

#### Delete `tslint.json`
This file is no longer used, and can lead to confusion.

#### Create a `.eslintrc.json`
Now that we're using eslint, you need to extend the eslint configuration baked into the module.  Create a new file named `.eslintrc.json`, and paste the following:
```js
{
  "extends": "./node_modules/gts"
}
```

#### Create a `.eslintignore`
The `.eslintignore` file lets you ignore specific directories.  This tool now lints and formats JavaScript, so it's _really_ important to ignore your build directory!  Here is an example of a `.eslintignore` file:

```
**/node_modules
build/
```

#### Rule changes
The underlying linter was changed, so naturally there are going to be a variety of rule changes along the way.  To see the full list, check out [.eslintrc.json](https://github.com/google/gts/blob/main/.eslintrc.json).

#### Require Node.js 10.x and up
Node.js 8.x is now end of life - this module now requires Ndoe.js 10.x and up.

### Features

* add the eol-last rule ([#425](https://www.github.com/google/gts/issues/425)) ([50ebd4d](https://www.github.com/google/gts/commit/50ebd4dbaf063615f4c025f567ca28076a734223))
* allow eslintrc to run over tsx files ([#469](https://www.github.com/google/gts/issues/469)) ([a21db94](https://www.github.com/google/gts/commit/a21db94601def563952d677cb0980a12b6730f4c))
* disable global rule for checking TODO comments ([#459](https://www.github.com/google/gts/issues/459)) ([96aa84a](https://www.github.com/google/gts/commit/96aa84a0a42181046daa248750cc8fef0c320619))
* override require-atomic-updates ([#468](https://www.github.com/google/gts/issues/468)) ([8105c93](https://www.github.com/google/gts/commit/8105c9334ee5104b05f6b1b2f150e51419637262))
* prefer single quotes if possible ([#475](https://www.github.com/google/gts/issues/475)) ([39a2705](https://www.github.com/google/gts/commit/39a2705e51b4b6329a70f91f8293a2d7a363bf5d))
* use eslint instead of tslint ([#400](https://www.github.com/google/gts/issues/400)) ([b3096fb](https://www.github.com/google/gts/commit/b3096fbd5076d302d93c2307bf627e12c423e726))


### Bug Fixes

* use .prettierrc.js ([#437](https://www.github.com/google/gts/issues/437)) ([06efa84](https://www.github.com/google/gts/commit/06efa8444cdf1064b64f3e8d61ebd04f45d90b4c))
* **deps:** update dependency chalk to v4 ([#477](https://www.github.com/google/gts/issues/477)) ([061d64e](https://www.github.com/google/gts/commit/061d64e29d37b93ce55228937cc100e05ddef352))
* **deps:** update dependency eslint-plugin-node to v11 ([#426](https://www.github.com/google/gts/issues/426)) ([a394b7c](https://www.github.com/google/gts/commit/a394b7c1f80437f25017ca5c500b968ebb789ece))
* **deps:** update dependency execa to v4 ([#427](https://www.github.com/google/gts/issues/427)) ([f42ef36](https://www.github.com/google/gts/commit/f42ef36709251553342e655e287e889df72ee3e3))
* **deps:** update dependency prettier to v2 ([#464](https://www.github.com/google/gts/issues/464)) ([20ef43d](https://www.github.com/google/gts/commit/20ef43d566df17d3c93949ef7db3b72ee9123ca3))
* disable no-use-before-define ([#431](https://www.github.com/google/gts/issues/431)) ([dea2c22](https://www.github.com/google/gts/commit/dea2c223d1d3a60a1786aa820eebb93be27016a7))
* **deps:** update dependency update-notifier to v4 ([#403](https://www.github.com/google/gts/issues/403)) ([57393b7](https://www.github.com/google/gts/commit/57393b74c6cf299e8ae09311f0382226b8baa3e3))
* **deps:** upgrade to meow 6.x ([#423](https://www.github.com/google/gts/issues/423)) ([8f93d00](https://www.github.com/google/gts/commit/8f93d0049337a832d9a22b6ae4e86fd41140ec56))
* align back to the google style guide ([#440](https://www.github.com/google/gts/issues/440)) ([8bd78c4](https://www.github.com/google/gts/commit/8bd78c4c78526a72400f618a95a987d2a7c1a8db))
* disable empty-function check ([#467](https://www.github.com/google/gts/issues/467)) ([6455d7a](https://www.github.com/google/gts/commit/6455d7a9d227320d3ffe1b00c9c739b846f339a8))
* drop support for node 8 ([#422](https://www.github.com/google/gts/issues/422)) ([888c686](https://www.github.com/google/gts/commit/888c68692079065f38ce66ec84472f1f3311a050))
* emit .prettierrc.js with init ([#462](https://www.github.com/google/gts/issues/462)) ([b114614](https://www.github.com/google/gts/commit/b114614d22ab5560d2d1dd5cb6695968cc80027b))
* enable trailing comma ([#470](https://www.github.com/google/gts/issues/470)) ([6518f58](https://www.github.com/google/gts/commit/6518f5843d3093e3beb7d3371b56d9aecedf3924))
* include *.tsx and *.jsx in default fix command ([#473](https://www.github.com/google/gts/issues/473)) ([0509780](https://www.github.com/google/gts/commit/050978005ad089d9b3b5d8895b25ea1175d75db2))

### [1.1.2](https://www.github.com/google/gts/compare/v1.1.1...v1.1.2) (2019-11-20)


### Bug Fixes

* **deps:** update to newest prettier (with support for optional chain) ([#396](https://www.github.com/google/gts/issues/396)) ([ce8ad06](https://www.github.com/google/gts/commit/ce8ad06c8489c44a9e2ed5292382637b3ebb7601))

### [1.1.1](https://www.github.com/google/gts/compare/v1.1.0...v1.1.1) (2019-11-11)


### Bug Fixes

* **deps:** update dependency chalk to v3 ([#389](https://www.github.com/google/gts/issues/389)) ([1ce0f45](https://www.github.com/google/gts/commit/1ce0f450677e143a27efc39def617d13c66503e8))
* **deps:** update dependency inquirer to v7 ([#377](https://www.github.com/google/gts/issues/377)) ([bf2c349](https://www.github.com/google/gts/commit/bf2c349b2208ac63e551542599ac9cd27b461338))
* **deps:** update dependency rimraf to v3 ([#374](https://www.github.com/google/gts/issues/374)) ([2058eaa](https://www.github.com/google/gts/commit/2058eaa682f4baae978b469fd708d1f866e7da74))
* **deps:** update dependency write-file-atomic to v3 ([#353](https://www.github.com/google/gts/issues/353)) ([59e6aa8](https://www.github.com/google/gts/commit/59e6aa8580a2f8e9457d2d2b6fa9e18e86347592))

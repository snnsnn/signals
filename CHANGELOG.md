# Changelog

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

## 7.0.0 (2024-04-19)


### ⚠ BREAKING CHANGES

* most packages have converged around the name
"signals." We'll follow suit so the same terminology can be
used when talking about them all. It also ensures new users
are familiar with what this package is about just from the name.
* Library authors can decide how to re-export bindings
from this package. The `$` prefix was used a little inconsistently so
it's best to drop it completely.
* - computed type `Computed` -> `Observable`
- observable return type is now `ObservableSubject`
- dropped `isComputed`
- `isObservable` checks readonly
- `isObservable` passes for computed observables

### Features

* `@maverick-js/observables` -> `@maverick-js/signals` ([c3b7b7d](https://github.com/maverick-js/signals/commit/c3b7b7dd08101fd1ba56f9affb4a00a94585bf63))
* `$observable` accepts dirty check option ([0c7a55d](https://github.com/maverick-js/signals/commit/0c7a55d9b71463200e90413a1d6987b00451e9ae))
* `$root` ([a70746f](https://github.com/maverick-js/signals/commit/a70746ffbdf286452b8f0379f942faa5c9a37c38))
* `computedMap` and `computedKeyedMap` ([4e9c91b](https://github.com/maverick-js/signals/commit/4e9c91b63e1ae9ab85c650553849c8b5a3d10ad1))
* `getContext` and `setContext` ([9578cd0](https://github.com/maverick-js/signals/commit/9578cd0b7a62b0838f03a0987094cb90bd254300))
* `getContext` and `setContext` accept scope arg ([980ed91](https://github.com/maverick-js/signals/commit/980ed9128dafca2649c178d8eba68cf10627da6c))
* `isObservable` ([88024da](https://github.com/maverick-js/signals/commit/88024dac825b548af6e40b78e618ec19d1e154d2))
* `onDispose` hook ([db8c142](https://github.com/maverick-js/signals/commit/db8c142625624f404fb021cc631a6cc8f5d44926))
* `onError` ([f36c1c0](https://github.com/maverick-js/signals/commit/f36c1c017061d4c20d61415bd1c74cc70da0018b))
* `scope` accepts parent arg ([4eb2760](https://github.com/maverick-js/signals/commit/4eb276005c8d21c2d1d7fedc6cac2b04f26a2bf6))
* `set` now returns newly set value ([9c2ad6f](https://github.com/maverick-js/signals/commit/9c2ad6f5785ae4b37b00a4ee29124372796f0058))
* 54% perf boost and added reactively bench ([6576447](https://github.com/maverick-js/signals/commit/65764479bd92a846cfdc84dcff3d8b3eb269dad2))
* add server bundle ([49742aa](https://github.com/maverick-js/signals/commit/49742aac0d5495126f57547aeadbd6c76bf29cd2))
* argumentless `getParent()` returns current parent ([c717439](https://github.com/maverick-js/signals/commit/c717439932a64e1c8ec6363c16b6a6aca2ce6021))
* bump scheduler to `1.0.2` ([b35f3bb](https://github.com/maverick-js/signals/commit/b35f3bb134c4c5bb2def73af0580db299c152491))
* bump scheduler to `2.0.0` ([58cf305](https://github.com/maverick-js/signals/commit/58cf305a030d7b61ce38c8d1038e7c2bbb21bb95))
* cleanup function can be returned inside `$effect` ([7a4f72f](https://github.com/maverick-js/signals/commit/7a4f72fac438010cae08d40244cd4e277995f8e6))
* complete internal rewrite focused on perf/mem improvements ([ef865f4](https://github.com/maverick-js/signals/commit/ef865f4b7dbc1fddc86e8183b8811ee850729f5e))
* export `createComputation` primitive ([8ba9f84](https://github.com/maverick-js/signals/commit/8ba9f84c85e97295543465aa917f603b9f5229d0))
* export `createScope` primitive ([7d568b4](https://github.com/maverick-js/signals/commit/7d568b47ae4c97942f6faf957c9679563453abde))
* export map functions separately from `@maverick-js/signals/map` ([f4fd01a](https://github.com/maverick-js/signals/commit/f4fd01ab1a5fdaca586721fe900b7c47acaceddd))
* expose `dispose` method on scopes ([58b0f89](https://github.com/maverick-js/signals/commit/58b0f89ef3065ecf954fb61e37b3f62d7b2fa290))
* improve type inference in `is` functions ([7cd7b92](https://github.com/maverick-js/signals/commit/7cd7b92eddce3cdaacb70100e6be021a89253e34))
* initial commit ([51cd6d5](https://github.com/maverick-js/signals/commit/51cd6d5cad05e3f1bb0f9446d29186b3b65e42b5))
* new `append` method on scopes ([ab2fcd4](https://github.com/maverick-js/signals/commit/ab2fcd48e5ac00d5ac3e0d669b0900b07d727f8a))
* new `dirty` option for `$computed` ([7ae2e6c](https://github.com/maverick-js/signals/commit/7ae2e6cb353d571e66a56c8c90ddc2e35fe126d9))
* new `isObserved` export ([1bf4cd1](https://github.com/maverick-js/signals/commit/1bf4cd1057e768de9a2f7646ed5232aa7905699b))
* new `ObservableOptions` type export ([e6aa68c](https://github.com/maverick-js/signals/commit/e6aa68c1459566ba3783ce08ff3c65cb1b42d904))
* new `onFlush` method on scheduler ([0eccb59](https://github.com/maverick-js/signals/commit/0eccb59d1781795df358d99b8d1ffb99010fd1b4))
* new `scope` export ([806e82a](https://github.com/maverick-js/signals/commit/806e82ac932cca7fdf822333318b8954d415a693))
* new `untrack` export ([a5a3fa5](https://github.com/maverick-js/signals/commit/a5a3fa58e425da7146851a7e43746eb23306f968))
* new export `getParent` ([88310aa](https://github.com/maverick-js/signals/commit/88310aadf829b984011b9fc108997701d767c8e2))
* new export `getScheduler` ([f92183b](https://github.com/maverick-js/signals/commit/f92183bcfa8c0959c0eb68b0f3efb24087a87e08))
* O(1) context and error handling ([efebd08](https://github.com/maverick-js/signals/commit/efebd08e757119d0be69a445bdac8c6f0e56aefe))
* perf/mem improvements ([2c51570](https://github.com/maverick-js/signals/commit/2c515706f18c766b6216919ece6e90a7309e15b6))
* refactor and few micro optimizations ([5f9f206](https://github.com/maverick-js/signals/commit/5f9f206412703e20b40d5e3083406d7e71601a4a))


### Bug Fixes

* `getParent` -> `getScope` ([adabf61](https://github.com/maverick-js/signals/commit/adabf61885853dc6489ced8df52c00b793f71b7b))
* `isObserved` -> `isObserving` ([7a96166](https://github.com/maverick-js/signals/commit/7a961669976cc861df8ce2ab17f40d4dfe7cfea7))
* `isObserving` now requires arg ([8fd3ade](https://github.com/maverick-js/signals/commit/8fd3ade77183136fa91fef81e978d2f1e5942279))
* `ObservabeleValue` -> `InferObservableValue` ([530ed2e](https://github.com/maverick-js/signals/commit/530ed2e59f742fe49f058296f47b0b3f51be3c78))
* `onDispose` should return dispose function if no scope ([ca04b24](https://github.com/maverick-js/signals/commit/ca04b24001d890f9b69d72e14ac7a00c9ad06348))
* `queueMicrotask` fallback will error ([0e0bea4](https://github.com/maverick-js/signals/commit/0e0bea4cfb13011cfdf121eb4c3279cb95459587)), closes [#2](https://github.com/maverick-js/signals/issues/2)
* `root` should block current observer ([119fcf1](https://github.com/maverick-js/signals/commit/119fcf1bf923569402688952af30fb183b4f3fd4))
* `root` should keep a reference to parent ([d8162ae](https://github.com/maverick-js/signals/commit/d8162ae8f5a20a14d00f0fb826219f2e5f911cd5))
* `scoped` should return value if no error is thrown ([703a6db](https://github.com/maverick-js/signals/commit/703a6db0a7dfdc6fcf8ad502ebde2d0adf1bcc24))
* `tick` is now a sync flush ([734cd4d](https://github.com/maverick-js/signals/commit/734cd4d8183f8d3948a7d493668816a28627f061))
* `tick` should not throw if called while running ([f45a59d](https://github.com/maverick-js/signals/commit/f45a59d950a8305cc6cc07ccc7e4f3d8ee7f936f))
* add `test` package export field ([1f6ea85](https://github.com/maverick-js/signals/commit/1f6ea85f76b1a8bf6ceaa8174f958d11aeb2d660))
* add context symbol description in dev ([96ea827](https://github.com/maverick-js/signals/commit/96ea827d88a9f1d9009ae64b832d2ddb426ef891))
* add few fast paths ([be1776d](https://github.com/maverick-js/signals/commit/be1776d0d59678a479556b8151271c2e25557c89))
* add symbol descriptions in dev ([298410a](https://github.com/maverick-js/signals/commit/298410a1651e57c68ac63854d19e85476bbdc7d0))
* additional parent tracking variable not required ([9df21ee](https://github.com/maverick-js/signals/commit/9df21ee0d104d1da85aa28ebebd7925c1995e56a))
* all types extend observable ([bef215c](https://github.com/maverick-js/signals/commit/bef215c1ec98cb3593e1f9daea71bb6b6974ee2f))
* allow effects to run server-side ([e50a1d6](https://github.com/maverick-js/signals/commit/e50a1d6d6bcdb9ea1742500cf0b86132765a0449)), closes [#20](https://github.com/maverick-js/signals/issues/20)
* allow fallback to be set if computed init error ([2cd85b2](https://github.com/maverick-js/signals/commit/2cd85b27bbd58df00ef5dbda43e08d4faf900101))
* append scopes correctly ([03cfc71](https://github.com/maverick-js/signals/commit/03cfc71b77bcf07d271aaf991c9c47c42a26698d))
* attach context/handlers in `scope.append` ([26f1f09](https://github.com/maverick-js/signals/commit/26f1f09990b59387667952e745f5e003044df5ea))
* auto-dispose computed if no observers ([0ab5855](https://github.com/maverick-js/signals/commit/0ab5855eb27dfcbe4fd5f5290fe725f6d0d76ebf))
* avoid recursion while performing work ([a8024bb](https://github.com/maverick-js/signals/commit/a8024bb15f3094eb88d2e6537c523ae641528eeb))
* avoid stack overflow in prod ([4cba856](https://github.com/maverick-js/signals/commit/4cba85621a693a8b3afb6f2a0fe663ec06384d31))
* avoid unnecessary scheduling while flushing ([6c876d6](https://github.com/maverick-js/signals/commit/6c876d61c862c1b5faa3dd17a17a85e73b995358))
* check prev sibling exists during dispose ([46ee520](https://github.com/maverick-js/signals/commit/46ee5200994e1a04d38c7054464d2778aa9ae1be))
* clean up callable types ([aa01378](https://github.com/maverick-js/signals/commit/aa01378112d034865a7d7c009ff5d321274ca9a9))
* clean up computation if error is thrown ([eba7b9a](https://github.com/maverick-js/signals/commit/eba7b9a417fe86d65b3d49442494fa32630355bb))
* clean up selector implementation ([7f85df4](https://github.com/maverick-js/signals/commit/7f85df4d3b2e818e9dd384339f9a1a69a0d70745))
* clear error handlers before each computed run ([8a716cd](https://github.com/maverick-js/signals/commit/8a716cd6cff592e5624dcee8a493bfd645fdec8f))
* completely remove next sibling reference on dispose ([f675a14](https://github.com/maverick-js/signals/commit/f675a14b1069824b387935cfdcbbc63258b6db3d))
* consistent empty disposals order ([3459a1a](https://github.com/maverick-js/signals/commit/3459a1a49bb9addaed4898fa4ad63d9b0c4ad622))
* deprecate and remove `isObserving` ([3c9e46f](https://github.com/maverick-js/signals/commit/3c9e46f3c70af5d899cf6e7a8d5c060a7b412c0a))
* detect zombie effects ([052b9c7](https://github.com/maverick-js/signals/commit/052b9c7209462798e154a2996fcffe7126b50976))
* dispose appended scopes correctly ([7c80b49](https://github.com/maverick-js/signals/commit/7c80b49875bb1dd525b765667b1757fb21cf9a6f))
* dispose cells at the end of each cellx benchmark run ([9c63d4b](https://github.com/maverick-js/signals/commit/9c63d4b83b2fe82868281a120d65cf63e6fbf15a))
* dispose conditional nested effects ([f06756c](https://github.com/maverick-js/signals/commit/f06756c7500c8e1306a1c094011a5f3cd6a912ef))
* do not empty disposal on non-dirty child computations ([86b2d75](https://github.com/maverick-js/signals/commit/86b2d75075b7c494636bf1127d3776bdc2989682))
* dont dispose of children on update ([a39679d](https://github.com/maverick-js/signals/commit/a39679d1ddb9b825a9e3fa8f33dc56f0bab18c43))
* dont need safe inequality check ([368af0c](https://github.com/maverick-js/signals/commit/368af0ccc594654defe619763935376abbdfb56c))
* dont treat setting functional signal values differently ([3b4b9d2](https://github.com/maverick-js/signals/commit/3b4b9d2f1cf00768eba06e981c382be32542dd52))
* drop `$` prefix on exports ([a18149b](https://github.com/maverick-js/signals/commit/a18149b929d7471f5d00597674aa1f0e5728c11a)), closes [#4](https://github.com/maverick-js/signals/issues/4) [#issuecomment-1171106602](https://github.com/maverick-js/signals/issues/issuecomment-1171106602)
* drop deprecated `getParent` ([6a1b64d](https://github.com/maverick-js/signals/commit/6a1b64d4a085d6a8c7bd428a0c82c7418989d755))
* drop deprecated `isObserved` ([a7d169a](https://github.com/maverick-js/signals/commit/a7d169a32b1d947b1d8f80d8d85399258a738069))
* effect should run all disposals on each new run ([3217217](https://github.com/maverick-js/signals/commit/3217217a85c232e6e0311d31ea3fd9d9b25db825))
* exclude `@maverick-js/scheduler` from bundle (external) ([2f37a04](https://github.com/maverick-js/signals/commit/2f37a0448a2f62fe52f23bfc936c11fbb60ef338))
* export `SCOPE` symbol ([a00ace7](https://github.com/maverick-js/signals/commit/a00ace7bc184bc977b7dcf21fcb75fcb198813e0))
* export `SCOPE` symbol so it can be set externally ([43f451c](https://github.com/maverick-js/signals/commit/43f451c1a6f45cdda06de9b3209d491ce0ddcfbc))
* extend context/handlers on late scope append ([905ba92](https://github.com/maverick-js/signals/commit/905ba92b1d5c6442c140e1e86049f94aab51cd57))
* fix sinuous benchmarks ([f55e188](https://github.com/maverick-js/signals/commit/f55e1881eb01f93aa8762f6118774c98be426da1))
* forward error re-throw to parent handler ([5034795](https://github.com/maverick-js/signals/commit/50347954e37314f72f84661aebebcbe649c4e899))
* general error handling improvements ([3b7095f](https://github.com/maverick-js/signals/commit/3b7095f8cbde680f8dce00e959f40b021535c2d3))
* identify signals using symbol ([c43326e](https://github.com/maverick-js/signals/commit/c43326e1ae771d2a8027f97ff073082eaefb2aab))
* include declaration files as-is in dist ([0fd383e](https://github.com/maverick-js/signals/commit/0fd383e3441fe4a65a9e6ce7595193d89156e3c6))
* incorrect recursive parent tracking ([7390155](https://github.com/maverick-js/signals/commit/7390155f7a5e8be85c7d2fc8d06c4c261dc43437))
* it should not throw on dispose call during active disposal ([09eb2a7](https://github.com/maverick-js/signals/commit/09eb2a7a2b0b74e5bccb804e1234c5f8aa4ae379))
* keep child computations alive on update ([f4b1d2d](https://github.com/maverick-js/signals/commit/f4b1d2d6651da0692fdb77c8ac30c6a803710b9e)), closes [#4](https://github.com/maverick-js/signals/issues/4)
* let cellx release its global pendingCells array between benchmarks ([0a02af1](https://github.com/maverick-js/signals/commit/0a02af19b6e966404ed0f134dde578e52fa27b14))
* locally scope compute prev tracking variables ([8305d52](https://github.com/maverick-js/signals/commit/8305d5273ce326151928fa932a42516069540765))
* log error if computed throws on first run ([8582879](https://github.com/maverick-js/signals/commit/8582879caa2c930d5990607074748695c6bb9bbc))
* make `untrack` a single fn call ([3972e40](https://github.com/maverick-js/signals/commit/3972e40cebcf642717e63251492df432c5e34fb0))
* mem leak during disposal ([09ebc3c](https://github.com/maverick-js/signals/commit/09ebc3cb4fe50034ad29e3636bdcadcf193d5e04))
* memory improvements ([32aa98f](https://github.com/maverick-js/signals/commit/32aa98f8b81ca8f74ab70b1f22366ff28e3f8000))
* more faithful port of reactively for stability ([f7d78f9](https://github.com/maverick-js/signals/commit/f7d78f9d72c6cde4ef30dc1188c15e7f3bae7a6c))
* move scheduler to separate package ([83120d7](https://github.com/maverick-js/signals/commit/83120d7662daaf5e7ac2fe0ac0cceda26f80f1c5))
* only clean computation on throw if still dirty after handling ([d465f02](https://github.com/maverick-js/signals/commit/d465f02a28726eb90a68c7a67337f680aaeae1d6))
* only dispose needed parts ([a3db078](https://github.com/maverick-js/signals/commit/a3db078c366b7e4f4350f09cbd06b309ccd10953))
* only provide dispose function to `root` if needed ([88b550f](https://github.com/maverick-js/signals/commit/88b550f391873edecb992255758932327db7ec17))
* only run `runTop` on effects ([d5342fe](https://github.com/maverick-js/signals/commit/d5342fe777d4ea8a56271ef3e2d0283e7aae8634))
* only track observed by if not same scope ([d609fef](https://github.com/maverick-js/signals/commit/d609fef7d2b771d36876639d01e416ebb5d2d9c9))
* option to silence computed init error ([7b98328](https://github.com/maverick-js/signals/commit/7b98328db844d79a4cf4a70e44bbfd6a005e2136))
* parent should be determined on creation ([117fa5b](https://github.com/maverick-js/signals/commit/117fa5bc77dc84970f262801887238d3e5ead4c7))
* port over `runTop` fix from x-reactivity ([ec66f8c](https://github.com/maverick-js/signals/commit/ec66f8c9e2e7491ec2bdb2041489e1ccad0a38ac))
* port over deep deterministic disposal ([66974e5](https://github.com/maverick-js/signals/commit/66974e53b4ac888e24d0313888a5fd2ecbabbe72))
* prefer named functions over anon for debugging ([e57a0cf](https://github.com/maverick-js/signals/commit/e57a0cfcab09025ef1a5e4cc4ebee5c6f8bcfeb5))
* prevent infinite `getParent` recursion (attempt 2) ([b600c7a](https://github.com/maverick-js/signals/commit/b600c7ac6bb0d68c9ad9a08c1f161c0a8dfdf270))
* prevent infinite recursion when nesting `getParent` calls ([68d850d](https://github.com/maverick-js/signals/commit/68d850dfbaeeb922bce86739f35c17bbdc3ddd83))
* production node export field blocking dev ([b1e52a8](https://github.com/maverick-js/signals/commit/b1e52a80100e18b67655d8df7cc75ced4de872df))
* refactor dispose types ([33aae66](https://github.com/maverick-js/signals/commit/33aae6658d5a904687b1c9803a911d6b58c29c85))
* remove auto-dispose perf overhead ([bbbbbe6](https://github.com/maverick-js/signals/commit/bbbbbe634a04e42fa91d3d4eb16ede33343ca58e))
* remove child from parent set on dispose ([4fcbaec](https://github.com/maverick-js/signals/commit/4fcbaec39dd37cd5cfb8df17d56b065c9ffd01c3))
* remove redundant `unrefSet` calls ([778b8ee](https://github.com/maverick-js/signals/commit/778b8ee360d9c4ce3174f5d8d779b54bd96e1478))
* remove redundant try/catch in queued task ([c95e02e](https://github.com/maverick-js/signals/commit/c95e02ea461c088c0898eb45968fb888aa806454))
* remove redundant types exports ([06e5f26](https://github.com/maverick-js/signals/commit/06e5f26d32f24d0d7f3f0225262ada87584a101f))
* rename `update()` to `next()` ([323f20e](https://github.com/maverick-js/signals/commit/323f20e8d491461dce873e999c6a4447274b9b7a))
* rename type `ObservableSubject` -> `Subject` ([32e4a24](https://github.com/maverick-js/signals/commit/32e4a24dd00b376ab108ba872e562f67e135689d))
* revert a39679d1ddb9b825a9e3fa8f33dc56f0bab18c43 ([88c5dbe](https://github.com/maverick-js/signals/commit/88c5dbe26c312c86c1663a71562ea1bfe1a0fad5))
* rework `scope` and rename to `scoped` ([f5e1789](https://github.com/maverick-js/signals/commit/f5e1789bd5004b6bc00021d184bb17512b9ffb26))
* root dispose type should be function ([da040b3](https://github.com/maverick-js/signals/commit/da040b3237b621bc4b2f26f2b5a3f8643d025681))
* root should not add any observers ([36baad2](https://github.com/maverick-js/signals/commit/36baad202538bf0f0effebd6bd5118bcdcf076d0))
* run disposal last in first out ([2bfc3ff](https://github.com/maverick-js/signals/commit/2bfc3ff95d83d160db590cb2835a6e27712f17e4))
* scheduler task index tracking should not start from 0 ([f9e868a](https://github.com/maverick-js/signals/commit/f9e868a6939ee5eba172313266b42e91fb3398ee))
* scope computeds by default to avoid potential mem leaks ([45422e8](https://github.com/maverick-js/signals/commit/45422e8871ff167ad606cc335dddc5d7da888f4b)), closes [#15](https://github.com/maverick-js/signals/issues/15) [#16](https://github.com/maverick-js/signals/issues/16)
* scoped function can return value ([c1d13c8](https://github.com/maverick-js/signals/commit/c1d13c85590fb7e52e2d1acbca25af72d89840c8))
* scoped function should still be observable ([0c1d2ea](https://github.com/maverick-js/signals/commit/0c1d2ea334db68cb22e91a8571b35867ab0cbeb3))
* second argument to observables is an options object (prev debug id) ([d0c31e7](https://github.com/maverick-js/signals/commit/d0c31e745867283e190a6c1626c8156b624aeeda))
* separate import/require package exports ([d65ed6f](https://github.com/maverick-js/signals/commit/d65ed6f6adea3744c5e68cc3a2e8e4bfc0efedcc))
* set computation value to any to avoid type conflicts ([57477e4](https://github.com/maverick-js/signals/commit/57477e4e0bd2beff62da86486e5ee0fd057edb64))
* set effect result tracking to null when done ([1e9f057](https://github.com/maverick-js/signals/commit/1e9f0574f6b177d4d24c78362aca4df005087989))
* simplify `peek` and `untrack` ([383f717](https://github.com/maverick-js/signals/commit/383f7179154028b8aa35df204a88194898abf9df))
* simplify `scope` ([b2867d1](https://github.com/maverick-js/signals/commit/b2867d1018de2794721e4a4ce2de243f6e54d65a))
* simplify effect child disposal ([0feced4](https://github.com/maverick-js/signals/commit/0feced47e9ee68df7709f17d3ada3245d9205bc1))
* simplify setting functional signals ([f276131](https://github.com/maverick-js/signals/commit/f276131bb5c7d50f2ccfca41461b9380a022273a))
* small perf boost `class` -> prototype functions ([ec6d77c](https://github.com/maverick-js/signals/commit/ec6d77cfbc02b1fe1a518a5f4a956f2e19bcfaf5))
* stop observing computed after its disposed ([c2daca8](https://github.com/maverick-js/signals/commit/c2daca8ae29bdae7de08b815626eb7233283b8dd))
* throw error up if no handler is defined ([a0a1f1a](https://github.com/maverick-js/signals/commit/a0a1f1a4877e7e5dc041e81bfe2099e234091734))
* throw errors that are not handled ([69070c3](https://github.com/maverick-js/signals/commit/69070c376f79b0c8b486f4ac1f76daf12f29efc5))
* track only current observers on each run ([1f1d818](https://github.com/maverick-js/signals/commit/1f1d818cf6e9676d4db0a4e72fa3ab1dcb597ab5))
* track parent across peeks ([af4d561](https://github.com/maverick-js/signals/commit/af4d5615d78560f75ecea780a15ee46c33049719))
* track parent separately to handle disposals correctly ([50110d4](https://github.com/maverick-js/signals/commit/50110d4d8fa590310a24d3e9b4433463c455c189))
* update computed map docs ([0bbf814](https://github.com/maverick-js/signals/commit/0bbf8149ce52ae3ffe4f790675dc00b4d72e0b2c))
* use array scope disposal ([c9c740c](https://github.com/maverick-js/signals/commit/c9c740ccedc5cf2785cbd81d9a61b8e09b0849c0))
* use mangle cache ([f0995cf](https://github.com/maverick-js/signals/commit/f0995cf8a2222599651f749149013f46bfd83553))
* use rollup for cleaner build output ([8f232fb](https://github.com/maverick-js/signals/commit/8f232fb29246c7cd3159bdf552bbfc57ec096cde))
* use set so error handlers are only added once ([68c75ab](https://github.com/maverick-js/signals/commit/68c75ab0f7a1a8661592183d4c947600c3231b37))
* use ts interface over type alias where possible ([1464490](https://github.com/maverick-js/signals/commit/1464490d130010e939cb9182fbad9b7d4462659b))

## [6.0.0](https://github.com/maverick-js/signals/compare/v5.11.5...v6.0.0) (2024-19-04)


### ⚠ BREAKING CHANGES

* automatic error coersion is removed from the error handlers.
Now, re-thrown errors are passed to the next handler as is.

### [5.11.5](https://github.com/maverick-js/signals/compare/v5.11.4...v5.11.5) (2024-04-09)


### Bug Fixes

* use array scope disposal ([c9c740c](https://github.com/maverick-js/signals/commit/c9c740ccedc5cf2785cbd81d9a61b8e09b0849c0))

### [5.11.4](https://github.com/maverick-js/signals/compare/v5.11.3...v5.11.4) (2023-09-13)


### Bug Fixes

* completely remove next sibling reference on dispose ([f675a14](https://github.com/maverick-js/signals/commit/f675a14b1069824b387935cfdcbbc63258b6db3d))

### [5.11.3](https://github.com/maverick-js/signals/compare/v5.11.2...v5.11.3) (2023-09-13)


### Bug Fixes

* dispose appended scopes correctly ([7c80b49](https://github.com/maverick-js/signals/commit/7c80b49875bb1dd525b765667b1757fb21cf9a6f))

### [5.11.2](https://github.com/maverick-js/signals/compare/v5.11.1...v5.11.2) (2023-06-22)


### Bug Fixes

* identify signals using symbol ([c43326e](https://github.com/maverick-js/signals/commit/c43326e1ae771d2a8027f97ff073082eaefb2aab))

### [5.11.1](https://github.com/maverick-js/signals/compare/v5.11.0...v5.11.1) (2023-06-19)


### Bug Fixes

* run disposal last in first out ([2bfc3ff](https://github.com/maverick-js/signals/commit/2bfc3ff95d83d160db590cb2835a6e27712f17e4))

## [5.11.0](https://github.com/maverick-js/signals/compare/v5.10.5...v5.11.0) (2023-06-18)


### Features

* expose `dispose` method on scopes ([58b0f89](https://github.com/maverick-js/signals/commit/58b0f89ef3065ecf954fb61e37b3f62d7b2fa290))


### Bug Fixes

* extend context/handlers on late scope append ([905ba92](https://github.com/maverick-js/signals/commit/905ba92b1d5c6442c140e1e86049f94aab51cd57))
* throw error up if no handler is defined ([a0a1f1a](https://github.com/maverick-js/signals/commit/a0a1f1a4877e7e5dc041e81bfe2099e234091734))

### [5.10.5](https://github.com/maverick-js/signals/compare/v5.10.4...v5.10.5) (2023-06-14)


### Bug Fixes

* use mangle cache ([f0995cf](https://github.com/maverick-js/signals/commit/f0995cf8a2222599651f749149013f46bfd83553))

### [5.10.4](https://github.com/maverick-js/signals/compare/v5.10.3...v5.10.4) (2023-06-12)


### Bug Fixes

* use rollup for cleaner build output ([8f232fb](https://github.com/maverick-js/signals/commit/8f232fb29246c7cd3159bdf552bbfc57ec096cde))

### [5.10.3](https://github.com/maverick-js/signals/compare/v5.10.2...v5.10.3) (2023-06-03)


### Bug Fixes

* allow effects to run server-side ([e50a1d6](https://github.com/maverick-js/signals/commit/e50a1d6d6bcdb9ea1742500cf0b86132765a0449)), closes [#20](https://github.com/maverick-js/signals/issues/20)
* mem leak during disposal ([09ebc3c](https://github.com/maverick-js/signals/commit/09ebc3cb4fe50034ad29e3636bdcadcf193d5e04))

### [5.10.2](https://github.com/maverick-js/signals/compare/v5.10.1...v5.10.2) (2023-05-08)


### Bug Fixes

* throw errors that are not handled ([69070c3](https://github.com/maverick-js/signals/commit/69070c376f79b0c8b486f4ac1f76daf12f29efc5))

### [5.10.1](https://github.com/maverick-js/signals/compare/v5.10.0...v5.10.1) (2023-05-08)


### Bug Fixes

* attach context/handlers in `scope.append` ([26f1f09](https://github.com/maverick-js/signals/commit/26f1f09990b59387667952e745f5e003044df5ea))

## [5.10.0](https://github.com/maverick-js/signals/compare/v5.9.4...v5.10.0) (2023-05-08)


### Features

* O(1) context and error handling ([efebd08](https://github.com/maverick-js/signals/commit/efebd08e757119d0be69a445bdac8c6f0e56aefe))

### [5.9.4](https://github.com/maverick-js/signals/compare/v5.9.3...v5.9.4) (2023-04-26)


### Bug Fixes

* port over deep deterministic disposal ([66974e5](https://github.com/maverick-js/signals/commit/66974e53b4ac888e24d0313888a5fd2ecbabbe72))

### [5.9.3](https://github.com/maverick-js/signals/compare/v5.9.2...v5.9.3) (2023-04-17)


### Bug Fixes

* only run `runTop` on effects ([d5342fe](https://github.com/maverick-js/signals/commit/d5342fe777d4ea8a56271ef3e2d0283e7aae8634))
* simplify `peek` and `untrack` ([383f717](https://github.com/maverick-js/signals/commit/383f7179154028b8aa35df204a88194898abf9df))

### [5.9.2](https://github.com/maverick-js/signals/compare/v5.9.1...v5.9.2) (2023-04-12)


### Bug Fixes

* port over `runTop` fix from x-reactivity ([ec66f8c](https://github.com/maverick-js/signals/commit/ec66f8c9e2e7491ec2bdb2041489e1ccad0a38ac))

### [5.9.1](https://github.com/maverick-js/signals/compare/v5.9.0...v5.9.1) (2023-01-23)


### Bug Fixes

* `scoped` should return value if no error is thrown ([703a6db](https://github.com/maverick-js/signals/commit/703a6db0a7dfdc6fcf8ad502ebde2d0adf1bcc24))

## [5.9.0](https://github.com/maverick-js/signals/compare/v5.8.0...v5.9.0) (2023-01-22)


### Features

* export `createComputation` primitive ([8ba9f84](https://github.com/maverick-js/signals/commit/8ba9f84c85e97295543465aa917f603b9f5229d0))
* export `createScope` primitive ([7d568b4](https://github.com/maverick-js/signals/commit/7d568b47ae4c97942f6faf957c9679563453abde))

## [5.8.0](https://github.com/maverick-js/signals/compare/v5.7.4...v5.8.0) (2023-01-22)


### Features

* `getContext` and `setContext` accept scope arg ([980ed91](https://github.com/maverick-js/signals/commit/980ed9128dafca2649c178d8eba68cf10627da6c))

### [5.7.4](https://github.com/maverick-js/signals/compare/v5.7.3...v5.7.4) (2023-01-22)


### Bug Fixes

* scope computeds by default to avoid potential mem leaks ([45422e8](https://github.com/maverick-js/signals/commit/45422e8871ff167ad606cc335dddc5d7da888f4b)), closes [#15](https://github.com/maverick-js/signals/issues/15) [#16](https://github.com/maverick-js/signals/issues/16)

### [5.7.3](https://github.com/maverick-js/signals/compare/v5.7.2...v5.7.3) (2023-01-22)


### Bug Fixes

* only clean computation on throw if still dirty after handling ([d465f02](https://github.com/maverick-js/signals/commit/d465f02a28726eb90a68c7a67337f680aaeae1d6))

### [5.7.2](https://github.com/maverick-js/signals/compare/v5.7.1...v5.7.2) (2023-01-17)


### Bug Fixes

* append scopes correctly ([03cfc71](https://github.com/maverick-js/signals/commit/03cfc71b77bcf07d271aaf991c9c47c42a26698d))

### [5.7.1](https://github.com/maverick-js/signals/compare/v5.7.0...v5.7.1) (2023-01-17)


### Bug Fixes

* check prev sibling exists during dispose ([46ee520](https://github.com/maverick-js/signals/commit/46ee5200994e1a04d38c7054464d2778aa9ae1be))
* clean up computation if error is thrown ([eba7b9a](https://github.com/maverick-js/signals/commit/eba7b9a417fe86d65b3d49442494fa32630355bb))
* it should not throw on dispose call during active disposal ([09eb2a7](https://github.com/maverick-js/signals/commit/09eb2a7a2b0b74e5bccb804e1234c5f8aa4ae379))

## [5.7.0](https://github.com/maverick-js/signals/compare/v5.6.5...v5.7.0) (2023-01-17)


### Features

* new `append` method on scopes ([ab2fcd4](https://github.com/maverick-js/signals/commit/ab2fcd48e5ac00d5ac3e0d669b0900b07d727f8a))

### [5.6.5](https://github.com/maverick-js/signals/compare/v5.6.4...v5.6.5) (2023-01-09)


### Bug Fixes

* add `test` package export field ([1f6ea85](https://github.com/maverick-js/signals/commit/1f6ea85f76b1a8bf6ceaa8174f958d11aeb2d660))

### [5.6.4](https://github.com/maverick-js/signals/compare/v5.6.3...v5.6.4) (2023-01-09)


### Bug Fixes

* separate import/require package exports ([d65ed6f](https://github.com/maverick-js/signals/commit/d65ed6f6adea3744c5e68cc3a2e8e4bfc0efedcc))

### [5.6.3](https://github.com/maverick-js/signals/compare/v5.6.2...v5.6.3) (2023-01-08)


### Bug Fixes

* remove redundant types exports ([06e5f26](https://github.com/maverick-js/signals/commit/06e5f26d32f24d0d7f3f0225262ada87584a101f))

### [5.6.2](https://github.com/maverick-js/signals/compare/v5.6.1...v5.6.2) (2023-01-08)


### Bug Fixes

* export `SCOPE` symbol so it can be set externally ([43f451c](https://github.com/maverick-js/signals/commit/43f451c1a6f45cdda06de9b3209d491ce0ddcfbc))

### [5.6.1](https://github.com/maverick-js/signals/compare/v5.6.0...v5.6.1) (2023-01-08)


### Bug Fixes

* include declaration files as-is in dist ([0fd383e](https://github.com/maverick-js/signals/commit/0fd383e3441fe4a65a9e6ce7595193d89156e3c6))

## [5.6.0](https://github.com/maverick-js/signals/compare/v5.5.1...v5.6.0) (2023-01-06)


### Features

* add server bundle ([49742aa](https://github.com/maverick-js/signals/commit/49742aac0d5495126f57547aeadbd6c76bf29cd2))

### [5.5.1](https://github.com/maverick-js/signals/compare/v5.5.0...v5.5.1) (2023-01-05)


### Bug Fixes

* more faithful port of reactively for stability ([f7d78f9](https://github.com/maverick-js/signals/commit/f7d78f9d72c6cde4ef30dc1188c15e7f3bae7a6c))

## [5.5.0](https://github.com/maverick-js/signals/compare/v5.4.2...v5.5.0) (2023-01-03)


### Features

* export map functions separately from `@maverick-js/signals/map` ([f4fd01a](https://github.com/maverick-js/signals/commit/f4fd01ab1a5fdaca586721fe900b7c47acaceddd))


### Bug Fixes

* dont treat setting functional signal values differently ([3b4b9d2](https://github.com/maverick-js/signals/commit/3b4b9d2f1cf00768eba06e981c382be32542dd52))

### [5.4.2](https://github.com/maverick-js/signals/compare/v5.4.1...v5.4.2) (2023-01-02)


### Bug Fixes

* refactor dispose types ([33aae66](https://github.com/maverick-js/signals/commit/33aae6658d5a904687b1c9803a911d6b58c29c85))

### [5.4.1](https://github.com/maverick-js/signals/compare/v5.4.0...v5.4.1) (2023-01-02)


### Bug Fixes

* memory improvements ([32aa98f](https://github.com/maverick-js/signals/commit/32aa98f8b81ca8f74ab70b1f22366ff28e3f8000))

## [5.4.0](https://github.com/maverick-js/signals/compare/v5.3.0...v5.4.0) (2023-01-01)


### Features

* refactor and few micro optimizations ([5f9f206](https://github.com/maverick-js/signals/commit/5f9f206412703e20b40d5e3083406d7e71601a4a))


### Bug Fixes

* clean up callable types ([aa01378](https://github.com/maverick-js/signals/commit/aa01378112d034865a7d7c009ff5d321274ca9a9))
* root dispose type should be function ([da040b3](https://github.com/maverick-js/signals/commit/da040b3237b621bc4b2f26f2b5a3f8643d025681))
* small perf boost `class` -> prototype functions ([ec6d77c](https://github.com/maverick-js/signals/commit/ec6d77cfbc02b1fe1a518a5f4a956f2e19bcfaf5))

## [5.3.0](https://github.com/maverick-js/signals/compare/v5.2.0...v5.3.0) (2022-12-30)


### Features

* perf/mem improvements ([2c51570](https://github.com/maverick-js/signals/commit/2c515706f18c766b6216919ece6e90a7309e15b6))

## [5.2.0](https://github.com/maverick-js/signals/compare/v5.1.7...v5.2.0) (2022-12-29)


### Features

* `set` now returns newly set value ([9c2ad6f](https://github.com/maverick-js/signals/commit/9c2ad6f5785ae4b37b00a4ee29124372796f0058))


### Bug Fixes

* only provide dispose function to `root` if needed ([88b550f](https://github.com/maverick-js/signals/commit/88b550f391873edecb992255758932327db7ec17))
* production node export field blocking dev ([b1e52a8](https://github.com/maverick-js/signals/commit/b1e52a80100e18b67655d8df7cc75ced4de872df))
* scheduler task index tracking should not start from 0 ([f9e868a](https://github.com/maverick-js/signals/commit/f9e868a6939ee5eba172313266b42e91fb3398ee))

### [5.1.7](https://github.com/maverick-js/signals/compare/v5.1.6...v5.1.7) (2022-12-29)


### Bug Fixes

* `root` should block current observer ([119fcf1](https://github.com/maverick-js/signals/commit/119fcf1bf923569402688952af30fb183b4f3fd4))

### [5.1.6](https://github.com/maverick-js/signals/compare/v5.1.5...v5.1.6) (2022-12-28)


### Bug Fixes

* avoid recursion while performing work ([a8024bb](https://github.com/maverick-js/signals/commit/a8024bb15f3094eb88d2e6537c523ae641528eeb))
* avoid unnecessary scheduling while flushing ([6c876d6](https://github.com/maverick-js/signals/commit/6c876d61c862c1b5faa3dd17a17a85e73b995358))

### [5.1.5](https://github.com/maverick-js/signals/compare/v5.1.4...v5.1.5) (2022-12-28)


### Bug Fixes

* add few fast paths ([be1776d](https://github.com/maverick-js/signals/commit/be1776d0d59678a479556b8151271c2e25557c89))

### [5.1.4](https://github.com/maverick-js/signals/compare/v5.1.3...v5.1.4) (2022-12-28)


### Bug Fixes

* clean up selector implementation ([7f85df4](https://github.com/maverick-js/signals/commit/7f85df4d3b2e818e9dd384339f9a1a69a0d70745))

### [5.1.3](https://github.com/maverick-js/signals/compare/v5.1.2...v5.1.3) (2022-12-27)


### Bug Fixes

* detect zombie effects ([052b9c7](https://github.com/maverick-js/signals/commit/052b9c7209462798e154a2996fcffe7126b50976))

### [5.1.2](https://github.com/maverick-js/signals/compare/v5.1.1...v5.1.2) (2022-12-27)


### Bug Fixes

* simplify setting functional signals ([f276131](https://github.com/maverick-js/signals/commit/f276131bb5c7d50f2ccfca41461b9380a022273a))

### [5.1.1](https://github.com/maverick-js/signals/compare/v5.1.0...v5.1.1) (2022-12-26)


### Bug Fixes

* set computation value to any to avoid type conflicts ([57477e4](https://github.com/maverick-js/signals/commit/57477e4e0bd2beff62da86486e5ee0fd057edb64))

## [5.1.0](https://github.com/maverick-js/signals/compare/v5.0.7...v5.1.0) (2022-12-26)


### Features

* complete internal rewrite focused on perf/mem improvements ([ef865f4](https://github.com/maverick-js/signals/commit/ef865f4b7dbc1fddc86e8183b8811ee850729f5e))

### [5.0.7](https://github.com/maverick-js/signals/compare/v5.0.6...v5.0.7) (2022-12-11)


### Bug Fixes

* export `SCOPE` symbol ([a00ace7](https://github.com/maverick-js/signals/commit/a00ace7bc184bc977b7dcf21fcb75fcb198813e0))

### [5.0.6](https://github.com/maverick-js/signals/compare/v5.0.5...v5.0.6) (2022-12-09)


### Bug Fixes

* rework `scope` and rename to `scoped` ([f5e1789](https://github.com/maverick-js/signals/commit/f5e1789bd5004b6bc00021d184bb17512b9ffb26))

### [5.0.5](https://github.com/maverick-js/signals/compare/v5.0.4...v5.0.5) (2022-12-09)


### Bug Fixes

* locally scope compute prev tracking variables ([8305d52](https://github.com/maverick-js/signals/commit/8305d5273ce326151928fa932a42516069540765))

### [5.0.4](https://github.com/maverick-js/signals/compare/v5.0.3...v5.0.4) (2022-12-09)


### Bug Fixes

* simplify `scope` ([b2867d1](https://github.com/maverick-js/signals/commit/b2867d1018de2794721e4a4ce2de243f6e54d65a))

### [5.0.3](https://github.com/maverick-js/signals/compare/v5.0.2...v5.0.3) (2022-12-09)


### Bug Fixes

* `tick` should not throw if called while running ([f45a59d](https://github.com/maverick-js/signals/commit/f45a59d950a8305cc6cc07ccc7e4f3d8ee7f936f))

### [5.0.2](https://github.com/maverick-js/signals/compare/v5.0.1...v5.0.2) (2022-12-09)


### Bug Fixes

* make `untrack` a single fn call ([3972e40](https://github.com/maverick-js/signals/commit/3972e40cebcf642717e63251492df432c5e34fb0))
* prefer named functions over anon for debugging ([e57a0cf](https://github.com/maverick-js/signals/commit/e57a0cfcab09025ef1a5e4cc4ebee5c6f8bcfeb5))

### [5.0.1](https://github.com/maverick-js/signals/compare/v5.0.0...v5.0.1) (2022-12-08)


### Bug Fixes

* `tick` is now a sync flush ([734cd4d](https://github.com/maverick-js/signals/commit/734cd4d8183f8d3948a7d493668816a28627f061))
* set effect result tracking to null when done ([1e9f057](https://github.com/maverick-js/signals/commit/1e9f0574f6b177d4d24c78362aca4df005087989))

## [5.0.0](https://github.com/maverick-js/signals/compare/v4.10.0...v5.0.0) (2022-12-06)


### ⚠ BREAKING CHANGES

* most packages have converged around the name
"signals." We'll follow suit so the same terminology can be
used when talking about them all. It also ensures new users
are familiar with what this package is about just from the name.

### Features

* `@maverick-js/observables` -> `@maverick-js/signals` ([c3b7b7d](https://github.com/maverick-js/signals/commit/c3b7b7dd08101fd1ba56f9affb4a00a94585bf63))
* 54% perf boost and added reactively bench ([6576447](https://github.com/maverick-js/signals/commit/65764479bd92a846cfdc84dcff3d8b3eb269dad2))


### Bug Fixes

* `ObservabeleValue` -> `InferObservableValue` ([530ed2e](https://github.com/maverick-js/signals/commit/530ed2e59f742fe49f058296f47b0b3f51be3c78))
* deprecate and remove `isObserving` ([3c9e46f](https://github.com/maverick-js/signals/commit/3c9e46f3c70af5d899cf6e7a8d5c060a7b412c0a))
* rename type `ObservableSubject` -> `Subject` ([32e4a24](https://github.com/maverick-js/signals/commit/32e4a24dd00b376ab108ba872e562f67e135689d))
* use ts interface over type alias where possible ([1464490](https://github.com/maverick-js/signals/commit/1464490d130010e939cb9182fbad9b7d4462659b))

## [4.10.0](https://github.com/maverick-js/observables/compare/v4.9.7...v4.10.0) (2022-11-30)


### Features

* new `untrack` export ([a5a3fa5](https://github.com/maverick-js/observables/commit/a5a3fa58e425da7146851a7e43746eb23306f968))


### Bug Fixes

* `onDispose` should return dispose function if no scope ([ca04b24](https://github.com/maverick-js/observables/commit/ca04b24001d890f9b69d72e14ac7a00c9ad06348))

### [4.9.7](https://github.com/maverick-js/observables/compare/v4.9.6...v4.9.7) (2022-11-26)


### Bug Fixes

* only track observed by if not same scope ([d609fef](https://github.com/maverick-js/observables/commit/d609fef7d2b771d36876639d01e416ebb5d2d9c9))
* track only current observers on each run ([1f1d818](https://github.com/maverick-js/observables/commit/1f1d818cf6e9676d4db0a4e72fa3ab1dcb597ab5))

### [4.9.6](https://github.com/maverick-js/observables/compare/v4.9.5...v4.9.6) (2022-11-25)


### Bug Fixes

* `isObserving` now requires arg ([8fd3ade](https://github.com/maverick-js/observables/commit/8fd3ade77183136fa91fef81e978d2f1e5942279))
* drop deprecated `getParent` ([6a1b64d](https://github.com/maverick-js/observables/commit/6a1b64d4a085d6a8c7bd428a0c82c7418989d755))
* drop deprecated `isObserved` ([a7d169a](https://github.com/maverick-js/observables/commit/a7d169a32b1d947b1d8f80d8d85399258a738069))

### [4.9.5](https://github.com/maverick-js/observables/compare/v4.9.4...v4.9.5) (2022-11-25)


### Bug Fixes

* `isObserved` -> `isObserving` ([7a96166](https://github.com/maverick-js/observables/commit/7a961669976cc861df8ce2ab17f40d4dfe7cfea7))
* allow fallback to be set if computed init error ([2cd85b2](https://github.com/maverick-js/observables/commit/2cd85b27bbd58df00ef5dbda43e08d4faf900101))
* remove auto-dispose perf overhead ([bbbbbe6](https://github.com/maverick-js/observables/commit/bbbbbe634a04e42fa91d3d4eb16ede33343ca58e))
* root should not add any observers ([36baad2](https://github.com/maverick-js/observables/commit/36baad202538bf0f0effebd6bd5118bcdcf076d0))

### [4.9.4](https://github.com/maverick-js/observables/compare/v4.9.3...v4.9.4) (2022-11-25)


### Bug Fixes

* clear error handlers before each computed run ([8a716cd](https://github.com/maverick-js/observables/commit/8a716cd6cff592e5624dcee8a493bfd645fdec8f))

### [4.9.3](https://github.com/maverick-js/observables/compare/v4.9.2...v4.9.3) (2022-11-25)


### Bug Fixes

* option to silence computed init error ([7b98328](https://github.com/maverick-js/observables/commit/7b98328db844d79a4cf4a70e44bbfd6a005e2136))

### [4.9.2](https://github.com/maverick-js/observables/compare/v4.9.1...v4.9.2) (2022-11-25)


### Bug Fixes

* log error if computed throws on first run ([8582879](https://github.com/maverick-js/observables/commit/8582879caa2c930d5990607074748695c6bb9bbc))
* remove redundant try/catch in queued task ([c95e02e](https://github.com/maverick-js/observables/commit/c95e02ea461c088c0898eb45968fb888aa806454))

### [4.9.1](https://github.com/maverick-js/observables/compare/v4.9.0...v4.9.1) (2022-11-25)


### Bug Fixes

* general error handling improvements ([3b7095f](https://github.com/maverick-js/observables/commit/3b7095f8cbde680f8dce00e959f40b021535c2d3))

## [4.9.0](https://github.com/maverick-js/observables/compare/v4.8.5...v4.9.0) (2022-11-25)


### Features

* new `ObservableOptions` type export ([e6aa68c](https://github.com/maverick-js/observables/commit/e6aa68c1459566ba3783ce08ff3c65cb1b42d904))


### Bug Fixes

* auto-dispose computed if no observers ([0ab5855](https://github.com/maverick-js/observables/commit/0ab5855eb27dfcbe4fd5f5290fe725f6d0d76ebf))
* only dispose needed parts ([a3db078](https://github.com/maverick-js/observables/commit/a3db078c366b7e4f4350f09cbd06b309ccd10953))
* remove child from parent set on dispose ([4fcbaec](https://github.com/maverick-js/observables/commit/4fcbaec39dd37cd5cfb8df17d56b065c9ffd01c3))
* stop observing computed after its disposed ([c2daca8](https://github.com/maverick-js/observables/commit/c2daca8ae29bdae7de08b815626eb7233283b8dd))

### [4.8.5](https://github.com/maverick-js/observables/compare/v4.8.4...v4.8.5) (2022-11-16)


### Bug Fixes

* consistent empty disposals order ([3459a1a](https://github.com/maverick-js/observables/commit/3459a1a49bb9addaed4898fa4ad63d9b0c4ad622))
* simplify effect child disposal ([0feced4](https://github.com/maverick-js/observables/commit/0feced47e9ee68df7709f17d3ada3245d9205bc1))

### [4.8.4](https://github.com/maverick-js/observables/compare/v4.8.3...v4.8.4) (2022-11-15)


### Bug Fixes

* `getParent` -> `getScope` ([adabf61](https://github.com/maverick-js/observables/commit/adabf61885853dc6489ced8df52c00b793f71b7b))
* dispose conditional nested effects ([f06756c](https://github.com/maverick-js/observables/commit/f06756c7500c8e1306a1c094011a5f3cd6a912ef))

### [4.8.3](https://github.com/maverick-js/observables/compare/v4.8.2...v4.8.3) (2022-11-08)


### Bug Fixes

* scoped function should still be observable ([0c1d2ea](https://github.com/maverick-js/observables/commit/0c1d2ea334db68cb22e91a8571b35867ab0cbeb3))

### [4.8.2](https://github.com/maverick-js/observables/compare/v4.8.1...v4.8.2) (2022-11-08)


### Bug Fixes

* add context symbol description in dev ([96ea827](https://github.com/maverick-js/observables/commit/96ea827d88a9f1d9009ae64b832d2ddb426ef891))

### [4.8.1](https://github.com/maverick-js/observables/compare/v4.8.0...v4.8.1) (2022-11-08)


### Bug Fixes

* add symbol descriptions in dev ([298410a](https://github.com/maverick-js/observables/commit/298410a1651e57c68ac63854d19e85476bbdc7d0))

## [4.8.0](https://github.com/maverick-js/observables/compare/v4.7.1...v4.8.0) (2022-11-08)


### Features

* `scope` accepts parent arg ([4eb2760](https://github.com/maverick-js/observables/commit/4eb276005c8d21c2d1d7fedc6cac2b04f26a2bf6))

### [4.7.1](https://github.com/maverick-js/observables/compare/v4.7.0...v4.7.1) (2022-11-04)


### Bug Fixes

* scoped function can return value ([c1d13c8](https://github.com/maverick-js/observables/commit/c1d13c85590fb7e52e2d1acbca25af72d89840c8))

## [4.7.0](https://github.com/maverick-js/observables/compare/v4.6.0...v4.7.0) (2022-11-04)


### Features

* new `scope` export ([806e82a](https://github.com/maverick-js/observables/commit/806e82ac932cca7fdf822333318b8954d415a693))

## [4.6.0](https://github.com/maverick-js/observables/compare/v4.5.0...v4.6.0) (2022-10-28)


### Features

* new `isObserved` export ([1bf4cd1](https://github.com/maverick-js/observables/commit/1bf4cd1057e768de9a2f7646ed5232aa7905699b))


### Bug Fixes

* dispose cells at the end of each cellx benchmark run ([9c63d4b](https://github.com/maverick-js/observables/commit/9c63d4b83b2fe82868281a120d65cf63e6fbf15a))
* fix sinuous benchmarks ([f55e188](https://github.com/maverick-js/observables/commit/f55e1881eb01f93aa8762f6118774c98be426da1))
* let cellx release its global pendingCells array between benchmarks ([0a02af1](https://github.com/maverick-js/observables/commit/0a02af19b6e966404ed0f134dde578e52fa27b14))

## [4.5.0](https://github.com/maverick-js/observables/compare/v4.4.0...v4.5.0) (2022-08-30)


### Features

* bump scheduler to `2.0.0` ([58cf305](https://github.com/maverick-js/observables/commit/58cf305a030d7b61ce38c8d1038e7c2bbb21bb95))

## [4.4.0](https://github.com/maverick-js/observables/compare/v4.3.2...v4.4.0) (2022-08-30)


### Features

* bump scheduler to `1.0.2` ([b35f3bb](https://github.com/maverick-js/observables/commit/b35f3bb134c4c5bb2def73af0580db299c152491))

### [4.3.2](https://github.com/maverick-js/observables/compare/v4.3.1...v4.3.2) (2022-08-10)


### Bug Fixes

* use set so error handlers are only added once ([68c75ab](https://github.com/maverick-js/observables/commit/68c75ab0f7a1a8661592183d4c947600c3231b37))

### [4.3.1](https://github.com/maverick-js/observables/compare/v4.3.0...v4.3.1) (2022-08-09)


### Bug Fixes

* forward error re-throw to parent handler ([5034795](https://github.com/maverick-js/observables/commit/50347954e37314f72f84661aebebcbe649c4e899))

## [4.3.0](https://github.com/maverick-js/observables/compare/v4.2.3...v4.3.0) (2022-08-09)


### Features

* `getContext` and `setContext` ([9578cd0](https://github.com/maverick-js/observables/commit/9578cd0b7a62b0838f03a0987094cb90bd254300))
* `onError` ([f36c1c0](https://github.com/maverick-js/observables/commit/f36c1c017061d4c20d61415bd1c74cc70da0018b))


### Bug Fixes

* exclude `@maverick-js/scheduler` from bundle (external) ([2f37a04](https://github.com/maverick-js/observables/commit/2f37a0448a2f62fe52f23bfc936c11fbb60ef338))

### [4.2.3](https://github.com/maverick-js/observables/compare/v4.2.2...v4.2.3) (2022-08-09)


### Bug Fixes

* `root` should keep a reference to parent ([d8162ae](https://github.com/maverick-js/observables/commit/d8162ae8f5a20a14d00f0fb826219f2e5f911cd5))

### [4.2.2](https://github.com/maverick-js/observables/compare/v4.2.1...v4.2.2) (2022-08-09)


### Bug Fixes

* prevent infinite `getParent` recursion (attempt 2) ([b600c7a](https://github.com/maverick-js/observables/commit/b600c7ac6bb0d68c9ad9a08c1f161c0a8dfdf270))

### [4.2.1](https://github.com/maverick-js/observables/compare/v4.2.0...v4.2.1) (2022-08-09)


### Bug Fixes

* prevent infinite recursion when nesting `getParent` calls ([68d850d](https://github.com/maverick-js/observables/commit/68d850dfbaeeb922bce86739f35c17bbdc3ddd83))

## [4.2.0](https://github.com/maverick-js/observables/compare/v4.1.2...v4.2.0) (2022-08-09)


### Features

* argumentless `getParent()` returns current parent ([c717439](https://github.com/maverick-js/observables/commit/c717439932a64e1c8ec6363c16b6a6aca2ce6021))

### [4.1.2](https://github.com/maverick-js/observables/compare/v4.1.1...v4.1.2) (2022-08-08)


### Bug Fixes

* remove redundant `unrefSet` calls ([778b8ee](https://github.com/maverick-js/observables/commit/778b8ee360d9c4ce3174f5d8d779b54bd96e1478))

### [4.1.1](https://github.com/maverick-js/observables/compare/v4.1.0...v4.1.1) (2022-08-08)


### Bug Fixes

* update computed map docs ([0bbf814](https://github.com/maverick-js/observables/commit/0bbf8149ce52ae3ffe4f790675dc00b4d72e0b2c))

## [4.1.0](https://github.com/maverick-js/observables/compare/v4.0.2...v4.1.0) (2022-08-08)


### Features

* `computedMap` and `computedKeyedMap` ([4e9c91b](https://github.com/maverick-js/observables/commit/4e9c91b63e1ae9ab85c650553849c8b5a3d10ad1))

### [4.0.2](https://github.com/maverick-js/observables/compare/v4.0.1...v4.0.2) (2022-08-05)


### Bug Fixes

* do not empty disposal on non-dirty child computations ([86b2d75](https://github.com/maverick-js/observables/commit/86b2d75075b7c494636bf1127d3776bdc2989682))

### [4.0.1](https://github.com/maverick-js/observables/compare/v4.0.0...v4.0.1) (2022-08-05)


### Bug Fixes

* keep child computations alive on update ([f4b1d2d](https://github.com/maverick-js/observables/commit/f4b1d2d6651da0692fdb77c8ac30c6a803710b9e)), closes [#4](https://github.com/maverick-js/observables/issues/4)

## [4.0.0](https://github.com/maverick-js/observables/compare/v3.4.1...v4.0.0) (2022-08-04)

### ⚠ BREAKING CHANGES

- Library authors can decide how to re-export bindings
  from this package. The `$` prefix was used a little inconsistently so
  it's best to drop it completely.

### Bug Fixes

- drop `$` prefix on exports ([a18149b](https://github.com/maverick-js/observables/commit/a18149b929d7471f5d00597674aa1f0e5728c11a)), see [#4](https://github.com/maverick-js/observables/issues/4#issuecomment-1171106602)

### [3.4.1](https://github.com/maverick-js/observables/compare/v3.4.0...v3.4.1) (2022-07-12)

### Bug Fixes

- move scheduler to separate package ([83120d7](https://github.com/maverick-js/observables/commit/83120d7662daaf5e7ac2fe0ac0cceda26f80f1c5))

## [3.4.0](https://github.com/maverick-js/observables/compare/v3.3.0...v3.4.0) (2022-07-08)

### Features

- new `dirty` option for `computed` ([7ae2e6c](https://github.com/maverick-js/observables/commit/7ae2e6cb353d571e66a56c8c90ddc2e35fe126d9))

## [3.3.0](https://github.com/maverick-js/observables/compare/v3.2.0...v3.3.0) (2022-07-08)

### Features

- new export `getParent` ([88310aa](https://github.com/maverick-js/observables/commit/88310aadf829b984011b9fc108997701d767c8e2))

### Bug Fixes

- track parent across peeks ([af4d561](https://github.com/maverick-js/observables/commit/af4d5615d78560f75ecea780a15ee46c33049719))

## [3.2.0](https://github.com/maverick-js/observables/compare/v3.1.5...v3.2.0) (2022-07-06)

### Features

- new `onFlush` method on scheduler ([0eccb59](https://github.com/maverick-js/observables/commit/0eccb59d1781795df358d99b8d1ffb99010fd1b4))
- new export `getScheduler` ([f92183b](https://github.com/maverick-js/observables/commit/f92183bcfa8c0959c0eb68b0f3efb24087a87e08))

### [3.1.5](https://github.com/maverick-js/observables/compare/v3.1.4...v3.1.5) (2022-07-03)

### Bug Fixes

- revert a39679d1ddb9b825a9e3fa8f33dc56f0bab18c43 ([88c5dbe](https://github.com/maverick-js/observables/commit/88c5dbe26c312c86c1663a71562ea1bfe1a0fad5))

### [3.1.4](https://github.com/maverick-js/observables/compare/v3.1.3...v3.1.4) (2022-07-03)

### Bug Fixes

- dont dispose of children on update ([a39679d](https://github.com/maverick-js/observables/commit/a39679d1ddb9b825a9e3fa8f33dc56f0bab18c43))

### [3.1.3](https://github.com/maverick-js/observables/compare/v3.1.2...v3.1.3) (2022-07-02)

### Bug Fixes

- additional parent tracking variable not required ([9df21ee](https://github.com/maverick-js/observables/commit/9df21ee0d104d1da85aa28ebebd7925c1995e56a))

### [3.1.2](https://github.com/maverick-js/observables/compare/v3.1.1...v3.1.2) (2022-07-02)

### Bug Fixes

- incorrect recursive parent tracking ([7390155](https://github.com/maverick-js/observables/commit/7390155f7a5e8be85c7d2fc8d06c4c261dc43437))

### [3.1.1](https://github.com/maverick-js/observables/compare/v3.1.0...v3.1.1) (2022-07-02)

### Bug Fixes

- parent should be determined on creation ([117fa5b](https://github.com/maverick-js/observables/commit/117fa5bc77dc84970f262801887238d3e5ead4c7))

## [3.1.0](https://github.com/maverick-js/observables/compare/v3.0.0...v3.1.0) (2022-07-01)

### Features

- `observable` accepts dirty check option ([0c7a55d](https://github.com/maverick-js/observables/commit/0c7a55d9b71463200e90413a1d6987b00451e9ae))

### Bug Fixes

- effect should run all disposals on each new run ([3217217](https://github.com/maverick-js/observables/commit/3217217a85c232e6e0311d31ea3fd9d9b25db825))
- second argument to observables is an options object (prev debug id) ([d0c31e7](https://github.com/maverick-js/observables/commit/d0c31e745867283e190a6c1626c8156b624aeeda))

## [3.0.0](https://github.com/maverick-js/observables/compare/v2.0.3...v3.0.0) (2022-06-30)

### ⚠ BREAKING CHANGES

- computed type `Computed` -> `Observable`
- observable return type is now `ObservableSubject`
- dropped `isComputed`
- `isObservable` checks readonly
- `isObservable` passes for computed observables

### Bug Fixes

- all types extend observable ([bef215c](https://github.com/maverick-js/observables/commit/bef215c1ec98cb3593e1f9daea71bb6b6974ee2f))

### [2.0.3](https://github.com/maverick-js/observables/compare/v2.0.2...v2.0.3) (2022-06-28)

### Bug Fixes

- track parent separately to handle disposals correctly ([50110d4](https://github.com/maverick-js/observables/commit/50110d4d8fa590310a24d3e9b4433463c455c189))

### [2.0.2](https://github.com/maverick-js/observables/compare/v2.0.1...v2.0.2) (2022-06-27)

### Bug Fixes

- dont need safe inequality check ([368af0c](https://github.com/maverick-js/observables/commit/368af0ccc594654defe619763935376abbdfb56c))

### [2.0.1](https://github.com/maverick-js/observables/compare/v2.0.0...v2.0.1) (2022-06-27)

### Bug Fixes

- avoid stack overflow in prod ([4cba856](https://github.com/maverick-js/observables/commit/4cba85621a693a8b3afb6f2a0fe663ec06384d31))

## 2.0.0 (2022-06-27)

### Features

- `root` ([a70746f](https://github.com/maverick-js/observables/commit/a70746ffbdf286452b8f0379f942faa5c9a37c38))
- `isObservable` ([88024da](https://github.com/maverick-js/observables/commit/88024dac825b548af6e40b78e618ec19d1e154d2))
- `onDispose` hook ([db8c142](https://github.com/maverick-js/observables/commit/db8c142625624f404fb021cc631a6cc8f5d44926))
- cleanup function can be returned inside `effect` ([7a4f72f](https://github.com/maverick-js/observables/commit/7a4f72fac438010cae08d40244cd4e277995f8e6))
- improve type inference in `is` functions ([7cd7b92](https://github.com/maverick-js/observables/commit/7cd7b92eddce3cdaacb70100e6be021a89253e34))
- initial commit ([51cd6d5](https://github.com/maverick-js/observables/commit/51cd6d5cad05e3f1bb0f9446d29186b3b65e42b5))

### Bug Fixes

- `queueMicrotask` fallback will error ([0e0bea4](https://github.com/maverick-js/observables/commit/0e0bea4cfb13011cfdf121eb4c3279cb95459587)), closes [#2](https://github.com/maverick-js/observables/issues/2)
- rename `update()` to `next()` ([323f20e](https://github.com/maverick-js/observables/commit/323f20e8d491461dce873e999c6a4447274b9b7a))

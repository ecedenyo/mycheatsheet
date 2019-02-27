Feature | Sass | LESS
--- | --- | ---
Variables | $var_name: value; | @var_name: value;
Import file | @import "folder/file"; | _... the same..._
"Extending" | .new-class { @extend .class-to-be-extended; } | .new-class { .class-to-be-extended(); }
Mixins def. | @mixin mixin-name($optional-params) { ... } | .mixin-name(@optional-params) { ... }
Mixin call | @include mixin-name($optional-params); | .mixin-name(@optional-params);
Control functions | @if condition { ... } | when (condition) { ... }
Nesting _(parent referencing)_ | .parent-class { ... &:hover { ... } | _... the same..._

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ1MjY1NDkxNCwxMjA3NDE3MzA0LDEyND
g4MDkzNTAsNDU1MjA0NzIzLC0xMTEzODk3Njk2XX0=
-->
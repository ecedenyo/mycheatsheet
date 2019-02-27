Description | SASS | LESS
--- | --- | ---
Import file | @import "folder/file"; | _... the same..._
Variables | $var_name: value; | @var_name: value;
Mixins def. | @mixin mixin-name($optional-params) { ... } | .mixin-name(@optional-params) { ... }
Mixin call | @include mixin-name | .mixin-name();
Control functions | @if condition { ... } | when (condition) { ... }
Nesting _(parent referencing)_ | .parent-class { ... &:hover { ... } | _... the same..._

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY5NTQ5NjQ4OSwtMTExMzg5NzY5Nl19
-->
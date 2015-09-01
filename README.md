# angular-perfect-scrollbar-2
Another wrapper around [perfect-scrollbar](https://github.com/noraesae/perfect-scrollbar).

### Usage
0. `npm install angular-perfect-scrollbar-2`
1. In app code:
```
angular.module('app', [ require('angular-perfect-scrollbar-2') ])
```
2. Use `<perfect-scrollbar>` directive in your templates:
```
<style type="text/css">
	.scroll-wrapper {
		position: relative;
		overflow: hidden;
		height: 300px;
	}
</style>

<perfect-scrollbar class="scroll-wrapper" opts="..." update="update">
	... SCROLLABLE CONTENT HERE ...
</perfect-scrollbar>
```

The `opts` attribute allows to configure the perfect-scrollbar instance
(see [perfect-scrollbar](https://github.com/noraesae/perfect-scrollbar)).

The `update` attribute may point to a variable from $scope. Setting this variable to
`true` forces scrollbar update. The variable is set to `false` automatically afterwards.

### License
MIT

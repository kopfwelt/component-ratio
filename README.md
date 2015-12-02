# Ratio component

If you want an element to scale its height in relation to the width, like a normal image would, you can use the styles of this component. Also known as "flexible responsive media CSS intrinsic ratio scaling technique".

## How to use

1) Install the component using NPM

```
npm install --save kopfwelt/component-ratio
```

2) Import the SCSS mixins and apply them

```scss
@import 'node_modules/kopfwelt/component-ratio/component-ratio-mixin';

.Ratio {
	@include aspect-ratio(16,9);
}
.Ratio-inner {
	@include aspect-ratio-inner;
}
```

Note: the `.Ratio` and `.Ratio-inner` classes are examples. You can apply the mixins to any thing.

3) Use it

```markup
<div class="Ratio">
	<img class="Ratio-inner" alt="" />
</div>

<div class="Ratio">
	<iframe width="560" height="315" src="https://www.youtube.com/embed/yJkmHQ2q--I" frameborder="0" allowfullscreen></iframe>
</div>
```

and presto!

You can put anything inside, not just video. The important part is using two elements: parent and child.

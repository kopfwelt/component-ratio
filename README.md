# Ratio component

Use this when you want an element to scale along a certain aspect ratio.

Example, you have a `<video>` element in a weird format. You want it to always scale in 16/9.

Do this:

```markup
<div class="Ratio">
	<video class="Ratio-inner"></video>
</div>
```

and presto!

You can also use the mixin directly `@include aspect-ratio(4,3)` in your Sass styles.

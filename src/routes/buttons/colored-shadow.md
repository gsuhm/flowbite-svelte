---
layout: buttonLayout
---

<script>
  import { ColorShadowButton }from '$lib/index';
</script>

<h1 class="text-3xl w-full text-gray-900 dark:text-white py-8">Colored Shadow</h1>

<h2 class="text-2xl w-full text-gray-900 dark:text-white py-8">Button Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
type Textsize = 'text-xs' | 'text-sm' | 'text-base' | 'text-lg' | 'text-xl' | 'text-2xl' | 'text-3xl' | 'text-4xl'
type Buttonshadows = 'blue' | 'green' | 'cyan' | 'teal' | 'lime' | 'red' | 'pink' | 'purple';
type ButtonType = 'button' | 'submit' | 'reset'
let textSize: Textsize = 'text-sm';
let color: Buttonshadows = 'blue';
let name = 'Read more';
let type: ButtonType = 'button';
```

<h2 class="text-2xl w-full dark:text-white py-8">text-sm</h2>


<div class=" flex flex-wrap justify-center rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ColorShadowButton color="blue" name="Blue" />
<ColorShadowButton color="green" name="Green" />
<ColorShadowButton color="cyan" name="Cyan" />
<ColorShadowButton color="teal" name="Teal" />
<ColorShadowButton color="lime" name="Lime" />
<ColorShadowButton color="red" name="Red" />
<ColorShadowButton color="pink" name="Pink" />
<ColorShadowButton color="purple" name="Purple" />
</div>

```html
<ColorShadowButton color="blue" name="Blue" />
<ColorShadowButton color="green" name="Green" />
<ColorShadowButton color="cyan" name="Cyan" />
<ColorShadowButton color="teal" name="Teal" />
<ColorShadowButton color="lime" name="Lime" />
<ColorShadowButton color="red" name="Red" />
<ColorShadowButton color="pink" name="Pink" />
<ColorShadowButton color="purple" name="Purple" />
```

<h2 class="text-2xl w-full dark:text-white py-8">text-xs</h2>


<div class=" flex flex-wrap justify-center rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ColorShadowButton color="blue" name="Blue" textSize="text-xs"/>
<ColorShadowButton color="green" name="Green" textSize="text-xs" />
<ColorShadowButton color="cyan" name="Cyan" textSize="text-xs" />
<ColorShadowButton color="teal" name="Teal" textSize="text-xs" />
<ColorShadowButton color="lime" name="Lime" textSize="text-xs" />
<ColorShadowButton color="red" name="Red" textSize="text-xs" />
<ColorShadowButton color="pink" name="Pink" textSize="text-xs" />
<ColorShadowButton color="purple" name="Purple" textSize="text-xs" />
</div>

```html
<ColorShadowButton color="blue" name="Blue" textSize="text-xs"/>
<ColorShadowButton color="green" name="Green" textSize="text-xs" />
<ColorShadowButton color="cyan" name="Cyan" textSize="text-xs" />
<ColorShadowButton color="teal" name="Teal" textSize="text-xs" />
<ColorShadowButton color="lime" name="Lime" textSize="text-xs" />
<ColorShadowButton color="red" name="Red" textSize="text-xs" />
<ColorShadowButton color="pink" name="Pink" textSize="text-xs" />
<ColorShadowButton color="purple" name="Purple" textSize="text-xs" />
```

<h2 class="text-2xl w-full dark:text-white py-8">text-base</h2>

<div class=" flex flex-wrap justify-center rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ColorShadowButton color="blue" name="Blue" textSize="text-base"/>
<ColorShadowButton color="green" name="Green" textSize="text-base" />
<ColorShadowButton color="cyan" name="Cyan" textSize="text-base" />
<ColorShadowButton color="teal" name="Teal" textSize="text-base" />
<ColorShadowButton color="lime" name="Lime" textSize="text-base" />
<ColorShadowButton color="red" name="Red" textSize="text-base" />
<ColorShadowButton color="pink" name="Pink" textSize="text-base" />
<ColorShadowButton color="purple" name="Purple" textSize="text-base" />
</div>

```html
<ColorShadowButton color="blue" name="Blue" textSize="text-base"/>
<ColorShadowButton color="green" name="Green" textSize="text-base" />
<ColorShadowButton color="cyan" name="Cyan" textSize="text-base" />
<ColorShadowButton color="teal" name="Teal" textSize="text-base" />
<ColorShadowButton color="lime" name="Lime" textSize="text-base" />
<ColorShadowButton color="red" name="Red" textSize="text-base" />
<ColorShadowButton color="pink" name="Pink" textSize="text-base" />
<ColorShadowButton color="purple" name="Purple" textSize="text-base" />
```

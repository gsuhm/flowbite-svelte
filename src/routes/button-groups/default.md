---
layout: buttongroupLayout
---

<script>
  import {ButtonGroup, ButtonGroupOutline} from '$lib/index'
  import {UserCircleIconSolid, AdjustmentsIconSolid, CloudDownloadIconSolid} from "@codewithshin/svelte-heroicons"
  let buttons1 = [
  {
    name: "Profile",
  },
  {
    name: "Settings",
  },
  {
    name: "Messages",
  },
];
  let buttons2 = [
  {
    name: "Profile",
    href:"/",
    icon: UserCircleIconSolid
  },
  {
    name: "Settings",
    href:"/",
    icon: AdjustmentsIconSolid
  },
  {
    name: "Messages",
    href:"/",
    icon: CloudDownloadIconSolid
  },
];
</script>


<h1 class="text-3xl w-full text-gray-900 dark:text-white py-8">Button Group</h1>

<h2 class="text-2xl w-full text-gray-900 dark:text-white py-8">Setup</h2>

```html
<script>
  import {ButtonGroup, ButtonGroupOutline} from 'flowbite-svelte'
  import {UserCircleIconSolid, AdjustmentsIconSolid, CloudDownloadIconSolid} from "@codewithshin/svelte-heroicons"
  let buttons1 = [
  {
    name: "Profile",
  },
  {
    name: "Settings",
  },
  {
    name: "Messages",
  },
];
  let buttons2 = [
  {
    name: "Profile",
    href:"/",
    icon: UserCircleIconSolid
  },
  {
    name: "Settings",
    href:"/",
    icon: AdjustmentsIconSolid
  },
  {
    name: "Messages",
    href:"/",
    icon: CloudDownloadIconSolid
  },
];
</script>
```

<h2 class="text-2xl w-full text-gray-900 dark:text-white py-8">Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
interface ButtonGroupType {
  name: string;
  href?: string;
  rel?: string;
  icon?: typeof SvelteComponent;
}
let buttons: ButtonGroupType[];
```

<h2 class="text-2xl w-full text-gray-900 dark:text-white py-8">Default</h2>

<div
  class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ButtonGroup buttons={buttons1}/>
</div>


```html
<ButtonGroup buttons={buttons1}/>
```

<h2 class="text-2xl w-full text-gray-900 dark:text-white py-8">Default with icon</h2>

<div
  class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ButtonGroup buttons={buttons2}/>
</div>


```html
<ButtonGroup buttons={buttons2}/>
```

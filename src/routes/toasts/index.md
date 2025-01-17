---
layout: toastLayout
---

<script>
import {Toast} from '$lib/index'
import { quintOut, elasticOut } from 'svelte/easing';
import {FireIconOutline, CheckCircleIconSolid, PlusCircleIconOutline,ArchiveIconSolid} from '@codewithshin/svelte-heroicons'
</script>

<h1 class="text-3xl w-full dark:text-white py-8">Toast</h1>

<p class="dark:text-white py-4 text-lg">Import the Toast component and Icons.</p>

```html
<script>
import {Toast} from 'flowbite-svelte'
import {FireIconOutline, CheckCircleIconSolid, PlusCircleIconOutline,ArchiveIconSolid} from '@codewithshin/svelte-heroicons'
</script>
```

<h2 class="text-2xl w-full dark:text-white py-8">Examples</h2>

<p class="dark:text-white py-4 text-lg">Use fade, fly, slide, or blur for transitionType.</p>

<h3 class="text-xl w-full dark:text-white py-8">Fade examples</h3>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Toast>
    <span slot="icon">
    <FireIconOutline />
    </span>
    <span slot="text">
      Transition type: fade
    </span>
  </Toast>
</div>

```html
<Toast>
  <span slot="icon">
  <FireIconOutline />
  </span>
  <span slot="text">
    Transition type: fade
  </span>
</Toast>
```

<h3 class="text-xl w-full dark:text-white py-8">Slide examples</h3>

<p class="dark:text-white py-4 text-lg">You can use one of <a href="https://svelte.dev/docs#run-time-svelte-easing" target="_blank"  class="text-blue-600 hover:underline dark:text-blue-500"></a>Svelte/easing.</p>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
   <Toast transitionType="slide" iconColor='red'>
    <span slot="icon">
    <CheckCircleIconSolid className="h-5 w-5 text-red-500"/>
    </span>
    <span slot="text">
      Transition type: slide
    </span>
  </Toast>
</div>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
   <Toast transitionType="slide" iconColor='red' transitionParams={{delay: 250, duration: 300, easing: quintOut}}>
    <span slot="icon">
    <CheckCircleIconSolid className="h-5 w-5 text-red-500"/>
    </span>
    <span slot="text">
      Transition type: slide, delay: 250, duration: 300, easing: quintOut
    </span>
  </Toast>
</div>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
   <Toast transitionType="slide" iconColor='red' transitionParams={{delay: 250, duration: 2000, easing: elasticOut}}>
    <span slot="icon">
    <CheckCircleIconSolid className="h-5 w-5 text-red-500"/>
    </span>
    <span slot="text">
      Transition type: slide, delay: 250, duration: 2000, easing: elasticOut
    </span>
  </Toast>
</div>

```html
<Toast transitionType="slide" iconColor='red'>
  <span slot="icon">
  <CheckCircleIconSolid className="h-5 w-5 text-red-500"/>
  </span>
  <span slot="text">
    Transition type: slide
  </span>
</Toast>

 <Toast transitionType="slide" iconColor='red' transitionParams={{delay: 250, duration: 300, easing: quintOut}}>
  <span slot="icon">
  <CheckCircleIconSolid className="h-5 w-5 text-red-500"/>
  </span>
  <span slot="text">
    Transition type: slide, delay: 250, duration: 300, easing: quintOut
  </span>
</Toast>

<Toast transitionType="slide" iconColor='red' transitionParams={{delay: 250, duration: 2000, easing: elasticOut}}>
  <span slot="icon">
  <CheckCircleIconSolid className="h-5 w-5 text-red-500"/>
  </span>
  <span slot="text">
    Transition type: slide, delay: 250, duration: 2000, easing: elasticOut
  </span>
</Toast>
```

<h3 class="text-xl w-full dark:text-white py-8">Blur examples</h3>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Toast transitionType="blur" iconColor='purple' transitionParams={{amount: 10}}>
    <span slot="icon">
    <PlusCircleIconOutline className="h-5 w-5 text-purple-500"/>
    </span>
    <span slot="text">
      Transition type: blur, amount: 10
    </span>
  </Toast>
</div>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Toast transitionType="blur" iconColor='purple' transitionParams={{amount: 50, delay: 1000}}>
    <span slot="icon">
    <PlusCircleIconOutline className="h-5 w-5 text-purple-500"/>
    </span>
    <span slot="text">
      Transition type: blur, amount: 50, delay 1000
    </span>
  </Toast>
</div>

```html
<Toast transitionType="blur" iconColor='purple' transitionParams={{amount: 10}}>
  <span slot="icon">
  <PlusCircleIconOutline className="h-5 w-5 text-purple-500"/>
  </span>
  <span slot="text">
    Transition type: blur, amount: 10
  </span>
</Toast>

<Toast transitionType="blur" iconColor='purple' transitionParams={{amount: 50, delay: 1000}}>
  <span slot="icon">
  <PlusCircleIconOutline className="h-5 w-5 text-purple-500"/>
  </span>
  <span slot="text">
    Transition type: blur, amount: 50, delay 1000
  </span>
</Toast>
```

<h3 class="text-xl w-full dark:text-white py-8">Fly examples</h3>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Toast transitionType="fly" transitionParams={{x: 200}} iconColor="green">
    <span slot="icon">
    <ArchiveIconSolid  className="h-5 w-5 text-green-500"/>
    </span>
    <span slot="text">
      Transition type: fly right
    </span>
  </Toast>
</div>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Toast transitionType="fly" transitionParams={{y: 200}} iconColor="green">
    <span slot="icon">
    <ArchiveIconSolid  className="h-5 w-5 text-green-500"/>
    </span>
    <span slot="text">
      Transition type: fly down
    </span>
  </Toast>
</div>

```html
<Toast transitionType="fly" transitionParams={{x: 200}} iconColor="green">
  <span slot="icon">
  <ArchiveIconSolid  className="h-5 w-5 text-green-500"/>
  </span>
  <span slot="text">
    Transition type: fly right
  </span>
</Toast>

<Toast transitionType="fly" transitionParams={{y: 200}} iconColor="green">
  <span slot="icon">
  <ArchiveIconSolid  className="h-5 w-5 text-green-500"/>
  </span>
  <span slot="text">
    Transition type: fly down
  </span>
</Toast>
```

<h2 class="text-2xl w-full dark:text-white py-8">Icons</h2>

<p class="dark:text-white py-4 text-lg">Use any <a href="https://flowbite-svelte.vercel.app/icons" class="text-blue-600 hover:underline dark:text-blue-500">icon components.</a></p>

```html
<script>
import {Toast} from 'flowbite-svelte'
import {FireIconOutline, CheckCircleIconSolid, PlusCircleIconOutline,ArchiveIconSolid} from '@codewithshin/svelte-heroicons'
</scrip>
```

<h2 class="text-2xl w-full dark:text-white py-8">Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
type Colors = 'blue' | 'gray' | 'red' | 'yellow' | 'purple' | 'green' | 'indigo' | 'pink';
type TransitionTypes = 'fade' | 'fly' | 'slide' | 'blur'
export let iconColor: Colors = 'blue'; 
export let transitionType: TransitionTypes = 'fade'; 
export let divClass =
  'flex items-center w-full max-w-xs p-4 text-gray-500 bg-white rounded-lg shadow dark:text-gray-400 dark:bg-gray-800';
export let btnClass =
  'ml-auto -mx-1.5 -my-1.5 bg-white text-gray-400 hover:text-gray-900 rounded-lg focus:ring-2 focus:ring-gray-300 p-1.5 hover:bg-gray-100 inline-flex h-8 w-8 dark:text-gray-500 dark:hover:text-white dark:bg-gray-800 dark:hover:bg-gray-700';
export let text: string = '';
```
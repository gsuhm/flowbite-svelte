---
layout: navbarLayout
---

<script>
  import { Navbar }from '$lib/index';
  let sitename = "Flowbite Svelte";
  let menus = [
    {
      name: "Home",
      href: "/"
    },
    {
      name: "GitHub",
      href: "https://github.com/shinokada/flowbite-svelte"
    },
    {
      name: "Design",
      href: "https://flowbite-svelte.vercel.app"
    },
  ];
 
</script>

<h1 class="text-3xl w-full dark:text-white py-8">Navbar Default</h1>


```html
<script>
  import { Navbar } from "flowbite-svelte";
  let sitename = "Flowbite Svelte";
  let logo = "/images/mkdir-logo.webp";
  let alt = "flowbite-svelte";
  let textsize = "text-lg";
  let menus = [
    {
      name: "Home",
      href: "/",
    },
    {
      name: "GitHub",
      href: "https://github.com/shinokada/flowbite-svelte"
    },
    {
      name: "Design",
      href: "https://flowbite-svelte.vercel.app",
    },
  ];
</script>

<Navbar {menus} {sitename} {alt} {logo} {textsize} />
```

<h2 class="text-2xl w-full dark:text-white py-8">Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
interface LinkType {
  name: string;
  href: string;
  rel?: string;
}
let sitename = 'Svelte Flow';
let logo = '/images/mkdir-logo.png';
let alt = 'Svelte Flow';
let textsize = 'text-sm';
let menus: LinkType[];
let navClass = 'px-2 bg-white border-gray-200 dark:bg-gray-800 dark:border-gray-700';
let spanClass = 'self-center text-lg font-semibold text-gray-900 whitespace-nowrap dark:text-white';
let buttonClass = 'inline-flex justify-center items-center ml-3 text-gray-400 rounded-lg md:hidden hover:text-gray-900 focus:outline-none focus:ring-2 focus:ring-blue-300 dark:text-gray-400 dark:hover:text-white dark:focus:ring-gray-500';
let liLinkClass = `block py-2 pr-4 pl-3  text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-gray-400 dark:hover:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent ${textsize}`;
```

<h2 class="text-lg dark:text-white py-8">Text Size text-xs</h2>

```html
<Navbar textsize="text-xs" {sitename} {menus}/>
```

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Navbar textsize="text-xs" {sitename} {menus}/>
</div>

<h2 class="text-lg dark:text-white py-8">Text Size text-sm</h2>

```html
<Navbar textsize="text-sm" {sitename} {menus} />
```

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Navbar textsize="text-sm" {sitename} {menus}/>
</div>

<h2 class="text-lg dark:text-white py-8">Text Size text-base</h2>

```html
<Navbar textsize="text-base" {sitename} {menus} />
```

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Navbar textsize="text-base" {sitename} {menus}/>
</div>

<h2 class="text-lg dark:text-white py-8">Text Size text-lg</h2>

```html
<Navbar textsize="text-lg" {sitename} {menus}/>
```

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Navbar textsize="text-lg" {sitename} {menus}/>
</div>

<h2 class="text-lg dark:text-white py-8">Text Size text-xl</h2>

```html
<Navbar textsize="text-xl" {menus}/>
```

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Navbar textsize="text-xl" {sitename} {menus} />
</div>

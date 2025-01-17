---
layout: footerLayout
---

<script>
  import {LogoFooter} from '$lib/index'
  let site = {
    href: "/",
    name: "Flowbite Svelte",
    img: "/images/mkdir-logo.png",
  };
  let links = [
    { name: "About", href: "/" },
    { name: "Profile", href: "/" },
    { name: "Contact", href: "/" },
  ];
</script>

<h1 class="text-3xl w-full dark:text-white py-8">Footer with logo</h1>


<h2 class="text-2xl w-full dark:text-white py-8">Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
interface SiteType {
  name: string;
  href: string;
  img?: string;
}
interface LinkType {
  name: string;
  href: string;
  rel?: string;
}
let site: SiteType;
let links: LinkType[];
let footerClass = 'p-4 bg-white rounded-lg shadow md:px-6 md:py-8 dark:bg-gray-800';
let divClass = 'sm:flex sm:items-center sm:justify-between';
let siteNameClass = 'self-center text-2xl font-semibold whitespace-nowrap dark:text-white';
let ulClass =
		'flex flex-wrap items-center mb-6 text-sm text-gray-500 sm:mb-0 dark:text-gray-400';
let aClass = 'mr-4 hover:underline md:mr-6';
let siteNameLinkClass = 'flex items-center mb-4 sm:mb-0';
let imgClass = 'mr-3 h-8';
let hrClass = 'my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8';
let copyRightSpanClass = 'block text-sm text-gray-500 sm:text-center dark:text-gray-400';
let copyRightLinkClass = 'hover:underline';
let copyrightYear = '© 2022';
let allRightsReserved = 'All Rights Reserved.';
```

<h2 class="text-2xl w-full dark:text-white py-8">Examples</h2>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<LogoFooter {site} {links}/>
</div>

```html
<script>
  import {LogoFooter} from 'flowbite-svelte'
  let site = {
    href: "/",
    name: "Flowbite Svelte",
    img: "/images/mkdir-logo.png",
  };
  let links = [
    { name: "About", href: "/" },
    { name: "Profile", href: "/" },
    { name: "Contact", href: "/" },
  ];
</script>

<LogoFooter {site} {links}/>
```

---
layout: navbarLayout
---

<script>
  import { DropdownNavbar }from '$lib/index';

  let menus = [
    {
      id: 1,
      name: "Home",
      href: "/"
    },
    {
      id: 2,
      name: "Cards",
      href: "/cards",
      child: [
        {
          id: 3,
          name: "Card",
          href: "/cards/card",
        },
        {
          id: 4,
          name: "CTA Card",
          href: "/cards/cta",
        },
        {
          id: 5,
          name: "Ecommerce Card",
          href: "/cards/ecommerce",
        },
      ],
    },
    {
      id: 6,
      name: "Modals",
      href: "/",
      child: [
        {
          id: 7,
          name: "Small",
          href: "/modals/small",
        },
        {
          id: 8,
          name: "Medium",
          href: "/modals/medium",
        },
      ],
    },
  ];
</script>



<h1 class="text-3xl w-full dark:text-white py-8">Dropdown Navbar</h1>

<h2 class="text-2xl w-full dark:text-white py-8">Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
interface NavbarType {
  id: number;
  name: string;
  href: string;
  rel?: string;
  child?: NavbarType[];
}
let sitename = 'Svelte Flow';
let logo = '/images/mkdir-logo.png';
let alt: string;
let textsize = 'text-sm';
let menus: NavbarType[];
let navClass = 'px-2 bg-white border-gray-200 dark:bg-gray-800 dark:border-gray-700';
let spanClass =
		'self-center text-lg font-semibold text-gray-900 whitespace-nowrap dark:text-white';
let buttonClass =
		'inline-flex justify-center items-center ml-3 text-gray-400 rounded-lg md:hidden hover:text-gray-900 focus:outline-none focus:ring-2 focus:ring-blue-300 dark:text-gray-400 dark:hover:text-white dark:focus:ring-gray-500';
let dropdownDiv =
		'z-10 w-44 text-base list-none bg-white rounded divide-y divide-gray-100 shadow dark:bg-gray-700 dark:divide-gray-600';
let dropdownLinkClassWithChild = `block py-2 px-4 ${textsize} text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-400 dark:hover:text-white`;
let dropdownLinkClassWithoutChild = `block py-2 pr-4 pl-3  text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-gray-400 dark:hover:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent ${textsize}`;
let liButtonClass = `flex justify-between items-center py-2 pr-4 pl-3 w-full ${textsize} font-medium text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto dark:text-gray-400 dark:hover:text-white dark:focus:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent`;
```

<h2 class="text-2xl w-full dark:text-white py-8">Examples</h2>

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <DropdownNavbar textsize="text-lg" {menus} />
</div>

<p class="dark:text-white text-lg py-8">
  You can change textsize prop to text-xs, text-sm, text-base, text-lg or text-xl.
</p>

<h1 class="text-3xl w-full dark:text-white py-8">Dropdown Navbar Setup</h1>

```html
<script>
  import { DropdownNavbar } from "flowbite-svelte";
  let sitename = "Flowbite Svelte";
  let logo = "/images/mkdir-logo.webp";
  let alt = "flowbite-svelte";
  let textsize = "text-lg";
  let menus = [
    {
      id: 1,
      name: "Home",
      href: "/",
      rel: "",
    },
    {
      id: 2,
      name: "Cards",
      href: "/cards",
      rel: "",
      child: [
        {
          id: 3,
          name: "Card",
          href: "/cards/card",
          rel: "",
        },
        {
          id: 4,
          name: "CTA Card",
          href: "/cards/cta",
          rel: "",
        },
        {
          id: 5,
          name: "Ecommerce Card",
          href: "/cards/ecommerce",
          rel: "",
        },
      ],
    },
    {
      id: 6,
      name: "Modals",
      href: "/",
      rel: "",
      child: [
        {
          id: 7,
          name: "Small",
          href: "/modals/small",
          rel: "",
        },
        {
          id: 8,
          name: "Medium",
          href: "/modals/medium",
          rel: "",
        },
      ],
    },
  ];
</script>

<DropdownNavbar {menus} {sitename} {alt} {logo} {textsize} />
```

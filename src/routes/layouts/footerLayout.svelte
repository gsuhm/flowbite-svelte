<script>
	import Prism from 'prismjs';
	import 'prismjs/themes/prism.css';
	import 'prism-themes/themes/prism-holi-theme.css';
	import 'prismjs/components/prism-markdown.js';
	import { Utterances } from '@codewithshin/svelte-utterances';
</script>

<div class="max-w-3xl mx-auto pb-8">
	<div class="container flex flex-wrap mx-auto pt-8">
		<slot />

		<h2 class="text-2xl w-full dark:text-white py-8">Related components</h2>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/footer/default"
				class="text-blue-600 hover:underline dark:text-blue-500">Default Footer</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/footer/logo"
				class="text-blue-600 hover:underline dark:text-blue-500">Footer with Logo</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/footer/sitemap"
				class="text-blue-600 hover:underline dark:text-blue-500">Footer with Sitemap</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/footer/socialmedia"
				class="text-blue-600 hover:underline dark:text-blue-500">Footer with Socialmedia</a
			>
		</p>

		<h2 class="text-2xl w-full dark:text-white py-8">References</h2>

		<p class="dark:text-white text-lg">
			<a
				href="https://flowbite.com/docs/components/footer/"
				target="_blank"
				class="text-blue-600 hover:underline dark:text-blue-500">Flowbite Footer</a
			>
		</p>
	</div>

	<div class="container my-16 mx-auto">
		<Utterances reponame="shinokada/flowbite-svelte" theme="dark-blue" />
	</div>
</div>

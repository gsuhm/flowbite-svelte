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
				href="https://flowbite-svelte.vercel.app/buttons/setup"
				class="text-blue-600 hover:underline dark:text-blue-500">Button Setup</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/buttons/default"
				class="text-blue-600 hover:underline dark:text-blue-500">Default Button</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/buttons/colored-shadow"
				class="text-blue-600 hover:underline dark:text-blue-500">Colored Shadow Button</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/buttons/gradient-duotone"
				class="text-blue-600 hover:underline dark:text-blue-500">Gradient Duotone Button</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/buttons/gradient-monochrome"
				class="text-blue-600 hover:underline dark:text-blue-500">Gradient Monochrome Button</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/buttons/gradient-outline"
				class="text-blue-600 hover:underline dark:text-blue-500">Gradietn Outline Button</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/buttons/outlined"
				class="text-blue-600 hover:underline dark:text-blue-500">Outlined Button</a
			>
		</p>

		<p class="dark:text-white text-lg w-full">
			<a
				href="https://flowbite-svelte.vercel.app/buttons/rounded"
				class="text-blue-600 hover:underline dark:text-blue-500">Rounded Button</a
			>
		</p>

		<h2 class="text-2xl w-full dark:text-white py-8">References</h2>

		<p class="dark:text-white text-lg">
			<a
				href="https://flowbite.com/docs/components/buttons/"
				target="_blank"
				class="text-blue-600 hover:underline dark:text-blue-500">Flowbite Buttons</a
			>
		</p>
	</div>

	<div class="container my-16 mx-auto">
		<Utterances reponame="shinokada/flowbite-svelte" theme="dark-blue" />
	</div>
</div>

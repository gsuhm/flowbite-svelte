---
layout: modalLayout
---

<script>
  import { MediumModal, ModalButton, modalIdStore }from '$lib/index';

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  // modal 1
  const id = "basic-modal";
  const btnBasicName = "Medium Modal for information";

  // modal 2
  let id1 = "medium-modal";
  let btnMName = "Medium Modal with one button";
  let btnColor = "pink";

  const handlebtnM1 = () => {
    closeModal()
  };

  // modal 3
  let id2 = "medium-modal2";
  let btnName2 = "Medium Modal with two buttons";
  let btnColor2 = "purple";

  const handlebtnM2 = () => {
    closeModal()
  };
  const handlebtnM3 = () => {
    closeModal()
  };
</script>


<h1 class="text-3xl w-full dark:text-white py-8">Medium Modals</h1>

<h2 class="text-2xl w-full dark:text-white py-8">Set up</h2>

<p class="dark:text-white py-4 text-lg">Import MediumModal, ModalButton, modalIdStor components and set variables in the script tag. Add `closeModal` method if you want to close the modal in a button.</p>

```html
<script>
  import { MediumModal, ModalButton, modalIdStore } from "flowbite-svelte";

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  // modal 1
  const id = "basic-modal";
  const btnBasicName = "Medium Modal for information";

  // modal 2
  let id1 = "medium-modal";
  let btnMName = "Medium Modal with one button";
  let btnColor = "pink";

  const handlebtnM1 = () => {
    closeModal()
  };

  // modal 3
  let id2 = "medium-modal2";
  let btnName2 = "Medium Modal with two buttons";
  let btnColor2 = "purple";

  const handlebtnM2 = () => {
    closeModal()
  };
  const handlebtnM3 = () => {
    closeModal()
  };
</script>
```

<h2 class="text-2xl w-full dark:text-white py-8">Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
type Colors = 'blue' | 'gray' | 'red' | 'yellow' | 'purple' | 'green' | 'indigo' | 'pink';
let id = 'medium-modal';
let btnColor: Colors = 'blue';
let textColor: Colors = 'gray';
let title = 'Terms of Service';
let btn1: string;
let btn2: string;
let showModalId: string;
```

<h2 class="text-2xl w-full dark:text-white py-8">Examples</h2>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton {id} btnName={btnBasicName} />
</div>

<p class="dark:text-white py-4 text-lg"> Create a button and modal.</p>

```html
<ModalButton {id} btnName={btnBasicName} />
<MediumModal {id} title="Basic Modal Title">
  Basic Modal Content: Lorem ipsum dolor sit, amet consectetur adipisicing elit.
  Ad odit aspernatur minus deserunt illo error eum temporibus officiis. 
</MediumModal>
```

<h2 class="text-2xl w-full dark:text-white py-8">Medium Modals with an Action Button</h2>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton id={id1} btnName={btnMName} {btnColor} />
</div>

```html
<ModalButton id={id1} btnName={btnMName} {btnColor} />
<MediumModal
  id={id1}
  btnColor="yellow"
  title="Medium Modal Title"
  btn1="Yes"
  on:handlebtn1={handlebtnM1}
>
  Modal 2 Content: Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ad
  odit aspernatur minus deserunt illo error eum temporibus officiis. 
</MediumModal>
```

<h2 class="text-2xl w-full dark:text-white py-8">Medium Modals with action buttons</h2>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
</div>

```html
<ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
<MediumModal
  id={id2}
  btnColor="indigo"
  title="Default Modal Title"
  btn1="Yes"
  btn2="No"
  on:handlebtn1={handlebtnM2}
  on:handlebtn2={handlebtnM3}
>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.
</MediumModal>
```

<MediumModal {id} title="Basic Modal Title">
  Basic Modal Content: Lorem ipsum dolor sit, amet consectetur adipisicing
  elit. Ad odit aspernatur minus deserunt illo error eum temporibus officiis.
  Ab facere dolorem quisquam omnis? Aspernatur, asperiores voluptas quis culpa
  consectetur saepe!
</MediumModal>

<MediumModal
  id={id1}
  btnColor="yellow"
  title="Medium Modal Title"
  btn1="Yes"
  on:handlebtn1={handlebtnM1}
>
  Modal 2 Content: Lorem ipsum dolor sit, amet consectetur adipisicing elit.
  Ad odit aspernatur minus deserunt illo error eum temporibus officiis. Ab
  facere dolorem quisquam omnis? Aspernatur, asperiores voluptas quis culpa
  consectetur saepe!
</MediumModal>

<MediumModal
  id={id2}
  btnColor="indigo"
  title="Default Modal Title"
  btn1="Yes"
  btn2="No"
  on:handlebtn1={handlebtnM2}
  on:handlebtn2={handlebtnM3}
>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
  tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
  quis nostrud exercitation ullamco.
</MediumModal>


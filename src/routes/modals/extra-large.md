---
layout: modalLayout
---

<script>
  import { ModalButton, ExtraLargeModal, modalIdStore }from '$lib/index';

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  // simple modal
  let id = "simple";

  // Modal 1
  let id1 = "extra-large-modal";
  let btnExLName = "Extra Large Modal with one button";
  let btnExLColor = "blue";

  // Modal 2
  let id2 = "extra-large-modal-2";
  let btnExLName2 = "Extra Large Modal with two buttons";
  let btnExLColor2 = "purple";
  let btn1 = "Read more";
  let btn2 = "Close";

  const handlebtn1 = () => {
    alert("handlebtn1 is clicked from a parent page.");
    closeModal()
  };

  const handlebtn2 = () => {
    alert("handlebtn2 is clicked from a parent page.");
    closeModal()
  };

  const handlebtn3 = () => {
    alert("handlebtn3 is clicked from a parent page.");
    closeModal()
  };
</script>

<h1 class="text-3xl w-full dark:text-white py-8">Extra-large Modals</h1>

<h2 class="text-2xl w-full dark:text-white py-8">Setup</h2>

<p class="dark:text-white py-4 text-lg">Import ExtraLargeModal, ModalButton, modalIdStor components and set variables in the script tag. Add `closeModal` method if you want to close the modal in a button.</p>


```html
<script>
  import { ModalButton, ExtraLargeModal, modalIdStore } from "flowbite-svelte";

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  // simple modal
  let id = "simple";

  // Modal 1
  let id1 = "extra-large-modal";
  let btnExLName = "Extra Large Modal with one button";
  let btnExLColor = "blue";

  // Modal 2
  let id2 = "extra-large-modal-2";
  let btnExLName2 = "Extra Large Modal with two buttons";
  let btnExLColor2 = "purple";
  let btn1 = "Read more";
  let btn2 = "Close";

  const handlebtn1 = () => {
    alert("handlebtn1 is clicked from a parent page.");
    closeModal()
  };

  const handlebtn2 = () => {
    alert("handlebtn2 is clicked from a parent page.");
    closeModal()
  };

  const handlebtn3 = () => {
    alert("handlebtn3 is clicked from a parent page.");
    closeModal()
  };
</script>
```

<h2 class="text-2xl w-full dark:text-white py-8">Props</h2>

<p class="dark:text-white py-4 text-lg">The component has the following props, type, and default values:</p>

```js
type Colors = 'blue' | 'gray' | 'red' | 'yellow' | 'purple' | 'green' | 'indigo' | 'pink';
let id = 'extralarge-modal';
let btnColor: Colors = 'blue';
let textColor: Colors = 'gray';
let title = 'Terms of Service';
let btn1: string;
let btn2: string;
let showModalId: string;
```

<h2 class="text-2xl w-full dark:text-white py-8">Examples</h2>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton {id} btnName="Info Modal" />
</div>

<p class="dark:text-white py-4 text-lg"> Create a button and modal.</p>

```html
<ModalButton {id} btnName="Info Modal" />

<ExtraLargeModal {id} title="Info Modal">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.
</ExtraLargeModal>
```

<h2 class="text-2xl w-full dark:text-white py-8">Extra-large Modals with One Button</h2>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton id={id1} btnName={btnExLName} btnColor={btnExLColor} />
</div>

<p class=" dark:text-white py-4"> Create a button and modal.</p>

```html
<ModalButton id={id1} btnName={btnExLName} btnColor={btnExLColor} />

<ExtraLargeModal
  id={id1}
  title="Default Modal Title"
  {btn1}
  on:handlebtn1={handlebtn1}
>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.
</ExtraLargeModal>
```

<h2 class="text-2xl w-full dark:text-white py-8">Extra-large Modals with Two Buttons</h2>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton id={id2} btnName={btnExLName2} btnColor={btnExLColor2} />
</div>

<p class=" dark:text-white py-4">Create a button and modal.</p>

```html
<ModalButton id={id2} btnName={btnExLName2} btnColor={btnExLColor2} />

<ExtraLargeModal
  id={id2}
  btnColor="indigo"
  textColor="red"
  title="Default Modal Title"
  {btn1}
  {btn2}
  on:handlebtn1={handlebtn2}
  on:handlebtn2={handlebtn3}
>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.
</ExtraLargeModal>
```

  <ExtraLargeModal {id} title="Info Modal">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco.
  </ExtraLargeModal>

  <ExtraLargeModal
    id={id1}
    title="Default Modal Title"
    {btn1}
    on:handlebtn1={handlebtn1}
  >
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco.
  </ExtraLargeModal>

  <ExtraLargeModal
    id={id2}
    btnColor="indigo"
    textColor="red"
    title="Default Modal Title"
    {btn1}
    {btn2}
    on:handlebtn1={handlebtn2}
    on:handlebtn2={handlebtn3}
  >
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco.
  </ExtraLargeModal>


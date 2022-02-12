---
layout: doc
---

<script>
  import { SmallModal, ModalButton, modalIdStore } from "svelte-flow";
  import { goto } from "$app/navigation";

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  // common
  const textSColor = "blue";

  // for basic
  const idBasic = "basic-modal";
  const btnBasicName = "Basic Modal";

  // for small modal 1
  const btnName1 = "Small Modal";
  const id1 = "small-modal";
  const btnColor1 = "purple";

  const handlebtnS1 = () => {
    closeModal()
    goto("/about");
  };

  const handlebtnS2 = () => {
    closeModal()
  };

  // for small modal 2
  const btnName2 = "Small Modal 2";
  const id2 = "small-modal-2";
  const btnColor2 = "red";

  const handlebtnS3 = () => {
    closeModal()
  };

  const handlebtnS4 = () => {
    closeModal()
  };
</script>

<h1 class="text-3xl w-full dark:text-white">Small Modals: Setup</h1>

<p class="dark:text-white my-4">Import SmallModal, ModalButton, modalIdStor components and set variables in the script tag. Add `closeModal` method if you want to close the modal in a button.</p>

```svelte
<script>
  import { SmallModal, ModalButton, modalIdStore } from "svelte-flow";
  import { goto } from "$app/navigation";

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  // common
  const textSColor = "blue";

  // for basic
  const idBasic = "basic-modal";
  const btnBasicName = "Basic Modal";

  // for small modal 1
  const btnName1 = "Small Modal";
  const id1 = "small-modal";
  const btnColor1 = "purple";

  const handlebtnS1 = () => {
    closeModal()
    goto("/about");
  };

  const handlebtnS2 = () => {
    closeModal()
  };

  // for small modal 2
  const btnName2 = "Small Modal 2";
  const id2 = "small-modal-2";
  const btnColor2 = "red";

  const handlebtnS3 = () => {
    closeModal()
  };

  const handlebtnS4 = () => {
    closeModal()
  };
</script>
```

<h1 class="text-3xl w-full dark:text-white">Small Modals</h1>

<div class="container flex flex-wrap my-8 mx-auto justify-center">
  <ModalButton id={idBasic} btnName={btnBasicName} />
</div>

<p class="dark:text-white pb-4">Create a button and modal.</p>

```svelte
<ModalButton id={idBasic} btnName={btnBasicName} />
<SmallModal id={idBasic} title={"Basic Modal Title"}>
  Basic Modal Content
</SmallModal>
```

<h1 class="text-3xl w-full dark:text-white">Small Modals with Action Buttons</h1>

<div class="container flex flex-wrap my-8 mx-auto justify-center">
  <ModalButton id={id1} btnName={btnName1} btnColor={btnColor1} />
</div>

```svelte
<ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
<SmallModal
  id={id1}
  btnColor={"pink"}
  title={"Small Modal Title"}
  btn1="View"
  btn2="No"
  on:handlebtn1={handlebtnS1}
  on:handlebtn2={handlebtnS2}
>
  Modal 1: Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
  sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
</SmallModal>
```

<h1 class="text-3xl w-full dark:text-white">Small Modals with different colors</h1>

<div class="container flex flex-wrap my-8 mx-auto justify-center">
  <ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
</div>

```svelte
<ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
<SmallModal
  id={id2}
  btnColor={"yellow"}
  textColor={textSColor}
  title={"Small Modal Title"}
  btn1="Yes"
  btn2="No"
  on:handlebtn1={handlebtnS3}
  on:handlebtn2={handlebtnS4}
>
  Modal 2: Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
  sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
</SmallModal>
```

<SmallModal id={idBasic} title={"Basic Modal Title"}>
  Basic Modal Content
</SmallModal>

  <SmallModal
    id={id1}
    btnColor={"pink"}
    title={"Small Modal Title"}
    btn1="View"
    btn2="No"
    on:handlebtn1={handlebtnS1}
    on:handlebtn2={handlebtnS2}
  >
    Modal 1: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
eiusmod tempor incididunt ut labore et dolore magna aliqua.
  </SmallModal>

  <SmallModal
    id={id2}
    btnColor={"yellow"}
    textColor={textSColor}
    title={"Small Modal Title"}
    btn1="Yes"
    btn2="No"
    on:handlebtn1={handlebtnS3}
    on:handlebtn2={handlebtnS4}
  >
    Modal 2: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
    eiusmod tempor incididunt ut labore et dolore magna aliqua.
  </SmallModal>

<h1 class="text-3xl w-full dark:text-white pb-8">References</h1>

<p class="dark:text-white text-base"><a href="https://flowbite.com/docs/components/modal/" target="_blank">- Flowbite Modal</a></p>

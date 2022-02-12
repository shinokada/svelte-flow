---
layout: doc
---

<script>
  import { MediumModal, ModalButton, modalIdStore } from "svelte-flow";

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
  let textMColor = "red";

  const handlebtnM1 = () => {
    closeModal()
  };

  // modal 3
  let id2 = "medium-modal2";
  let btnName2 = "Medium Modal with two buttons";
  let textMColor2 = "yellow";
  let btnColor2 = "purple";

  const handlebtnM2 = () => {
    closeModal()
  };
  const handlebtnM3 = () => {
    closeModal()
  };
</script>


<h1 class="text-3xl w-full dark:text-white">Medium Modals: Setup</h1>

<p class="dark:text-white my-4">Import MediumModal, ModalButton, modalIdStor components and set variables in the script tag. Add `closeModal` method if you want to close the modal in a button.</p>

```svelte
<script>
  import { MediumModal, ModalButton, modalIdStore } from "svelte-flow";

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
  let textMColor = "red";

  const handlebtnM1 = () => {
    closeModal()
  };

  // modal 3
  let id2 = "medium-modal2";
  let btnName2 = "Medium Modal with two buttons";
  let textMColor2 = "yellow";
  let btnColor2 = "purple";

  const handlebtnM2 = () => {
    closeModal()
  };
  const handlebtnM3 = () => {
    closeModal()
  };
</script>
```

<h1 class="text-3xl w-full dark:text-white pb-4">Medium Modals for Information</h1>

<div class="container flex flex-wrap my-8 mx-auto justify-center">
  <ModalButton {id} btnName={btnBasicName} />
</div>

<p class="dark:text-white pb-4"> Create a button and modal.</p>

```svelte
<ModalButton {id} btnName={btnBasicName} />
<MediumModal {id} title={"Basic Modal Title"}>
  Basic Modal Content: Lorem ipsum dolor sit, amet consectetur adipisicing elit.
  Ad odit aspernatur minus deserunt illo error eum temporibus officiis. 
</MediumModal>
```

<h1 class="text-3xl w-full dark:text-white pb-4">Medium Modals with an Action Button</h1>

<div class="container flex flex-wrap my-8 mx-auto justify-center">
  <ModalButton id={id1} btnName={btnMName} {btnColor} />
</div>

```svelte
<ModalButton id={id1} btnName={btnMName} {btnColor} />
<MediumModal
  id={id1}
  btnColor={"yellow"}
  title={"Medium Modal Title"}
  textColor={textMColor}
  btn1="Yes"
  on:handlebtn1={handlebtnM1}
>
  Modal 2 Content: Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ad
  odit aspernatur minus deserunt illo error eum temporibus officiis. 
</MediumModal>
```

<h1 class="text-3xl w-full dark:text-white pb-8">Medium Modals with action buttons</h1>

<div class="container flex flex-wrap my-8 mx-auto justify-center">
  <ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
</div>

```svelte
<ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
<MediumModal
  id={id2}
  btnColor={"indigo"}
  title={"Default Modal Title"}
  textColor={textMColor2}
  btn1="Yes"
  btn2="No"
  on:handlebtn1={handlebtnM2}
  on:handlebtn2={handlebtnM3}
>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.
</MediumModal>
```

  <MediumModal {id} title={"Basic Modal Title"}>
    Basic Modal Content: Lorem ipsum dolor sit, amet consectetur adipisicing
    elit. Ad odit aspernatur minus deserunt illo error eum temporibus officiis.
    Ab facere dolorem quisquam omnis? Aspernatur, asperiores voluptas quis culpa
    consectetur saepe!
  </MediumModal>

  <MediumModal
    id={id1}
    btnColor={"yellow"}
    title={"Medium Modal Title"}
    textColor={textMColor}
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
    btnColor={"indigo"}
    title={"Default Modal Title"}
    textColor={textMColor2}
    btn1="Yes"
    btn2="No"
    on:handlebtn1={handlebtnM2}
    on:handlebtn2={handlebtnM3}
  >
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco.
  </MediumModal>

<h1 class="text-3xl w-full dark:text-white pb-8">References</h1>

<p class="dark:text-white text-base"><a href="https://flowbite.com/docs/components/modal/" target="_blank">- Flowbite Modal</a></p>
---
layout: doc
---

<script>
  import { SignInModal, ModalButton, modalIdStore } from "svelte-flow";

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  let signinId = "signin-modal2";
  let btnSignInName = "Sign In Modal";
  let btnSignInColor = "blue";
</script>

<h1 class="text-3xl w-full dark:text-white">Sign-in Modals: Setup</h1>

<p class="dark:text-white text-base">Import SignInModal, ModalButton components and set variables in the script tag.</p>

```svelte
import { SignInModal, ModalButton, modalIdStore } from "svelte-flow";

let signinId = "signin-modal2";
let btnSignInName = "Sign In Modal";
let btnSignInColor = "blue";
```

<h1 class="text-3xl w-full dark:text-white">SignIn Modals</h1>

<div class="container flex flex-wrap justify-center rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton
    id={signinId}
    btnName={btnSignInName}
    btnColor={btnSignInColor}
  />
</div>

<p class="dark:text-white text-base">Create a button and modal.</p>

```svelte
<ModalButton
  id={signinId}
  btnName={btnSignInName}
  btnColor={btnSignInColor}
/>
<SignInModal
  id={signinId}
  btnSignInColor={"pink"}
  titleSignIn={"SignIn Modal Title"}
  textSignInColor="pink"
  lostPasswordLink={"/auth/lost-password"}
  signUpLink={"/auth/signup"}
  formLink={"/auth/signin"}
/>
```

  <SignInModal
    id={signinId}
    btnSignInColor={"pink"}
    titleSignIn={"SignIn Modal Title"}
    textSignInColor="pink"
    lostPasswordLink={"/"}
    signUpLink={"/about"}
    formLink={"/modals"}
  />

<h1 class="text-3xl w-full dark:text-white pb-8">References</h1>

<p class="dark:text-white text-base"><a href="https://flowbite.com/docs/components/modal/" target="_blank" class="text-blue-600 hover:underline dark:text-blue-500">- Flowbite Modal</a></p>

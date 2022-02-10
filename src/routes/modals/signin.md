---
layout: doc
---

<script>
  import { SignInModal, ModalButton } from "svelte-flow";

  let signinId = "signin-modal2";
  let btnSignInName = "Sign In Modal";
  let btnSignInColor = "blue";
</script>

<h1 class="text-3xl w-full dark:text-white">Sign-in Modals: Setup</h1>

<p class="dark:text-white text-base">Import SignInModal, ModalButton components and set variables in the script tag.</p>

```svelte
import { SignInModal, ModalButton } from "svelte-flow";

let signinId = "signin-modal2";
let btnSignInName = "Sign In Modal";
let btnSignInColor = "blue";
```

<h1 class="text-3xl w-full dark:text-white">SignIn Modals</h1>

<div class="container flex flex-wrap my-8 mx-auto justify-center">
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
    lostPasswordLink={"/auth/lost-password"}
    signUpLink={"/auth/signup"}
    formLink={"/auth/signin"}
  />

<h1 class="text-3xl w-full dark:text-white pb-8">References</h1>

<p class="dark:text-white text-base"><a href="https://flowbite.com/docs/components/modal/" target="_blank">- Flowbite Modal</a></p>

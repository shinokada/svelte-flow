<script>
  import { ModalButton, ExtraLargeModal, modalIdStore } from "$lib/index";

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
  let btnExLColor = "purple";

  // Modal 2
  let id2 = "extra-large-modal-2";
  let btnExLName2 = "Extra Large Modal with two buttons";
  let btnExLColor2 = "red";
  let btn1 = "Read more";
  let btn2 = "Close";

  const handlebtn1 = () => {
    alert("handlebtn1 is clicked from a parent page.");
    closeModal();
  };

  const handlebtn2 = () => {
    alert("handlebtn2 is clicked from a parent page.");
    closeModal();
  };

  const handlebtn3 = () => {
    alert("handlebtn3 is clicked from a parent page.");
    closeModal();
  };
</script>

<div class="block p-8 space-y-4 md:flex md:space-y-0 md:space-x-4">
  <ModalButton {id} btnName="Info Modal" />
  <ModalButton id={id1} btnName={btnExLName} btnColor={btnExLColor} />
  <ModalButton id={id2} btnName={btnExLName2} btnColor={btnExLColor2} />
</div>

<ExtraLargeModal {id} title="Info Modal">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
  nostrud exercitation ullamco.
</ExtraLargeModal>

<ExtraLargeModal
  id={id1}
  title="Default Modal Title"
  {btn1}
  btnColor="yellow"
  on:handlebtn1={handlebtn1}
>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
  nostrud exercitation ullamco.
</ExtraLargeModal>

<ExtraLargeModal
  id={id2}
  btnColor="indigo"
  textColor="gray"
  title="Default Modal Title"
  {btn1}
  {btn2}
  on:handlebtn1={handlebtn2}
  on:handlebtn2={handlebtn3}
>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
  nostrud exercitation ullamco.
</ExtraLargeModal>

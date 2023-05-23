<script>
  import Modal from "components/Modal/Modal.svelte";

  
  let showModal = false;
  
  export function toggle() {
     showModal = !showModal;
  }

</script>
<Modal bind:showModal>

</Modal>
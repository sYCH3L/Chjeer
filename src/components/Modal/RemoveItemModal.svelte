<script>
  import Modal from "components/Modal/Modal.svelte";

  
  let showModal = false;
  
  export function toggle() {
     showModal = !showModal;
  }

</script>
<Modal bind:showModal>
	<p slot="accept-button-name"> sugu	</p>
  <p slot="body">olen peeter paan ja nikun sigu </p>
</Modal>
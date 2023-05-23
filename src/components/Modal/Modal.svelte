<script>
	export let showModal; // boolean

	let dialog; // HTMLDialogElement

	$: if (dialog && showModal) dialog.showModal();
</script>

<!-- svelte-ignore a11y-click-events-have-key-events on:click|stopPropagation -->
<dialog bind:this={dialog} on:close={() => (showModal = false)} on:click|self={() => dialog.close()}>

<div class="relative flex w-full flex-wrap items-stretch mb-3 my-11 h-10 active:border-indigo-500 group">
  <span class="z-10 h-full leading-snug font-normal absolute text-center text-slate-400 absolute bg-transparent border-[0.7px] border-gray-20 items-center justify-center w-8 py-2 rounded-l group-focus-within:border-blue-500">
    $
  </span>
  <input type="number" placeholder="Small Input" class="px-2 py-1 placeholder-slate-400 relative bg-white bg-white rounded outline-none border-l border-[0.7px] border-gray-20 bordf text-sm w-full pl-10 group-focus-within:border-blue-500"/>
</div>
</dialog>
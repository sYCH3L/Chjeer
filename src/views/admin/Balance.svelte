<script>
  // core components

import CardAssets from "components/Cards/CardAssets.svelte"
import CardLiablities from "components/Cards/CardLiablities.svelte"
  
  
  export let location;
</script>

<div>
  <div class="flex flex-wrap">
    <div class="w-full xl:w-8/12 mb-12 xl:mb-0 px-4">
      <CardAssets />
    </div>
  </div>
  <div class="flex flex-wrap mt-4">
    <div class="w-full xl:w-8/12 mb-12 xl:mb-0 px-4">
      <CardLiablities /> 
    </div>
  </div>
</div>
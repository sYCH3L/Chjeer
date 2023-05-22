<script>
  // core components
  import CardFinanceTable from "components/Cards/CardFinanceTable.svelte";
  import RemoveItemModal from "components/Modal/RemoveItemModal.svelte";
  export let location;
  
  let Data = [{
    Headings: ["Name","$",""],
    Entries: [{
        id: 0,
        Titles: [],
        Data: ["Work","4,700"]
    }]
    
}];

function ShowItem()
{
  RemoveItemModal.model.toggle();
}

</script>

<RemoveItemModal/>
<div>
  <div class="flex flex-wrap">
    <div class="w-full xl:w-8/12 mb-12 xl:mb-0 px-4">
      <CardFinanceTable TableName="TestData" Data={Data} showAddItem={ShowItem}/>
    </div>
  </div>
</div>
<script>
  // core components
  import CardFinanceTable from "components/Cards/CardFinanceTable.svelte";
  export let location;
  
  let Data = [{
    Headings: ["Name","$",""],
    Entries: [{
        id: 0,
        Titles: [],
        Data: ["Work","4,700"]
    }]
    
}];


    function EditItem(id) {
      console.log("Editing item: " + id)
    }
    function RemoveItem(id) {
      console.log("Removing item: " + id)
    }
    
    function AppendItem() {
      console.log("Appending item")
    }

</script>


<div>
  <div class="flex flex-wrap">
    <div class="w-full xl:w-8/12 mb-12 xl:mb-0 px-4">
      <CardFinanceTable TableName="TestData" Data={Data} EditItem={EditItem} RemoveItem={RemoveItem} AppendItem={AppendItem}/>
    </div>
  </div>
</div>
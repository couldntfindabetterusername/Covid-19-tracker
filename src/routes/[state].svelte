<script context="module">
  export async function preload(page) {
    console.log(page);
    return { state: page.params["state"] };
  }
</script>

<script>
  export let state;

  import CovidData from "../components/CovidData.svelte";
  import CovidGraph from "../components/CovidGraph.svelte";

  import TableContainer from "../components/TableContainer.svelte";
</script>

<svelte:head> 
  <title>Covid-19 Tracker</title>
</svelte:head>

<div class="section header">
  <div class="container">
    <h1>Covid-19 {state}</h1>
  </div>
</div>
<h1>{state}</h1>
<CovidData />
<CovidGraph />

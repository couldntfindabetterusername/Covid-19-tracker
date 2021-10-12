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

<h1>{state}</h1>
<CovidData />
<CovidGraph />

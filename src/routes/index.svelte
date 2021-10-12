<script>
  import CovidData from "../components/CovidData.svelte";
  import CovidGraph from "../components/CovidGraph.svelte";

  import TableContainer from "../components/TableContainer.svelte";
</script>

<svelte:head>
  <title>Covid-19 Tracker</title>
</svelte:head>

<div class="section header">
  <div class="container">
    <h1>Covid-19 India</h1>
  </div>
</div>

<CovidData />
<CovidGraph />
<TableContainer />

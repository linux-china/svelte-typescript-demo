<script lang="ts" type="typescript">
  let tuple1: [string,string,string] = ["Svelte","Typescript","Rollup"]
  let a: string = "Svelte";
  let b: string = "Typescript";
  let  c: string = "Rollup";

  function click1() {
     tuple1[0]="Clicked"
  }

</script>

<style lang="scss">
  :global(body) {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
  }

  h1 {
    font: normal 24pt Lato, "Helvetica Neue", Arial, Helvetica, sans-serif;
    color: dimgray;
    cursor: default;
  }
</style>

<button on:click="{click1}">click</button>

<h1>{tuple1[0]} + {tuple1[1]} + {tuple1[2]}</h1>


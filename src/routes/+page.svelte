<script lang="ts">
  import {onMount} from "svelte";
  import Sarus from "@anephenix/sarus";
  function makeSarus(): Sarus {
    return new Sarus({ url: "bogus-url"});
  }

  function action() {
    console.log("Constructing sarus");
    const sarus = makeSarus();
    console.log(sarus);
  }

  onMount(() => {
    action();
  });
</script>
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

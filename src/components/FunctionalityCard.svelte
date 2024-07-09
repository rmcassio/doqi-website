<script lang="ts">
  import ElevatedButton from "./ElevatedButton.svelte";

  export let title: string;
  export let description: string;
</script>

<div
  class="text-center flex flex-col items-center justify-center p-6 rounded-lg shadow-md bg-white"
>
  <h2 class="text-2xl font-bold text-red-500 mb-2">{title}</h2>
  <p class="text-gray-600 mb-4">{description}</p>
  <ElevatedButton label="Saiba mais" />
</div>

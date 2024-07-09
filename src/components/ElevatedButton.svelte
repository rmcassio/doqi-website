<script lang="ts">
  export let label: string = "Button";
  export let onClick: () => void = () => {};
  export let color: string = "bg-black";
  export let hoverColor: string = "hover:bg-gray-600";
  export let textColor: string = "text-white";
  export let width: string | null = null;
</script>

<div class="container py-2">
  <button
    on:click={onClick}
    class="btn py-1 {color} border-none hover:outline-none {hoverColor} {textColor} {width}"
    >{label}</button
  >
</div>

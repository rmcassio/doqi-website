<script lang="ts">
  export let withBackground = false;
  export let isFooter = false;
</script>

<nav class={!isFooter ? "hidden md:flex" : ""}>
  <ul
    class="menu menu-horizontal rounded-box {withBackground
      ? 'bg-base-200'
      : ''}"
  >
    <li>
      <a href="functionalities">
        <span class="block px-2 text-black">Funcionalidades</span>
      </a>
    </li>
    <li>
      <a href="plans-and-prices">
        <span class="block px-2 text-black">Planos e preços</span>
      </a>
    </li>
    <li>
      <a href="contact">
        <span class="block px-2 text-black">Fale conosco</span>
      </a>
    </li>
  </ul>
</nav>

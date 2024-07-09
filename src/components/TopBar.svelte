<script lang="ts">
  import NavButton from "./NavButton.svelte";

  let isOpen: boolean = false;

  function toggleDrawer() {
    isOpen = !isOpen;
  }

  function closeDrawer() {
    isOpen = false;
  }
</script>

<nav class=" fixed top-0 w-full bg-white shadow-lg z-50 px-4">
  <div class="container mx-auto flex items-center justify-between py-3 sm:py-2">
    <a href="/" class="text-3xl font-bold text-red-500">DOQI</a>
    <NavButton />
    <div class="md:hidden">
      <button on:click={toggleDrawer} class="focus:outline-none">
        <svg
          class="w-6 h-6 text-gray-700"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16m-7 6h7"
          ></path>
        </svg>
      </button>
    </div>
  </div>
  {#if isOpen}
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-no-static-element-interactions -->
    <div
      class="fixed inset-0 bg-gray-800 bg-opacity-50 z-40"
      on:click={closeDrawer}
    ></div>
    <div class="fixed inset-y-0 right-0 bg-white shadow-md w-64 z-50 md:hidden">
      <div
        class="border-b border-gray-200 p-4 flex justify-between items-center"
      >
        <h2 class="text-lg font-semibold">Menu</h2>

        <button
          on:click={closeDrawer}
          class="btn btn-square btn-outline btn-sm no-animation"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M6 18L18 6M6 6l12 12"
            />
          </svg>
        </button>
      </div>
      <div class="p-4">
        <a
          href="functionalities"
          class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded"
          on:click={closeDrawer}
        >
          Funcionalidades
        </a>
        <a
          href="plans-and-prices"
          class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded"
          on:click={closeDrawer}
        >
          Planos e preços
        </a>
        <a
          href="contact"
          class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded"
          on:click={closeDrawer}
        >
          Fale conosco
        </a>
      </div>
    </div>
  {/if}
</nav>

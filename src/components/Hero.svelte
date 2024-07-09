<script>
  import ElevatedButton from "./ElevatedButton.svelte";

  let label = "comece agora";
  let onClick = () => {
    window.location.href = "register";
  };
</script>

<section class="bg-red-500 text-white py-40 px-4">
  <div
    class="container mx-auto flex flex-col md:flex-row items-center justify-between"
  >
    <div class="md:w-1/2">
      <h1 class="text-5xl">Simplifique seus negócios</h1>
      <h2 class="text-4xl mt-4">
        sistema de gestão online para a sua empresa.
      </h2>
      <p class="mt-4 text-lg">
        o Doqi é um sistema agregador de dados que simplifica o controle entre
        seus negócios em uma única plataforma, além de realizar integrações com
        as principais plataformas de e-commerce e marketplaces.
      </p>
      <ElevatedButton {label} {onClick} />
    </div>
    <div class="hidden md:flex md:w-1/2 justify-center md:justify-end">
      <img src="doqi.png" alt="" />
    </div>
  </div>
</section>

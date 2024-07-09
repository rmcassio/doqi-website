<script>
  import ElevatedButton from "../../components/ElevatedButton.svelte";
</script>

<div
  class=" min-h-screen flex flex-col items-center justify-center bg-white p-4 my-8"
>
  <h1 class="text-center text-5xl font-bold text-red-500 mb-12 mt-6">
    Entre em contato
  </h1>
  <div class=" grid grid-cols-1 md:grid-cols-2 gap-6">
    <!-- Existing Client Section -->
    <div class="card shadow-lg bg-gray-100 rounded-lg px-12 py-16">
      <h2 class="text-xl font-semibold text-red-500 mb-4">
        É cliente Doqui e está precisando de ajuda?
      </h2>
      <div class="mb-4">
        <h3 class="text-lg font-semibold">Central de ajuda</h3>
        <p>Veja nossos manuais, dicas e tutoriais para te ajudar</p>
        <ElevatedButton
          label="Ver manuais"
          color="bg-red-500"
          textColor="text-gray-100"
        />
      </div>
      <div>
        <h3 class="text-lg font-semibold">Suporte</h3>
        <p>+55 (54) 3771-7278<br />Horário de suporte das 8:20 às 17:45</p>
        <ElevatedButton
          label="Abrir chamado"
          color="bg-red-500"
          textColor="text-gray-100"
        />
      </div>
    </div>
    <!-- New Client Section -->
    <div class="card shadow-md bg-gray-50 rounded-lg px-12 py-16">
      <h2 class="text-xl font-semibold text-gray-700 mb-4">
        Ainda não é cliente
      </h2>
      <div class="mb-4">
        <h3 class="text-lg font-semibold">Telefone</h3>
        <p>+55 (54) 3771-7278<br />Horário comercial das 8:20 às 17:15</p>
      </div>
      <div class="mb-4">
        <h3 class="text-lg font-semibold">Email</h3>
        <p>comercial@bling.com.br</p>
      </div>
      <div>
        <h3 class="text-lg font-semibold">Chat</h3>
        <p>Horário comercial das 8:20 às 17:15</p>
        <ElevatedButton
          label="Abrir WhatsApp"
          color="bg-gray-400"
          textColor="text-gray-50"
        />
      </div>
    </div>
  </div>

  <div class="card bg-black bg-opacity-5 w-100 shadow-lg my-12">
    <div class="card-body">
      <div class="card-actions justify-end"></div>
      <p>
        Endereço: Rua Olavo Bilac, 914, sala 101 térreo - Imigrante | Bento
        Gonçalves - RS Brasil - CEP 95720-000
      </p>
    </div>
  </div>
</div>

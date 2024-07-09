<script lang="ts">
  import ElevatedButton from "../../components/ElevatedButton.svelte";

  let username = "";
  let email = "";
  let password = "";
  let termsAccepted = false;

  let label = "registrar";

  const handleSubmit = () => {
    console.log({ username, email, password, termsAccepted });
  };
</script>

<div class="flex items-center justify-center min-h-screen">
  <div class="bg-white p-8 rounded-lg shadow-md w-full max-w-md">
    <h1 class="text-2xl font-bold mb-6">Comece o seu teste grátis!</h1>
    <form on:submit|preventDefault={handleSubmit}>
      <div class="mb-4">
        <label for="username" class="block text-sm font-medium text-gray-700"
          >Usuário (sem espaços e caracteres especiais)</label
        >
        <input
          id="username"
          type="text"
          bind:value={username}
          class="input input-bordered w-full"
          placeholder="Digite o nome para o seu usuário"
          required
        />
      </div>
      <div class="mb-4">
        <label for="email" class="block text-sm font-medium text-gray-700"
          >Seu melhor e-mail</label
        >
        <input
          id="email"
          type="email"
          bind:value={email}
          class="input input-bordered w-full"
          placeholder="Digite o seu e-mail"
          required
        />
      </div>
      <div class="mb-4">
        <label for="password" class="block text-sm font-medium text-gray-700"
          >Senha</label
        >
        <input
          id="password"
          type="password"
          bind:value={password}
          class="input input-bordered w-full"
          placeholder="12 ou mais caracteres"
          minlength="12"
          required
        />
      </div>
      <div class="mb-4">
        <label class="inline-flex items-center">
          <input
            type="checkbox"
            bind:checked={termsAccepted}
            class="checkbox [--chkbg:theme(colors.red.500)] [--chkfg:white] checked:border-red-500"
            required
          />
          <span class="ml-2"
            >Declaro ter lido e aceito os <a
              href="#"
              class="text-blue-500 underline">termos de serviço</a
            >
            e as
            <a href="#" class="text-blue-500 underline">políticas</a></span
          >
        </label>
      </div>
      <ElevatedButton {label} />
    </form>
  </div>
</div>

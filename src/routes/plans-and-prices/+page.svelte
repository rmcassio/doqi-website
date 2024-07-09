<script>
  import ElevatedButton from "../../components/ElevatedButton.svelte";
</script>

<div
  class="min-h-screen flex flex-col items-center justify-center bg-white p-4 py-20"
>
  <div class="text-center">
    <h1 class="text-4xl font-bold text-gray-800 mb-2">
      Cresça seu negócio com o <span class="text-red-500"
        >melhor investimento!</span
      >
    </h1>
    <p class="text-lg text-gray-600 mb-6">
      Teste 30 dias grátis sem informar dados de pagamento.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-4 gap-6 w-full max-w-6xl">
    <!-- Plan 1: Cobalto -->
    <div class="bg-white p-6 rounded-lg shadow-md">
      <h2 class="text-2xl font-bold text-gray-800 mb-2">Cobalto</h2>
      <p class="text-gray-600 mb-4">
        Integre com marketplaces, e-commerce e logística
      </p>
      <div class="text-3xl font-bold text-gray-800 mb-4">R$ 55/mês</div>
      <ElevatedButton width="w-full" label="Comece grátis" />
      <h3 class="text-lg font-semibold text-gray-700 mb-2">
        Recursos ilimitados
      </h3>
      <ul class="list-disc list-inside text-gray-600">
        <li>
          Integrações com +250 e-commerces, marketplaces e operadores logísticos
        </li>
        <li>Sincronização de estoque</li>
        <li>Atualização automática de pedidos</li>
      </ul>
    </div>

    <!-- Plan 2: Mercúrio -->
    <div class="bg-red-100 p-6 rounded-lg shadow-md relative">
      <div
        class="absolute top-2 right-2 bg-red-500 text-white text-sm px-2 py-1 rounded-full"
      >
        Popular
      </div>
      <h2 class="text-2xl font-bold text-gray-800 mb-2">Mercúrio</h2>
      <p class="text-gray-600 mb-4">
        O melhor custo benefício para simplificar suas vendas
      </p>
      <div class="text-3xl font-bold text-gray-800 mb-4">R$ 100/mês</div>
      <ElevatedButton width="w-full" label="Comece grátis" />
      <h3 class="text-lg font-semibold text-gray-700 mb-2">
        Recursos ilimitados
      </h3>
      <ul class="list-disc list-inside text-gray-600">
        <li>
          Integrações com +250 e-commerces, marketplaces e operadores logísticos
        </li>
        <li>Sincronização de estoque</li>
        <li>Atualização automática de pedidos</li>
      </ul>
    </div>

    <!-- Plan 3: Titânio -->
    <div class="bg-white p-6 rounded-lg shadow-md">
      <h2 class="text-2xl font-bold text-gray-800 mb-2">Titânio</h2>
      <p class="text-gray-600 mb-4">
        Para negócios que exigem alta organização na operação
      </p>
      <div class="text-3xl font-bold text-gray-800 mb-4">R$ 150/mês</div>
      <ElevatedButton width="w-full" label="Comece grátis" />
      <h3 class="text-lg font-semibold text-gray-700 mb-2">
        Recursos ilimitados
      </h3>
      <ul class="list-disc list-inside text-gray-600">
        <li>
          Integrações com +250 e-commerces, marketplaces e operadores logísticos
        </li>
        <li>Sincronização de estoque</li>
        <li>Atualização automática de pedidos</li>
      </ul>
    </div>

    <!-- Plan 4: Platina -->
    <div class="bg-white p-6 rounded-lg shadow-md">
      <h2 class="text-2xl font-bold text-gray-800 mb-2">Platina</h2>
      <p class="text-gray-600 mb-4">
        O máximo de benefícios para o seu negócio!
      </p>
      <div class="text-3xl font-bold text-gray-800 mb-4">R$ 400/mês</div>
      <ElevatedButton width="w-full" label="Comece grátis" />
      <h3 class="text-lg font-semibold text-gray-700 mb-2">
        Recursos ilimitados
      </h3>
      <ul class="list-disc list-inside text-gray-600">
        <li>
          Integrações com +250 e-commerces, marketplaces e operadores logísticos
        </li>
        <li>Sincronização de estoque</li>
        <li>Atualização automática de pedidos</li>
      </ul>
    </div>
  </div>
</div>

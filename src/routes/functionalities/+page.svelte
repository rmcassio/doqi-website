<script>
  import FunctionalityCard from "../../components/FunctionalityCard.svelte";
</script>

<div
  class="min-h-screen flex flex-col items-center justify-center bg-gray-50 p-4 py-20"
>
  <div class="text-center mb-10">
    <h1 class="text-4xl font-bold text-gray-800 mb-2">
      Conheça tudo o que o Doqi oferece!
    </h1>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-8 w-full max-w-6xl">
    <!-- Item 1: Notas fiscais -->
    <FunctionalityCard
      title="Notas fiscais"
      description="Emita notas fiscais de forma descomplicada, e preencha o setup inicial     apenas uma vez."
    />

    <!-- Item 2: Integração E-commerce e Marketplace -->
    <FunctionalityCard
      title="Integração E-commerce e Marketplace"
      description="Integre a sua loja virtual às principais plataformas e marketplaces do
        mercado."
    />

    <!-- Item 3: Estoque -->
    <FunctionalityCard
      title="Estoque"
      description="Cadastre, controle e organize as informações e os produtos do seu
        estoque."
    />

    <!-- Item 5: Link de Pagamento -->
    <FunctionalityCard
      title="Link de Pagamento"
      description="Receba pagamentos com Boleto, Pix ou cartão de crédito sem precisar de
        maquininha."
    />

    <!-- Item 8: Vendas -->
    <FunctionalityCard
      title="Vendas"
      description="Gerencie suas vendas, comissionamentos e envio de orçamentos, e venda
        mais com o Bling."
    />

    <!-- Item 9: Frente de Caixa -->
    <FunctionalityCard
      title="Frente de Caixa"
      description="Controle a movimentação do caixa, tanto da loja física quanto virtual,
        registrando suas vendas."
    />
  </div>
</div>

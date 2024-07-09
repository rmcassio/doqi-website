<script lang="ts">
  interface FAQItem {
    question: string;
    answer: string;
  }

  let faqItems: FAQItem[] = [
    {
      question:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque eleifend ante dolor?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question:
        "Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question: "Est qui dolorem ipsum quia dolor sit amet, consectetur?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question: "Lorem ipsum dolor sit amet, consectetur adipiscing?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question: "Dolor sit amet, consectetur adipiscing?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque eleifend ante dolor?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question:
        "Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question: "Est qui dolorem ipsum quia dolor sit amet, consectetur?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question: "Lorem ipsum dolor sit amet, consectetur adipiscing?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
    {
      question: "Dolor sit amet, consectetur adipiscing?",
      answer:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nibh nibh, ullamcorper at augue ut, rutrum mattis tortor. Proin aliquam erat turpis, ac laoreet erat molestie et. Ut malesuada lectus in justo tempor pharetra. Vestibulum lacinia sapien ac pharetra blandit. Integer sodales nibh sapien, vel auctor ipsum congue at. Nullam non tristique neque. Aenean vestibulum non felis vitae placerat. Cras quis ante accumsan, semper mi et, tempor massa. Quisque malesuada dolor non iaculis ornare. Ut ante neque, porta congue magna quis, bibendum gravida diam. Fusce vel fringilla ante. Vivamus molestie sagittis lectus, non commodo velit convallis eu. Integer dapibus turpis a lorem blandit, a finibus felis imperdiet.",
    },
  ];

  let activeIndex: number | null = null;

  function toggleAnswer(index: number) {
    activeIndex = activeIndex === index ? null : index;

    faqItems = faqItems.map((item, i) => (i === index ? { ...item } : item));
  }
</script>

<div class="bg-red-500 p-4">
  <h2 class="text-white text-2xl font-semibold mb-4">Perguntas frequentes</h2>
  <div class="grid grid-cols-2 gap-1">
    {#each faqItems as item, index}
      <div class="collapse collapse-arrow">
        <input
          type="checkbox"
          checked={activeIndex === index}
          on:change={() => toggleAnswer(index)}
          class="hidden"
          id={`faq-${index}`}
        />
        <label class="collapse-title text-left text-white" for={`faq-${index}`}>
          {item.question}
        </label>
        {#if activeIndex === index}
          <div class="collapse-content">
            <p class="text-gray-200">{item.answer}</p>
          </div>
        {/if}
      </div>
    {/each}
  </div>
</div>

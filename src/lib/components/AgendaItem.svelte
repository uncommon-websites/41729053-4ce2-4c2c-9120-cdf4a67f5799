<script lang="ts">
  interface AgendaItemType {
    time: string;
    title?: string;
    subtitle?: string;
    content?: string[];
  }

  export let date = "Week 1";
  export let items: AgendaItemType[] = [
    { time: "All day", title: "Pre-conference training (add-on)", subtitle: "Partner Summit (for Stripe partners only)" }
  ];
  export let tags: string[] = [];
  export let isFirst: boolean = false;
</script>

<div class="grid grid-cols-1 lg:grid-cols-12 gap-12 py-12 border-t border-[#333333]">
  <!-- Left Header (only show on first item) -->
  <div class="lg:col-span-5">
    {#if isFirst}
      <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-8 text-[#FCFCFC]">Your journey to connection</h2>
      <p class="text-base text-[#ABABAB] mb-8">
        From your first conversation with Mira to building lasting friendships, here's what to expect.
      </p>
    {/if}
  </div>

  <!-- Right Content -->
  <div class="lg:col-span-7">
    <div class="flex gap-2 mb-8">
      {#each tags as tag}
        <span class="inline-flex items-center gap-1.5 px-2 py-1 rounded bg-[#191919] text-[10px] font-medium text-[#ABABAB] uppercase tracking-wide border border-[#333333]">
          <span class="w-2 h-2 rounded-sm bg-[#3B51E1]"></span>
          {tag}
        </span>
      {/each}
    </div>

    <h3 class="text-3xl font-medium text-[#FCFCFC] mb-8">{date}</h3>

    <div class="space-y-0">
      {#each items as item}
        <div class="grid grid-cols-1 md:grid-cols-12 py-6 border-t border-[#333333]">
          <div class="md:col-span-3">
            <p class="text-sm text-[#919191] font-medium">{item.time}</p>
          </div>
          <div class="md:col-span-9">
             {#if Array.isArray(item.content)}
                <ul class="space-y-2">
                    {#each item.content as line}
                        <li class="text-sm text-[#ECECEC] flex items-start gap-2">
                          <span class="text-[#555555] mt-1">•</span>
                          <span>{line}</span>
                        </li>
                    {/each}
                </ul>
             {:else}
                <p class="text-sm text-[#FCFCFC] font-medium mb-1">{item.title}</p>
                {#if item.subtitle}
                    <p class="text-sm text-[#ABABAB]">{item.subtitle}</p>
                {/if}
             {/if}
          </div>
        </div>
      {/each}
    </div>
  </div>
</div>

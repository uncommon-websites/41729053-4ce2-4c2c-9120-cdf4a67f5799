<script lang="ts">
  import { Plus } from 'lucide-svelte';

  const faqs = [
    "Is Shiawase a dating app?",
    "How does the AI personality mapping work?",
    "What information does Mira collect during the video call?",
    "When will Shiawase be available at my university?",
    "Is Shiawase free for students?",
    "How do you maintain gender balance on the platform?",
    "What are micro-experiences and how do I join them?",
    "Can I host my own micro-experience?",
    "How is my data protected and used?",
    "What makes Shiawase different from other social apps?",
    "How do I provide feedback to improve my matches?",
    "Can I invite my friends to join Shiawase?"
  ];
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200" id="faq">
  <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-4">
      <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium text-black">FAQs</h2>
    </div>

    <div class="lg:col-span-8">
      <div class="border-t border-gray-200">
        {#each faqs as question}
          <div class="py-5 border-b border-gray-200 flex justify-between items-center cursor-pointer group hover:bg-gray-50 transition-colors px-2 -mx-2 rounded-sm">
            <h3 class="text-sm font-medium text-black pr-8">{question}</h3>
            <div class="text-gray-400 group-hover:text-black transition-colors">
              <Plus size={16} />
            </div>
          </div>
        {/each}
      </div>
      <div class="mt-8">
        <p class="text-sm text-gray-600">
          Have more questions? Email us at <a href="mailto:hello@shiawase.app" class="text-black underline hover:no-underline">hello@shiawase.app</a>
        </p>
      </div>
    </div>
  </div>
</section>

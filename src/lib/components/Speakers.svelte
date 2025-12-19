<script lang="ts">
  const founders = [
    { 
      name: 'Sonny Tai', 
      role: 'Co-Founder & CEO', 
      img: '/generated/image-asian-american-man-in-his-30s-confident--1766100153339-1.webp',
      bio: 'Sonny immigrated from Taiwan and experienced profound loneliness across cultures. His Marine Corps service taught him the power of deep bonds under pressure. He scaled Actuate from $1M to $6M ARR and raised over $22M.'
    },
    { 
      name: 'Otzar Jaffe', 
      role: 'Co-Founder & CTO', 
      img: '/generated/image-young-gen-z-male-in-early-20s-technical--1766100156260-2.webp',
      bio: 'Otzar joined Actuate at 15 after cold-emailing Sonny, showing early drive to connect. His Gen-Z perspective makes him uniquely attuned to his generation\'s isolation crisis. He shipped Shiawase\'s first version in just 6 hours.'
    }
  ];
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-[#333333] overflow-hidden" id="founders">
  <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-8 text-[#FCFCFC]">Meet the founders</h2>
  
  <p class="text-xl text-[#ABABAB] mb-16 max-w-3xl">
    Built by founders who deeply understand loneliness—one who experienced it across cultures and continents, another who grew up in the heart of Gen-Z's isolation crisis.
  </p>

  <!-- Founders Grid -->
  <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-20">
    {#each founders as founder}
      <div class="bg-[#191919] rounded-xl overflow-hidden border border-[#333333] group hover:border-[#3B51E1] transition-colors">
        <!-- Image -->
        <div class="relative h-[400px] bg-[#191919] overflow-hidden">
          <img 
            src={founder.img} 
            alt={founder.name} 
            class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" 
          />
        </div>

        <!-- Content -->
        <div class="p-8">
          <h3 class="text-2xl font-semibold text-[#FCFCFC] mb-1">{founder.name}</h3>
          <p class="text-sm font-medium text-[#919191] mb-4 uppercase tracking-wide">{founder.role}</p>
          <p class="text-sm leading-relaxed text-[#ABABAB]">
            {founder.bio}
          </p>
        </div>
      </div>
    {/each}
  </div>

  <!-- Mission Statement -->
  <div class="bg-[#191919] rounded-xl p-12 border border-[#333333]">
    <h3 class="text-3xl font-medium text-[#FCFCFC] mb-6">Our mission</h3>
    <p class="text-xl leading-relaxed text-[#ECECEC] mb-6">
      We're building Shiawase to solve one of the most pressing challenges facing our generation: the loneliness epidemic.
    </p>
    <p class="text-base leading-relaxed text-[#ABABAB]">
      Despite being the most "connected" generation, 80% of Gen-Z report feeling lonely. Dating apps have become over-monetized gambling mechanics. Social media has devolved into content farms optimized for ad revenue. AI companions offer parasocial substitutes that reinforce isolation rather than solve it.
    </p>
    <p class="text-base leading-relaxed text-[#ABABAB] mt-4">
      We believe AI should help humans connect with each other—not replace human connection. Shiawase uses AI to understand who you really are, then curates authentic introductions and experiences with people you'll genuinely click with. It's the magic of mutual friend introductions, at scale.
    </p>
  </div>

</section>

<style>
  .hide-scrollbar::-webkit-scrollbar {
    display: none;
  }
  .hide-scrollbar {
    -ms-overflow-style: none;
    scrollbar-width: none;
  }
</style>

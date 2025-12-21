<section class="pt-32 pb-20 px-6 max-w-[1400px] mx-auto">
  <style>
    @keyframes cycleTerms {
      0%, 22% { content: "ride or die"; }
      25%, 47% { content: "bff"; }
      50%, 72% { content: "loml"; }
      75%, 97% { content: "bae"; }
      100% { content: "ride or die"; }
    }
    
    .animated-term::before {
      content: "ride or die";
      animation: cycleTerms 8s infinite;
      display: inline-block;
      color: white;
      font-weight: 500;
      font-family: 'Courier New', Courier, monospace;
    }
  </style>
  <div class="mb-6">
    <span class="inline-block px-3 py-1 bg-gray-100 text-gray-700 text-xs font-medium rounded-full uppercase tracking-wide">
      Launching Fall 2026 at ASU
    </span>
  </div>

  <h1 class="text-[clamp(3rem,8vw,6.5rem)] leading-[0.95] tracking-tight font-medium max-w-5xl mb-12 text-white">
    Find your <span class="inline-block relative">
      <span class="animated-term bg-black px-3 py-1 rounded-md"></span>
    </span> people through AI-powered chemistry
  </h1>

  <div class="flex flex-col md:flex-row gap-8 md:gap-32 mb-16 text-sm font-medium text-gray-500">
    <div>
      <p class="text-gray-900 font-semibold mb-1">80% of Gen-Z</p>
      <p>feel lonely despite being</p>
      <p>the most "connected"</p>
    </div>
    <div>
      <p class="text-gray-900 font-semibold mb-1">Shiawase predicts</p>
      <p>genuine compatibility</p>
      <p>through personality mapping</p>
    </div>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-12 gap-8 mb-16">
    <div class="md:col-start-3 md:col-span-8 lg:col-start-4 lg:col-span-6">
      <p class="text-xl md:text-2xl leading-snug text-[#ECECEC] font-normal mb-8 text-center">
        Move beyond superficial swipes and content feeds. Shiawase uses AI to understand who you really are, then curates authentic connections and intimate experiences with people you'll genuinely click with.
      </p>
      <div class="flex flex-col sm:flex-row gap-4 justify-center">
        <a href="#join-waitlist" class="inline-block bg-[#3B51E1] text-white text-sm font-medium px-8 py-3 rounded-full hover:bg-[#4EA9EF] transition-colors text-center">
          Join the Waitlist
        </a>
        <a href="#how-it-works" class="inline-block bg-transparent text-[#FCFCFC] border border-[#555555] text-sm font-medium px-8 py-3 rounded-full hover:border-[#4EA9EF] hover:text-[#4EA9EF] transition-colors text-center">
          Learn More
        </a>
      </div>
    </div>
  </div>

  <!-- Hero Image -->
  <div class="w-full h-[400px] md:h-[500px] rounded-xl overflow-hidden border border-[#333333]">
    <img 
      src="/generated/image-two-gen-z-college-students-laughing-toge-1766100148868-0.webp" 
      alt="Students connecting authentically" 
      class="w-full h-full object-cover"
    />
  </div>
</section>

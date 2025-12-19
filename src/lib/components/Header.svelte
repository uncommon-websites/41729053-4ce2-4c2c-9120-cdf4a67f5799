<script lang="ts">
  let mobileMenuOpen = false;
</script>

<header class="fixed top-0 left-0 right-0 z-50 bg-[#101010]/90 backdrop-blur-sm border-b border-[#333333]">
  <div class="flex items-center justify-between px-6 py-4">
    <a href="/" class="flex items-center">
      <img src="/uploaded/1766114275287-l2f7rz6.png" alt="Shiawase" class="h-8" />
    </a>

    <div class="flex items-center gap-4">
      <nav class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-600">
        <a href="#how-it-works" class="hover:text-black transition-colors">How It Works</a>
        <a href="#founders" class="hover:text-black transition-colors">Our Story</a>
        <a href="#faq" class="hover:text-black transition-colors">FAQ</a>
      </nav>
      <a href="#join-waitlist" class="hidden sm:inline-block bg-black text-white text-sm font-medium px-5 py-2 rounded-full hover:bg-opacity-90 transition-opacity">
        Join Waitlist
      </a>
      <button 
        class="md:hidden p-2"
        on:click={() => mobileMenuOpen = !mobileMenuOpen}
        aria-label="Toggle menu"
      >
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          {#if mobileMenuOpen}
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
          {:else}
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
          {/if}
        </svg>
      </button>
    </div>
  </div>

  <!-- Mobile Menu -->
  {#if mobileMenuOpen}
    <div class="md:hidden border-t border-[#333333] bg-[#101010]">
      <nav class="flex flex-col px-6 py-4 space-y-4">
        <a href="#how-it-works" class="text-sm font-medium text-[#ABABAB] hover:text-[#4EA9EF] transition-colors" on:click={() => mobileMenuOpen = false}>How It Works</a>
        <a href="#founders" class="text-sm font-medium text-[#ABABAB] hover:text-[#4EA9EF] transition-colors" on:click={() => mobileMenuOpen = false}>Our Story</a>
        <a href="#faq" class="text-sm font-medium text-[#ABABAB] hover:text-[#4EA9EF] transition-colors" on:click={() => mobileMenuOpen = false}>FAQ</a>
        <a href="#join-waitlist" class="bg-[#3B51E1] text-white text-sm font-medium px-5 py-2 rounded-full hover:bg-[#4EA9EF] transition-colors text-center" on:click={() => mobileMenuOpen = false}>
          Join Waitlist
        </a>
      </nav>
    </div>
  {/if}
</header>

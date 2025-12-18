<script lang="ts">
  let mobileMenuOpen = false;
</script>

<header class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm border-b border-gray-100">
  <div class="flex items-center justify-between px-6 py-4">
    <a href="/" class="flex items-center gap-3">
      <svg width="32" height="32" viewBox="0 0 97 97" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M96.8438 48.3333C96.8438 75.0271 75.3534 96.6667 48.8438 96.6667C25.3046 96.6667 5.72283 79.605 1.63005 57.0928C1.61771 57.0251 1.60551 56.9572 1.59346 56.8891C1.10084 54.1121 0.84375 51.2529 0.84375 48.3333C0.84375 46.0025 1.00762 43.71 1.32439 41.4671C4.31845 20.2681 20.9721 3.49883 42.0249 0.483986C42.0602 0.478911 42.0954 0.473908 42.131 0.468905C44.3246 0.159814 46.5657 0 48.8438 0C51.8142 0 54.7216 0.271706 57.5428 0.791773C79.8997 4.91296 96.8438 24.6307 96.8438 48.3333ZM84.8438 48.3333C84.8438 68.3537 68.7261 84.5833 48.8438 84.5833C33.861 84.5833 21.0159 75.3669 15.5951 62.257C17.8219 62.6361 20.1099 62.8333 22.4438 62.8333C44.9769 62.8333 63.2438 44.4396 63.2438 21.75C63.2438 19.4 63.0479 17.096 62.6714 14.8538C75.6909 20.3123 84.8438 33.2466 84.8438 48.3333ZM49.6077 12.0913C50.6673 15.1126 51.2438 18.3635 51.2438 21.75C51.2438 37.7662 38.3495 50.75 22.4438 50.75C19.0806 50.75 15.8521 50.1695 12.8517 49.1026C12.8464 48.8469 12.8438 48.5905 12.8438 48.3333C12.8438 28.3129 28.9614 12.0833 48.8438 12.0833C49.0991 12.0833 49.3538 12.086 49.6077 12.0913Z" fill="black"/>
      </svg>
      <span class="font-bold text-xl tracking-tight">Shiawase</span>
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
    <div class="md:hidden border-t border-gray-100 bg-white">
      <nav class="flex flex-col px-6 py-4 space-y-4">
        <a href="#how-it-works" class="text-sm font-medium text-gray-600 hover:text-black transition-colors" on:click={() => mobileMenuOpen = false}>How It Works</a>
        <a href="#founders" class="text-sm font-medium text-gray-600 hover:text-black transition-colors" on:click={() => mobileMenuOpen = false}>Our Story</a>
        <a href="#faq" class="text-sm font-medium text-gray-600 hover:text-black transition-colors" on:click={() => mobileMenuOpen = false}>FAQ</a>
        <a href="#join-waitlist" class="bg-black text-white text-sm font-medium px-5 py-2 rounded-full hover:bg-opacity-90 transition-opacity text-center" on:click={() => mobileMenuOpen = false}>
          Join Waitlist
        </a>
      </nav>
    </div>
  {/if}
</header>

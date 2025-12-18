<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200" id="join-waitlist">
  <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-8 text-black">Join the movement</h2>
  
  <p class="text-xl text-gray-600 mb-16 max-w-2xl">
    We're launching at Arizona State University this fall. Be among the first to experience AI-powered authentic connection.
  </p>

  <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
    <!-- Cards -->
    <div class="lg:col-span-8 grid grid-cols-1 md:grid-cols-2 gap-6">
      
      <!-- Card 1 -->
      <div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-200 flex flex-col h-full relative overflow-hidden group hover:shadow-lg transition-shadow">
        <div class="flex justify-between items-start mb-6">
          <h3 class="text-lg font-semibold text-gray-900">ASU Students</h3>
          <span class="bg-black text-white text-[10px] uppercase tracking-wider font-semibold px-2 py-1 rounded">Priority Access</span>
        </div>
        
        <div class="flex items-baseline gap-2 mb-8">
          <span class="text-4xl font-medium text-black">Free</span>
        </div>

        <p class="text-sm text-gray-600 mb-8 flex-grow">
          Arizona State University students get priority access to the beta launch. Skip the waitlist and be part of building the future of connection.
        </p>

        <div class="mt-auto">
          <p class="text-xs text-gray-500 mb-4">Launching Fall 2026 at ASU campus</p>
          <button class="w-full bg-black text-white py-3 rounded-full text-sm font-medium hover:bg-opacity-90 transition-opacity">
            Join as ASU Student
          </button>
        </div>
      </div>

      <!-- Card 2 -->
      <div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-200 flex flex-col h-full relative overflow-hidden group hover:shadow-lg transition-shadow">
        <div class="flex justify-between items-start mb-6">
          <h3 class="text-lg font-semibold text-gray-900">Other Students</h3>
          <span class="bg-gray-100 text-gray-600 text-[10px] uppercase tracking-wider font-semibold px-2 py-1 rounded">Waitlist</span>
        </div>
        
        <div class="flex items-baseline gap-2 mb-8">
          <span class="text-4xl font-medium text-black">Free</span>
        </div>

        <p class="text-sm text-gray-600 mb-8 flex-grow">
          Join the waitlist to get early access when we expand to your campus. We're planning to reach the top 50 universities by 2027.
        </p>

        <div class="mt-auto">
          <p class="text-xs text-gray-500 mb-4">Expanding to more campuses in 2027</p>
          <button class="w-full bg-black text-white py-3 rounded-full text-sm font-medium hover:bg-opacity-90 transition-opacity">
            Join Waitlist
          </button>
        </div>
      </div>

    </div>

    <!-- Info List -->
    <div class="lg:col-span-4 pl-0 lg:pl-12 pt-4">
      <h3 class="text-sm font-semibold text-black mb-6 uppercase tracking-wide">Why Join Now</h3>
      <ul class="space-y-4">
        {#each [
          'Shape the product with your feedback',
          'Get lifetime premium features',
          'Join a founding community',
          'Priority matching with early adopters',
          'Exclusive campus events',
          'Direct access to founders'
        ] as item}
          <li class="text-sm text-gray-600 flex items-start gap-3">
            <svg class="w-5 h-5 text-black mt-0.5 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
            </svg>
            {item}
          </li>
        {/each}
      </ul>
    </div>
  </div>
</section>

<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-12">
  <div class="px-4 md:px-12 flex flex-col md:flex-row items-center justify-between gap-8">
    <!-- Logos -->
    <div class="flex flex-wrap items-center gap-8 md:gap-12 grayscale opacity-70">
        <!-- Lockheed Martin -->
        <div class="h-6 font-bold text-base tracking-tight uppercase">Lockheed Martin</div>
        <!-- Raytheon -->
        <div class="h-6 font-bold text-base tracking-wide uppercase">Raytheon</div>
        <!-- Northrop Grumman -->
        <div class="h-6 font-bold text-base tracking-tight uppercase">Northrop Grumman</div>
        <!-- BAE Systems -->
        <div class="h-6 font-bold text-base tracking-wide uppercase">BAE Systems</div>
    </div>

    <!-- Trust Text -->
    <div class="text-gray-400 text-sm font-light text-right md:text-left">
      Trusted by defense contractors worldwide
    </div>
  </div>
</SectionWrapper>

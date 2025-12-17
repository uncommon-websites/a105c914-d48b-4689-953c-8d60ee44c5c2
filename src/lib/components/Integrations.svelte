<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-24">
  <div class="px-4 md:px-12 max-w-4xl mx-auto text-center mb-16">
    <div class="text-xs font-mono uppercase tracking-widest text-gray-500 mb-4">
      Protocol Support
    </div>
    <h2 class="font-serif text-4xl text-gray-900 mb-6">
      Works with your existing infrastructure
    </h2>
    <p class="text-gray-500 leading-relaxed max-w-2xl mx-auto">
      Native support for industrial protocols including Modbus, OPC, EtherNet/IP, and Profinet. Trout integrates seamlessly with PLCs, SCADA systems, and legacy controllers without protocol conversion.
    </p>
  </div>

  <div class="px-4 md:px-12 relative">
    <!-- Connecting Line -->
    <div class="absolute top-1/2 left-0 w-full h-px bg-gray-200 -translate-y-1/2 hidden md:block"></div>

    <!-- Logos Row -->
    <div class="flex flex-wrap md:flex-nowrap items-center justify-center md:justify-between gap-8 relative z-10">
      
      <!-- Logo 1 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-gray-700">Modbus</div>
      </div>

       <!-- Logo 2 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-gray-700">OPC-UA</div>
      </div>

       <!-- Center Logo (Trout) -->
      <div class="w-24 h-24 bg-gray-900 rounded-full shadow-lg border-4 border-white flex items-center justify-center p-2 relative">
        <div class="text-white font-bold text-xs tracking-wider">TROUT</div>
        <!-- Orbit ring visual -->
        <div class="absolute inset-0 rounded-full border border-gray-700 scale-110 opacity-50"></div>
      </div>

       <!-- Logo 3 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-gray-700">Profinet</div>
      </div>

       <!-- Logo 4 -->
      <div class="w-16 h-16 bg-white rounded-full shadow-sm border border-gray-100 flex items-center justify-center p-3">
        <div class="text-[10px] font-bold text-gray-700">EtherNet/IP</div>
      </div>

    </div>
  </div>
</SectionWrapper>

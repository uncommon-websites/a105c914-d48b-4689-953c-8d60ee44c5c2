<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
  import SolutionBlock from './SolutionBlock.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="">
  <div class="px-4 md:px-12">
    <div class="py-16 text-center">
      <h2 class="font-serif text-4xl text-gray-900">How Trout secures your network</h2>
    </div>

    <!-- Block 1 -->
    <SolutionBlock
      label="Overlay Architecture"
      title="Deploy without rewiring"
      description="Software-defined network overlay sits on top of your existing infrastructure. No physical changes to legacy systems, no agent installation on endpoints, and zero disruption to ongoing operations. Deploy in hours across distributed sites."
    >
      <!-- Visual for Block 1: Network Nodes -->
      <div class="relative w-full h-full flex items-center justify-center">
        <!-- Central Hub -->
        <div class="w-16 h-16 bg-white shadow-lg rounded-lg flex items-center justify-center z-10 border border-gray-100">
           <div class="w-8 h-8 bg-[var(--color-primary-600)] rounded-sm"></div>
        </div>
        
        <!-- Connected Nodes -->
        <div class="absolute top-1/4 left-1/4 bg-white p-3 shadow rounded border border-gray-100 animate-pulse">
            <div class="w-8 h-10 bg-gray-700 rounded flex items-center justify-center text-[10px] font-bold text-white">PLC</div>
            <div class="mt-1 text-[10px] text-center">Controller</div>
        </div>
        <div class="absolute top-1/4 right-1/4 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-800 rounded flex items-center justify-center text-[10px] font-bold text-white">HMI</div>
            <div class="mt-1 text-[10px] text-center">Interface</div>
        </div>
        <div class="absolute bottom-1/4 left-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-600 rounded flex items-center justify-center text-[10px] font-bold text-white">SCADA</div>
            <div class="mt-1 text-[10px] text-center">System</div>
        </div>
         <div class="absolute bottom-1/4 right-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-500 rounded flex items-center justify-center text-[10px] font-bold text-white">RTU</div>
            <div class="mt-1 text-[10px] text-center">Remote</div>
        </div>
        
        <!-- Connecting Lines (Simplified) -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none opacity-20" viewBox="0 0 400 300">
            <path d="M100 100 L200 150 M300 100 L200 150 M150 220 L200 150 M250 220 L200 150" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4" />
        </svg>
      </div>
    </SolutionBlock>

    <!-- Block 2 -->
    <SolutionBlock
      label="Zero-Trust Security"
      title="Verify every connection"
      description="Microsegmentation and identity-based access control for every device and user. Continuous authentication ensures only authorized communications occur, preventing lateral movement and containing threats before they spread across your industrial network."
      reversed={true}
    >
      <!-- Visual for Block 2: Security Dashboard -->
      <div class="bg-white rounded-lg shadow-xl p-6 w-3/4 max-w-sm border border-gray-100">
        <div class="flex items-center space-x-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-green-500 flex items-center justify-center">
                <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"></path></svg>
            </div>
            <div class="text-xs text-gray-500">Site 7 • Manufacturing Floor</div>
        </div>
        <h4 class="font-serif text-xl mb-4">Network Status</h4>
        <div class="space-y-2 mb-6">
            <div class="flex items-center justify-between text-xs">
                <span class="text-gray-600">Authenticated Devices</span>
                <span class="font-bold text-green-600">127/127</span>
            </div>
            <div class="h-2 bg-green-100 rounded w-full"></div>
            <div class="flex items-center justify-between text-xs">
                <span class="text-gray-600">Threat Level</span>
                <span class="font-bold text-green-600">Secure</span>
            </div>
            <div class="h-2 bg-green-100 rounded w-2/6"></div>
        </div>
        <button class="w-full bg-gray-900 text-white py-2 rounded text-sm font-medium flex items-center justify-center space-x-2">
            <span>View Security Logs</span>
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
        </button>
      </div>
    </SolutionBlock>

    <!-- Block 3 -->
    <SolutionBlock
      label="Legacy System Compatible"
      title="Protect what you can't replace"
      description="Works with decades-old industrial equipment that can't support modern security agents. Brownfield-friendly deployment means your critical legacy systems get enterprise-grade protection without modification, replacement, or operational risk."
    >
       <!-- Visual for Block 3: Compatibility -->
       <div class="bg-white rounded shadow-lg p-8 w-2/3 max-w-xs border border-gray-100 relative">
          <div class="flex justify-between items-center mb-6 border-b pb-2">
              <div class="font-bold text-xs">Legacy Systems</div>
              <div class="w-4 h-4 bg-green-500 rounded-full"></div>
          </div>
          <div class="mb-4">
              <h5 class="font-bold text-sm">Protected Assets</h5>
              <div class="text-[10px] text-gray-400">Secured by Trout overlay network</div>
          </div>
          <div class="space-y-3 text-[10px] text-gray-600 leading-relaxed">
              <div class="flex items-center gap-2">
                  <div class="w-2 h-2 bg-green-500 rounded-full"></div>
                  <span>Allen-Bradley PLC (1998)</span>
              </div>
              <div class="flex items-center gap-2">
                  <div class="w-2 h-2 bg-green-500 rounded-full"></div>
                  <span>Siemens S7-300 Controller</span>
              </div>
              <div class="flex items-center gap-2">
                  <div class="w-2 h-2 bg-green-500 rounded-full"></div>
                  <span>Modbus RTU Network</span>
              </div>
              <div class="flex items-center gap-2">
                  <div class="w-2 h-2 bg-green-500 rounded-full"></div>
                  <span>Wonderware HMI System</span>
              </div>
          </div>
       </div>
    </SolutionBlock>
  </div>
</SectionWrapper>

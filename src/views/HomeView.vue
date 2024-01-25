<template>
  <div class="flex min-h-screen bg-gray-100">
    <!-- Sidebar -->
    <aside class="min-h-screen bg-white text-black p-4 w-[5rem] items-center space-y-10">
      <!-- Logo here -->
      <div class="flex justify-center items-center cursor-pointer">
        <img class="rounded-full" src="data:image/jpeg;base64,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">
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50  rounded-md mt-8 hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-home-3-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50  rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-mail-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50 rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-chat-2-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50  rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-bar-chart-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50  rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-settings-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="relative flex justify-center items-center text-gray-400 bg-gray-50 rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-hand-coin-line text-xl font-medium mt-2 mb-2"></i>
      </div>
    </aside>
       <!-- Main Content -->
       <main class="flex-1">
      <!-- Topbar -->
      <header class="border-l w-full h-[4rem] text-gray-500 bg-white p-4 shadow">
        <div class="flex justify-end space-x-5">
          <i class="ri-mail-line text-xl font-medium pt-1.5 cursor-pointer hover:text-[#13262d]"></i>
          <i class="ri-notification-3-line text-xl font-medium relative pt-1.5 cursor-pointer hover:text-[#13262d]">
            <span class="bg-red-700 text-white rounded-full w-4 h-4 text-xs flex items-center justify-center absolute top-0 right-0 -mr-1"> 1 </span>
          </i>
          <img src="../assets/papa.png" class="w-10 h-10 rounded-full border cursor-pointer">
        </div>
      </header>

      <!-- Main content here -->
      <div class="flex flex-col mx-0 bg-gray-200 h-screen w-[18rem]">
        <!-- Your main content goes here -->
        <div class="flex pt-8 ml-5 relative">
  <input class="border border-gray-300 rounded text-sm h-12 w-[16rem] pl-4 pr-12 outline-none text-gray-600 bg-gray-100"  type="text" placeholder="Cherher une conversation">
  <div class="absolute inset-y-0 right-0 flex items-center pr-3">
    <i class="ri-search-line text-gray-400 pt-8 mr-2 text-xl"></i>
  </div>
</div>
        
        <div
          class="flex flex-col border-l-2 border-green-600 ml-5 mt-5"
        >
           <h1 class="ml-2 font-medium italic">Visitor</h1>
           <p class="ml-2 font-normal"> J'i fait une transaction WAVE</p>
           <h1 class="ml-2 font-medium italic">Plateforme : <span class="text-green-500">SMS</span></h1>
        </div>
      </div>
    </main>
   
  </div>
 
</template>
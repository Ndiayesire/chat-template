<template>
  <div class="flex min-h-screen bg-gray-100">
    <!-- Sidebar -->
    <aside class="min-h-screen bg-white text-black p-4 w-[5rem] items-center space-y-10">
      <!-- Logo here -->
      <div class="flex justify-center items-center cursor-pointer">
        <img class="rounded-full" src="../assets/logo.jpg" />
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50 rounded-md mt-8 hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-home-2-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50 rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-mail-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50 rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-chat-2-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50 rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-bar-chart-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="flex justify-center items-center text-gray-400 bg-gray-50 rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-settings-line text-xl font-medium mt-2 mb-2"></i>
      </div>
      <div class="relative flex justify-center items-center text-gray-400 bg-gray-50 rounded-md hover:bg-[#13262d] hover:text-[#83f4be] cursor-pointer shadow-sm">
        <i class="ri-hand-coin-line text-xl font-medium mt-2 mb-2"></i>
      </div>
    </aside>

    <!-- Main Content -->
    <main class="flex-1">
      <!-- Topbar -->
      <header class="w-full h-[4rem] text-gray-500 bg-white p-4 shadow border-b">
        <div class="flex justify-end space-x-5">
          <i class="ri-mail-line text-xl font-medium pt-1.5 cursor-pointer hover:text-[#13262d] text-[#13262d]"></i>
          <i class="ri-notification-3-line text-xl font-medium relative pt-1.5 cursor-pointer hover:text-[#13262d] text-[#13262d]">
            <span class="bg-red-800 text-white rounded-full w-4 h-4 text-xs flex items-center justify-center absolute top-0 right-0 -mr-1">
              1
            </span>
          </i>
          <img src="../assets/papa.png" class="w-10 h-10 rounded-full border cursor-pointer" />
        </div>
      </header>

      <!-- Main content here -->
      <div class="flex min-h-screen bg-gray-100">
        <!-- Discussion list (left side) -->
        <div class="flex flex-col md:w-[20rem] border-r border-gray-300">
          <!-- Your main content goes here -->
          <div class="flex pt-2 ml-3 mr-3 relative">
            <input class="border border-gray-300 rounded text-sm h-12 w-full md:w-[17rem] pl-4 pr-12 outline-none text-gray-600 bg-white" type="text" placeholder="Chercher une conversation" />
            <div class="absolute inset-y-0 right-0 flex items-center pr-3">
              <i class="ri-search-line text-gray-400 pt-2 text-xl"></i>
            </div>
          </div>

          <!-- Discussion list content -->
          <div class="flex flex-col mt-5 mx-2 md:ml-3">
            <div class="flex flex-col border-l-2 border-green-600 hover:bg-green-50 cursor-pointer hover:border-r-2 hover:border-r-green-300 mb-5 bg-white rounded">
              <h1 class="ml-2 font-medium italic">Visitor</h1>
              <p class="ml-2 font-normal">J'ai fait une transaction WAVE</p>
              <h1 class="ml-2 font-medium italic">Plateforme : <span class="text-green-500">SMS</span></h1>
            </div>
            <div class="flex flex-col border-l-2 border-green-600 hover:bg-green-50 cursor-pointer hover:border-r-2 hover:border-r-green-300 mb-5 bg-white rounded">
              <h1 class="ml-2 font-medium italic">Visitor</h1>
              <p class="ml-2 font-normal">I want some informations</p>
              <h1 class="ml-2 font-medium italic">Plateforme : <span class="text-green-500">SMS</span></h1>
            </div>
            <div class="flex flex-col border-l-2 border-green-600 hover:bg-green-50 cursor-pointer hover:border-r-2 hover:border-r-green-300 mb-5 bg-white rounded">
              <h1 class="ml-2 font-medium italic">Visitor</h1>
              <p class="ml-2 font-normal">Je veux modifier mon code</p>
              <h1 class="ml-2 font-medium italic">Plateforme : <span class="text-yellow-500">WEB</span></h1>
            </div>
          </div>
        </div>

        <!-- Chat box section (right side) -->
        <div class="flex flex-col justify-start">
          <div class="bg-white p-4 md:h-[4rem] md:border-b md:border-r sm:w-full">
            <div class="flex justify-start">
              <div class="flex bg-[#13262d] justify-center items-center h-10 w-10 rounded-full">
                <h1 class="font-medium text-center text-[#83f4be]">N</h1>
              </div>
              <h1 class="ml-2 text-center text-medium font-semibold text-[#13262d] pt-2 md:text-left">+221 778673184</h1>
            </div>
          </div>

          <!-- Messages -->
          <div class="flex flex-col bg-gray-50 md:w-[55rem] border-r overflow-y-auto">
            <!-- Sender's message -->
            <div class="flex justify-end mb-2 pt-5 mr-3">
              <div class="max-w-[80%]">
                <div class="bg-[#13262d] text-[#83f4be] rounded-lg p-2">
                  <p class="text-sm text-white">Hello! How can I help you?</p>
                </div>
              </div>
            </div>

            <!-- Receiver's message -->
            <div class="flex justify-start mb-2 ml-3">
              <div class="max-w-[80%]">
                <div class="bg-white border border-gray-300 rounded-lg p-2">
                  <p class="text-sm text-[#13262d]">Hi there! I have a question about my account.</p>
                </div>
              </div>
            </div>

            <!-- Sender's message -->
            <div class="flex justify-end mb-2 pt-5 mr-3">
              <div class="max-w-[80%]">
                <div class="bg-[#13262d] text-[#83f4be] rounded-lg p-2">
                  <p class="text-sm text-white">Hello! How can I help you?</p>
                </div>
              </div>
            </div>

            <!-- Receiver's message -->
            <div class="flex justify-start mb-2 ml-3">
              <div class="max-w-[80%]">
                <div class="bg-white border border-gray-300 rounded-lg p-2">
                  <p class="text-sm text-[#13262d]">Hi there! I have a question about my account.</p>
                </div>
              </div>
            </div>

            <!-- Sender's message -->
            <div class="flex justify-end mb-2 pt-5 mr-3">
              <div class="max-w-[80%]">
                <div class="bg-[#13262d] text-[#83f4be] rounded-lg p-2">
                  <p class="text-sm text-white">Hello! How can I help you?</p>
                </div>
              </div>
            </div>

            <!-- Receiver's message -->
            <div class="flex justify-start mb-2 ml-3">
              <div class="max-w-[80%]">
                <div class="bg-white border border-gray-300 rounded-lg p-2">
                  <p class="text-sm text-[#13262d]">Hi there! I have a question about my account.</p>
                </div>
              </div>
            </div>

            <!-- Sender's message -->
            <div class="flex justify-end mb-2 pt-5 mr-3">
              <div class="max-w-[80%]">
                <div class="bg-[#13262d] text-[#83f4be] rounded-lg p-2">
                  <p class="text-sm text-white">Hello! How can I help you?</p>
                </div>
              </div>
            </div>

            <!-- Receiver's message -->
            <div class="flex justify-start mb-2 ml-3">
              <div class="max-w-[80%]">
                <div class="bg-white border border-gray-300 rounded-lg p-2">
                  <p class="text-sm text-[#13262d]">Hi there! I have a question about my account.</p>
                </div>
              </div>
            </div>

            <!-- Sender's message -->
            <div class="flex justify-end mb-2 pt-5 mr-3">
              <div class="max-w-[80%]">
                <div class="bg-[#13262d] text-[#83f4be] rounded-lg p-2">
                  <p class="text-sm text-white">Hello! How can I help you?</p>
                </div>
              </div>
            </div>

            <!-- Receiver's message -->
            <div class="flex justify-start mb-2 ml-3">
              <div class="max-w-[80%]">
                <div class="bg-white border border-gray-300 rounded-lg p-2">
                  <p class="text-sm text-[#13262d]">Hi there! I have a question about my account.</p>
                </div>
              </div>
            </div>

            <!-- Sender's message -->
            <div class="flex justify-end mb-2 pt-5 mr-3">
              <div class="max-w-[80%]">
                <div class="bg-[#13262d] text-[#83f4be] rounded-lg p-2">
                  <p class="text-sm text-white">Hello! How can I help you?</p>
                </div>
              </div>
            </div>

            <div class="bg-white p-4 relative">
              <div class="flex items-center">
                <input class="border border-gray-300 rounded text-sm w-full pl-4 pr-12 h-12 outline-none text-gray-600 bg-white" type="text" placeholder="Ecrire un message..." />
                <i class="ri-send-plane-line text-xl text-gray-800 absolute inset-y-0 right-0 pr-3 pt-7 mr-3 hover:text-[#83f4be] cursor-pointer"></i>
              </div>
            </div>
          </div>
        </div>
        <!-- Tabs section -->
        <div class="flex flex-col w-full">
          <div class="flex justify-center space-x-11 bg-white w-full p-4 h-[4rem] border-b">
            <!-- Tab 1 -->
            <div @click="changeTab(0)" :class="{ 'border-b-2 border-[#0E6655]': activeTab === 0 }" class="cursor-pointer text-center hover:border-b-2 hover:border-[#83f4be] w-[2rem]">
              <i class="ri-user-line text-2xl text-[#13262d]"></i>
            </div>

            <!-- Tab 2 -->
            <div @click="changeTab(1)" :class="{ 'border-b-2 border-[#0E6655]': activeTab === 1 }" class="cursor-pointer text-center hover:border-b-2 hover:border-[#83f4be] w-[2rem]">
              <i class="ri-settings-3-line text-2xl text-[#13262d]"></i>
            </div>

            <!-- Tab 3 -->
            <div @click="changeTab(2)" :class="{ 'border-b-2 border-[#0E6655]': activeTab === 2 }" class="cursor-pointer text-center hover:border-b-2 hover:border-[#83f4be] w-[2rem]">
              <i class="ri-chat-3-line text-2xl text-[#13262d]"></i>
            </div>
          </div>

          <!-- Dynamic tab content -->
          <div class="bg-white min-h-screen justify-center flex pt-8 italic">
            <div v-if="activeTab === 0" class="tab-content text-black">Contenu Tab 1</div>
            <div v-if="activeTab === 1" class="tab-content">Contenu Tab 2</div>
            <div v-if="activeTab === 2" class="tab-content">Contenu Tab 3</div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
  import { ref } from "vue";

  export default {
    setup() {
      const activeTab = ref(0);

      const changeTab = (tabIndex) => {
        activeTab.value = tabIndex;
      };

      return {
        activeTab,
        changeTab,
      };
    },
  };
</script>

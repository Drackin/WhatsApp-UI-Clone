<template>
  <div class="w-[30%] h-[100vh] bg-[#131c21] list-none" id="talk-list">
    <div class="h-3/15 bg-[#d7a53b] flex items-center select-none">
      <span class="material-icons-outlined bg-[#ece2ce] md-24 rounded-full p-3 ml-5 text-[#d7a53b]">wifi_off</span>
      <div class="pl-4">
        <h1 class="text-lg">Device Unreachable</h1>
        <p class="w-3/4">Make sure your computer has an active internet connection.</p>
        <p class="text-sm">Don't Panic. This is Test</p>
      </div>
    </div>
    <div class="h-12 select-none" id="search-box">
      <div class="pb-2"></div>
      <div class="flex bg-[#323739] rounded-full h-8 w-[95%] items-center ml-3">
        <span class="material-icons md-light pl-3 pr-4">search</span>
        <input type="text" placeholder="Search or start new chat" class="pl-1 bg-[#323739] h-8 w-[80%] outline-none border-none text-white">
      </div>
    </div>
    <div id="chats">
      <li class="flex transition duration-200 h-18 text-white pt-3 pl-3 cursor-pointer select-none" id="talk-item" v-for="(talk, i) in talks" :key="i">
        <img :src="talk.user_icon" class="w-12 h-12 rounded-full select-none">
        <div class="ml-4">
          <p class="text-lg" :title="talk.username">{{ talk.username }}</p>
          <p class="text-sm text-gray-400"
            :title="talk.username == 'Drackin' ? 'github.com/Drackin (Please Follow)' : `Hey, There! I'm Using WhatsApp`">{{
            talk.username == "Drackin" ? "github.com/Drackin (Please Follow)": "Hey, There! I'm Using WhatsApp"
            }}</p>
        </div>
      </li>
    </div>
  </div>
</template>

<script>
export default {
    props: {
        talks: Array
    }
}
</script>

<style>

@import url("https://fonts.googleapis.com/icon?family=Material+Icons");
@import url("https://fonts.googleapis.com/icon?family=Material+Icons+Outlined");


#talk-item:hover {
  background: #2d3134;
}

#talk-item {
  border-bottom: 1px solid #555;
}

#search-box {
  border-bottom: 1px solid #555;
}

.material-icons.md-light { color: #9ca3af }

.material-icons-outlined.md-24 { font-size: 24px; }

</style>
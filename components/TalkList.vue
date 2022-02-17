<template>
  <div class="w-[30%] h-full bg-[#111b21] list-none" id="talk-list">
    <div class="h-14 select-none flex items-center" id="search-box">
      <div class="flex bg-[#202c33] rounded-lg h-10 w-[95%] items-center ml-3">
        <span class="material-icons md-light pl-3 pr-4">search</span>
        <input type="text" placeholder="Search or start new chat" class="pl-1 bg-[#202c33] h-10 w-[80%] outline-none border-none text-white">
      </div>
    </div>
    <div id="chats" class="overflow-y-auto">
      <li class="flex transition duration-200 h-20 text-white items-center pl-3 cursor-pointer select-none" id="talk-item" v-for="(talk, i) in talks" :key="i">
        <img :src="talk.user_icon" class="w-14 h-14 rounded-full select-none object-cover">
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
  background: #202C33;
}

#talk-item {
  border-bottom: 1px solid #222d34;
}

#search-box {
  border-bottom: 1px solid #222d34;
}

.material-icons.md-light { color: #9ca3af }

.material-icons-outlined.md-24 { font-size: 24px; }

</style>
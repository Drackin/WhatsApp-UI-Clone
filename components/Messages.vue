<template>
  <div class="h-full w-[70%] bg-dark-400" id="bg">
    <div class="h-[89%]"></div>
    <div class="bg-[#202c33] flex items-center h-[11%]">
      <button class="material-icons md-light md-24 ml-4 select-none outline-none border-none">insert_emoticon</button>
      <button class="material-icons md-light md-24 ml-4 select-none outline-none border-none">attachment</button>
      <input type="text" class="bg-[#2a3942] h-[70%] outline-none border-none select-none rounded-lg ml-3 pl-3 text-white w-[85%] text-lg" placeholder="Text A Message">
      <button class="material-icons md-light md-24 ml-3 select-none outline-none border-none md-24">mic</button>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

#bg {
    background-image: linear-gradient(to bottom, rgba(11, 20, 26, 0.9) 0%,rgba(11, 20, 26, 0.9) 100%), url("../assets/images/background.png");
    border-left: 1px solid #2f3b43;
}

.material-icons-outlined.md-light {
    color: #828689;
}

.material-icons-outlined.md-24 { font-size: 48px; }

#bg button {
    outline: none;
    border: none;
}

</style>
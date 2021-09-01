<template>
  <div class="h-[100vh] w-[70%] bg-dark-400" id="bg">
    <div class="h-[80%]"></div>
    <div class="bg-[#1e2428] flex items-center h-[10%]">
      <button class="material-icons md-light md-24 ml-4 select-none outline-none border-none">insert_emoticon</button>
      <button class="material-icons md-light md-24 ml-4 select-none outline-none border-none">attachment</button>
      <input type="text" class="bg-[#33383b] h-11 outline-none border-none select-none rounded-full ml-3 pl-3 text-white w-[85%]" placeholder="Text A Message">
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
    background-image: linear-gradient(to bottom, rgba(0,0,0,0.9) 0%,rgba(0,0,0,0.9) 100%), url("../assets/images/background.png");
    border-left: 1px solid #555;
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
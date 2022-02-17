<template>
  <div class="w-[30%] bg-[#202c33] h-full flex items-center select-none" id="user-navbar">
    <img src="https://avatars.githubusercontent.com/u/78258229?v=4" class="cursor-pointer w-[2.75rem] h-[2.75rem] rounded-full ml-4">
    <button class="material-icons md-light md-mid ml-53" title="Status">motion_photos_on</button>
    <button class="material-icons md-light md-mid ml-5" title="New chat">chat</button>
    <button class="material-icons md-light md-mid ml-5">more_vert</button>
  </div>
</template>

<script>
export default {

}
</script>

<style>

.material-icons.md-mid { font-size: 1.5rem; }

#user-navbar button {
    border: none;
    outline: none;
}

</style>
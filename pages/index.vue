<template>
  <div class="w-screen h-screen">
    <div class="flex w-full h-1/10">
      <UserNavbar />
      <Navbar />
    </div>
    <div class="flex w-full h-9/10">
      <TalkList :talks="talks"/>
      <Messages/>
    </div>
  </div>
</template>

<script>
import * as data from "../assets/data/talks.json"

export default {
  data() {
    return {
      talks: data.talking_users
    }
  }
}

</script>

<template>
  <div>
    <div class="flex">
      <UserNavbar />
      <Navbar />
    </div>
    <div class="flex">
      <TalkList :talks="talks" class="fixed"/>
      <Messages class="fixed ml-102.5"/>
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

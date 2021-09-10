<template>
  <div id="onlinefriends">
      <h2>Online Friends</h2>
      <div>
          <ul>
              <li v-for="(friend, index) in friends" :key="index">
                 <h5 v-if="friend.online">{{friend.name}}</h5>
              </li>
          </ul>
      </div>

  </div>
</template>

<script>
export default {
    name:'OnlineFriends',
    props:['friends'],
    data(){
        return{
            
        }
    }

}
</script>

<style>

</style>
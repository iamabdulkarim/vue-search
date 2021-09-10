<template>
  <div id="allfriends">
      <h2> ALL Friends</h2>
        <ul>
            <li v-for="(friend,index) in friends" :key="index"
            @click="unfriend(friend.name)">
                {{friend.name}}
            </li>
        </ul>
  </div>
</template>

<script>
export default {
    name:'AllFriends',
    props:['friends'],
    data(){
        return{
           
        }
    },
    methods:{
        unfriend(name){
            this.$emit('delete',{name})
        }
    }
}
</script>

<style>

</style>
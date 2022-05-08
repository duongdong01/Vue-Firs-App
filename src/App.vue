
<template>
<section>
  <header><h1>My Friends</h1></header>
  <ul>
    <friend-contact 
    v-for="friend in friends"
      :key="friend.id"
      :name ="friend.name" 
      :phone-number="friend.phone" 
      :email-address="friend.email"
      :is-favorite="friend.isFavorite"
      >
      </friend-contact>
  </ul>
</section>
</template>Manuel lorenz

<script>
export default {
  data(){
    return {
      friends:[
        {
          id:'Manuel',
          name:'Manuel Jum',
          phone : '026161662',
          email:'Manuel@localhost.com',
          isFavorite:true
        },
          {
          id:'Julie',
          name:'Julie Jones',
          phone : '026161662',
          email:'Julie@localhost.com',
          isFavorite:false
        }
      ]
    }
  }
}
</script>

<style>
section{
  @import url('https://fonts.googleapis.com/css2?family=Jost&display=swap' );
}
</style>
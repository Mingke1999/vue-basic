<template>
  <div> 
    <!--onyl one root element-->
    <h3>Condition</h3>
    <p v-if="display">displayed set true</p>
    <p v-else>displayed set false</p>

    <template v-if="display"> <!--template woun't be rendered-->
        <h3>Patricia Lockwood, "Rape Joke"</h3>
        <p>The rape joke is that you were 19 years old.</p>
        <p>The rape joke is that he was your boyfriend.</p>
        <p>The rape joke it wore a goatee. A goatee.</p>
    </template>
    <template v-else>
        <h3>The Anactoria Poem</h3>
        <p>Some say thronging cavalry, some say foot soldiers</p>
        <p>others call a fleet the most beautiful of sights the dark earth offers,</p>
        <p>but I say it's whatever you love best.</p>
    </template>

  </div>
</template>

<script>
export default {
    data(){
        return{
            display:false
        }
    }
}
</script>

<style>

</style>
<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  
  <main>
    
      <div class="star-div"><img src="./assets/icon-star.svg" alt="icon-star"></div>
      <h1>How did we do?</h1>
      <p>Please let us know how we did with your support request. All feedback is appreciated to help us improve our offering!</p>
      <div class="inputs-div">
        <input type="checkbox" name="1-star" id="">
        <label for="1-star">1</label>
        <input type="checkbox" name="2-star" id="">
        <label for="1-star">2</label>
        <input type="checkbox" name="3-star" id="">
        <label for="1-star">3</label>
        <input type="checkbox" name="4-star" id="">
        <label for="1-star">4</label>
        <input type="checkbox" name="5-star" id="">
        <label for="1-star">5</label>
      </div>
      <button>SUBMIT</button>
        
  </main>

</template>


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
        <input type="radio" name="rating" id="1-star" value="1">
        <label for="1-star">1</label>
        <input type="radio" name="rating" id="2-star" value="2">
        <label for="2-star">2</label>
        <input type="radio" name="rating" id="3-star" value="3">
        <label for="3-star">3</label>
        <input type="radio" name="rating" id="4-star" value="4">
        <label for="4-star">4</label>
        <input type="radio" name="rating" id="5-star" value="5">
        <label class="selected" for="5-star">5</label>
      </div>
      <button>SUBMIT</button>
        
  </main>

</template>


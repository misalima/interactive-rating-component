<script>
export default {
  name: 'RatingComponent',
  data() {
    return {
      isSelected: false,
      isRated: false,
      rating: 0
    }
  },
  methods: {
    
    submitRating() {
      if(!this.isSelected) {
        document.querySelector(".error").classList.add("visible");
        return;
      }
      this.isRated = true;
    }
  }
};
</script>

<template>
  
  <div v-if="!isRated">
      <div class="star-div"><img src="../assets/icon-star.svg" alt="icon-star"></div>
      <h1>How did we do?</h1>
      <p>Please let us know how we did with your support request. All feedback is appreciated to help us improve our
        offering!</p>
      <div class="inputs-div">
        <input @change="isSelected = true" type="radio" name="rating" id="1-star" value="1" v-model="rating">
        <label :class="{selected: rating === '1'}" for="1-star">1</label>
        <input @change="isSelected = true" type="radio" name="rating" id="2-star" value="2" v-model="rating">
        <label :class="{selected: rating === '2'}" for="2-star">2</label>
        <input @change="isSelected = true" type="radio" name="rating" id="3-star" value="3" v-model="rating">
        <label :class="{selected: rating === '3'}" for="3-star">3</label>
        <input @change="isSelected = true" type="radio" name="rating" id="4-star" value="4" v-model="rating">
        <label :class="{selected: rating === '4'}" for="4-star">4</label>
        <input @change="isSelected = true" type="radio" name="rating" id="5-star" value="5" v-model="rating">
        <label :class="{selected: rating === '5'}" for="5-star">5</label>
      </div>
      <button @click="submitRating">SUBMIT</button>
      <p class="error">Please select a number to submit.</p>
    </div>

    <div v-if="isRated" class="thank-you" >
      <img src="../assets/illustration-thank-you.svg" alt="thank-you">
      <p class="given-rating">You selected {{ rating }} out of 5</p>
      <h1>Thank you!</h1>
      <p>We appreciate you taking the time to give a rating. If you ever need more support, don’t hesitate to get in touch!</p>
    </div>
</template>


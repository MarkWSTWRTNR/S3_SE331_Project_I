<template>
  <ReviewForm @review-submited="addReview" />
  <ReviewList v-if="GStore.reviews" :reviews="GStore.reviews" />
</template>

<script>
import ReviewForm from "@/components/ReviewForm.vue"
import ReviewList from "@/components/ReviewList.vue"

export default{
  inject: ['GStore'],
  components: {ReviewForm, ReviewList},
  methods: {addReview(review){
            this.GStore.reviews.push(review)
        }
  }     
}
</script>
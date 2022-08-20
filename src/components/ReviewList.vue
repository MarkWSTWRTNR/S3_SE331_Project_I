<template>
    <div class="review-container">
        <h3>Reviews: </h3>
            <ul>
                <li v-for="(review, index) in reviews" :key="index">
                    {{ review.name }} gave this {{ review.rating }} stars
                    <br/>
                    "{{ review.review }}"
                    <br/>
                    Recomend form {{ review.name }} to do something better is {{ review.recommend }}
                    <br/>
                </li>
            </ul>
        </div>
</template>

<script>
export default{
    props: ['reviews']
}
</script>


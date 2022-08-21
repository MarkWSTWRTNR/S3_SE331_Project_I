<template>
    <div class="review-container">
        <h3>Doctor's Suggestion: </h3>
            <ul>
                <li v-for="(review, index) in reviews" :key="index">
                    Date: {{ review.date }}
                    <br/>
                    Patient Name: {{ review.name }}
                    <br/>
                    Dortor's Suggestion: "{{ review.suggestion }}"
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


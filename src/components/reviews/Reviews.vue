<template>
    <div class="catrus-reviews container-fit">
        <h1 class="catrus-reviews__title">59,393 Real Reviews (as of Jan 11, 2019)</h1>
        <h2 class="catrus-reviews__subtitle text-with-line">Below are the true reviews from people that already ordered from us:</h2>

        <div class="catrus-reviews__list">
            <div class="catrus-reviews__list-item" v-for="review in reviews" v-bind:key="review.id">
                <div class="catrus-reviews__list-item__rates">
                    <span>{{review.rating}}</span> / 10
                </div>

                <h2 class="catrus-reviews__list-item__title">{{review.title}}</h2>
                <h5 class="catrus-reviews__list-item__order">{{review.order}}</h5>
                <div class="catrus-reviews__list-item__desc">{{review.desc}}</div>
            </div>
        </div>

        <div class="catrus-reviews__more">
            <div class="catrus-reviews__more-actions">
                <button class="catrus-reviews__more-btn">show more reviews</button>
                <div class="catrus-reviews__more-current">376 of 59.393</div>
            </div>

            <img src="../../assets/reviews-bg.png" alt="">
        </div>
    </div>
</template>

<script>
    export default {
        data: () => ({
            action: false,
            el: null,
            reviews: [
                {
                    id: 1,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer  have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer  have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer  have pass on this writers code to other sohe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so thahe writer  have pass on this writers code to other so tha that they may enjoy good quality work. Awesome Job. The writer . Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 2,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 3,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 4,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 5,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 6,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 7,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 8,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 9,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 10,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                },
                {
                    id: 11,
                    title: 'writer 21321',
                    order: 'Order #324u 238423',
                    rating: 8,
                    desc: 'I have pass on this writers code to other so that they may enjoy good quality work. Awesome Job. The writer had lot of patience and was able to fulfil my demands.'
                }
            ]
        }),
        methods: {

        },
        mounted() {

        }
    }
</script>
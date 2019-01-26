<template>
    <div class="catrus-carousel container">
        <div class="container-fit">
            <div class="catrus-carousel__container">
                <div class="catrus-carousel__container-item"
                    v-for="item in carousel"
                    v-bind:key="item.id"
                    v-bind:class="{ 'catrus-carousel__container-item-active': activeSlide === item.id}"
                    v-if="item.id === activeSlide">
                    <div class="catrus-carousel__container-title">
                        {{item.title}}
                    </div>
                    <div class="catrus-carousel__container-subtitle">
                        {{item.subtitle}}
                    </div>
                    <ul class="catrus-carousel__container-list">
                        <li class="catrus-carousel__container-list__item"
                            v-bind:key="index"
                            v-for="(li, index) in item.list"
                        >{{li}}
                        </li>
                    </ul>
                </div>
                <div class="catrus-carousel__container-action">
                    <button class="catrus-carousel__container-action__btn">get instant price quote</button>
                </div>

                <ul class="catrus-carousel__container-dots">
                    <li class="catrus-carousel__container-dots__item"
                        v-for="dot in carousel"
                        v-bind:key="dot.id"
                        v-bind:class="{ 'catrus-carousel__container-dots__item-active': activeSlide === dot.id}"
                        @click="changeActiveSlide(dot.id)"
                    >
                    </li>
                </ul>
            </div>
        </div>
        <div class="catrus-carousel__mouse">
            Scroll for more...
        </div>
    </div>
</template>

<script>
    export default {
        data: () => ({
            activeSlide: null,
            interval: null,
            carousel: [
                {
                    id: 1,
                    title: 'Get Your Paper Writt',
                    subtitle: 'We know exactly what it takes to write an excellent essay in the shortest amount of time possible',
                    list: [
                        'Over 250 writers on the team',
                        'All subjects and citation styles',
                        'Open 24/7. No holidays, no weekends'
                    ]
                },
                {
                    id: 2,
                    title: 'Get Your Paper Writt',
                    subtitle: 'We know exactly what it takes to write an excellent essay in the shortest amount of time possible',
                    list: [
                        '22222222222222',
                        'All subjects and citation styles',
                        'Open 24/7. No holidays, no weekends'
                    ]
                },
                {
                    id: 3,
                    title: 'Get Your Paper Writt',
                    subtitle: 'We know exactly what it takes to write an excellent essay in the shortest amount of time possible',
                    list: [
                        '3333333333333333333333333',
                        'All subjects and citation styles',
                        'Open 24/7. No holidays, no weekends'
                    ]
                }
            ]
        }),
        methods: {
            initCarousel () {
                this.activeSlide = this.carousel[0].id
            },
            changeActiveSlide (id) {
                this.activeSlide = id
            },
            initAutoTrigger () {
                let vm = this

                function change() {
                    for (let i = 0; i < vm.carousel.length; i++) {
                        if (vm.carousel[i].id === vm.activeSlide) {
                            let currentState = i
                            currentState = vm.carousel[i] === vm.carousel[vm.carousel.length - 1] ? 0 : currentState + 1

                            vm.activeSlide = vm.carousel[currentState].id
                            return
                        }
                    }
                }

                setInterval(change, 5000)
            }
        },
        mounted() {
            this.initCarousel()
            this.initAutoTrigger()
        }
    }
</script>

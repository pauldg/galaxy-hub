<template>
    <div class="carousel-container">
        <b-carousel
            id="carousel-1"
            v-model="slide"
            :interval="4000"
            controls
            indicators
            background="#ababab"
            img-width="650"
            img-height="450"
            style="text-shadow: 1px 1px 2px #333"
        >
            <!--
            It's important that the images here are 13x9 aspect ratio,
            otherwise the page will jump around when the carousel changes.
            -->
            <a href="https://galaxyproject.org/events/gcc2023/register/" target="_blank">
                <b-carousel-slide
                    img-src="/images/events/gcc2023/gcc2023-registration-early-deadline.png"
                    img-alt="The Galaxy Community Conference is an annual gathering that brings together scientists, software developers, and trainers of Galaxy from a variety of disciplines to share their experiences, knowledge, and skills. Early registration closes Friday, May 12."
                ></b-carousel-slide>
            </a>
            <a href="https://gxy.io/smorgasbord3" target="_blank">
                <b-carousel-slide
                    img-src="/images/events/2023-05-smorgasbord3/smorgasbord3-square.png"
                    img-alt="The Galaxy Training Network Smörgåsbord 3 is a free global online Galaxy training event from May 22 to May 26, 2023"
                ></b-carousel-slide>
            </a>
            <a href="https://jxtxfoundation.org" target="_blank">
                <b-carousel-slide
                    img-src="/images/jxtx/jxtx-jumbotron.png"
                    img-alt="Donate to the James P. Taylor Foundation for Open Science"
                ></b-carousel-slide>
            </a>
        </b-carousel>
    </div>
</template>

<script>
export default {
    name: "Carousel",
    data() {
        return {
            slide: 0,
        };
    },
};
</script>
<style lang="scss" scoped>
.carousel-container {
    padding-top: 2rem;
    max-width: 650px;
    margin: 0 auto;
}
</style>

<template>
    <section class="bg-light" id="portfolio">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-center">
            <h2 class="section-heading text-uppercase">Our experiences</h2>
            <h3 class="section-subheading text-muted">Within our courses, we worked on many projects proving our skills.</h3>
          </div>
        </div>
        <div class="row">
          
            <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj, key) in portfolioJSON" :key="key">
                <a class="portfolio-link" data-toggle="modal" href="#portfolioModal2">
                    <div class="portfolio-hover">
                        <div class="portfolio-hover-content">
                            <i class="fas fa-plus fa-3x"></i>
                        </div>
                    </div>
                    <img class="img-fluid" src="img/portfolio/02-thumbnail.jpg" alt="">
                </a>
                <div class="portfolio-caption">
                    <h4>{{ obj.caption }}</h4>
                    <p class="text-muted">{{ obj.title }}</p>
                </div>
            </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    data: () => ({
        portfolioJSON: [
            {
                img: '/something/random/img.jpg',
                caption: 'Responsive Apps',
                title: 'Graphic and efficient'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'DevOps projects',
                title: 'Rapid deployment '
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Database management',
                title: 'Security and informations'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'IoT projects',
                title: 'New technology devices'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Challenges with renowned companies',
                title: 'A new vision on societal issues '
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Professional skills',
                title: 'Knowledge shared with experts' 
            },
        ]
    })
}
</script>

<style lang="css">

</style>



<template>
    <div class="footer-top">
        <div class="container flex">
            <section>
                <h3>AVADA TECH FORUM</h3>
                <p>Sed semper, nisl id feugiat eleifend, erat est digssim felis, quis auctor elit enim nec ante. Cras et nibh risus. Pellentesque non mi sit amet mi intermentum.</p>
            </section>
            <section>
                <h3>POPULAR TOPICS</h3>
                <ul>
                    <li>Morbi vitae dui euismod vulputate sollicitudin</li>
                    <li>Vivamus pellenteque, felis quis varius</li>
                    <li>Donec ornare pretium eget scelisque justo</li>
                </ul>
            </section>
            <section>
                <h3>RECENT POSTS</h3>
                <ul>
                    <li>Morbi vitae dui euismod vulputate sollicitudin</li>
                    <li>Vivamus pellenteque, felis quis varius</li>
                    <li>Donec ornare pretium eget scelisque justo</li>
                </ul>
            </section>
            <section>
                <h3>LATEST REPLIES</h3>
                <ul>
                    <li>Dario Pineda on Morbi vitae dui euismod vulputate sollicitudin</li>
                    <li>Dario Pineda on Morbi vitae dui euismod vulputate sollicitudin</li>
                </ul>
            </section>
        </div>
    </div>
    <div class="footer-bottom">
        <div class="container flex">
            <section>
                <p>© Copyright 2012 - 2023 | Avada Website Builder by ThemeFusion | All Rights Reserved | Powered by WordPress</p>
            </section>
            <section></section>
        </div>
    </div>

    
</template>

<script>


export default {
    name: 'Appfooter',
    components:{
    }
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.footer-top{
    border-bottom: 2px solid $lightgreyColor;
}
.footer-top .container{
    padding: 5.5rem 0;

    & section{
        width: calc(100%/4);
        padding-right: 20px;
        & h3{
            margin-bottom: 2rem;
        }

        & p{
            color: $greyColor;
            font-size: 1.1rem;
            line-height: 1.7rem;
            margin-top: 3.15rem;
        }
        & ul li{
            border-bottom: 2px solid $lightgreyColor;
            padding: 1.4rem 1.7rem 1.4rem 0;
            color: $greyColor;
            font-size: 1.1rem;
            transition: $transition;
            &:hover{
                color: $skyblueColor;
            }
        }
    }
}

.footer-bottom .container{
    height: 400px;
    justify-content: space-between;
    align-items: center;

}
  
</style>

  
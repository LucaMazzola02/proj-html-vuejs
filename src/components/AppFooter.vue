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
                <p>© Copyright 2012 - 2023 | <span>Avada Website Builder</span> by <span>ThemeFusion</span>  | All Rights Reserved | Powered by <span>WordPress</span></p>
            </section>
            <section>
                <ul class="flex">
                    <li class="bg-fb"><i class="fa-brands fa-facebook-f"></i></li>
                    <li class="bg-tw"><i class="fa-brands fa-twitter"></i></li>
                    <li class="bg-ig"><i class="fa-brands fa-instagram"></i></li>
                    <li class="bg-yt"><i class="fa-brands fa-youtube"></i></li>
                </ul>
            </section>
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
    height: 200px;
    justify-content: space-between;
    align-items: center;

    & p{
        color: $greyColor;
        font-size: 1.05rem;
    }

    & section p span{
        color: $blackColor;
        transition: $transition;
        &:hover{
            color: $skyblueColor;
        }
    }



    section ul li{
        width: 60px;
        height: 60px;
        border-radius: 50%;
        margin-left: 2.5rem;
        font-size: 1.5rem;
        position: relative;
        color: $whiteColor;
        & i{
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
    }
}
  
</style>

  
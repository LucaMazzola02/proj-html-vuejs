<template>
    <article>
        <div class="container flex">
            <div class="right-cover flex">
                <div class="cover-text">
                   <h3>REVIEWED PRODUCT</h3>
                   <h1>Mauris Viverra Atisan Ipsum Eget Felis Prims Efficitur Varius</h1>
                   <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum.</p>
                   <button class="button">READ MORE ></button>
                </div>
            </div>
            <div class="left-guides">
                <h1>Tutorials & Guides</h1>
                <div class="separator"></div>
                <div class="cards flex">
                    <div class="cards-image">
                        <img src="../assets/img/post_feat_img_23-320x202.jpg" alt="cards-image">
                    </div>
                    <div class="cards-text">
                        <h2>Donec ornare pretium eget scelisque justo</h2>
                        <p>October 11th, 2015|  Comments Off</p>
                    </div>
                </div>
                <div class="cards flex">
                    <div class="cards-image">
                        <img src="../assets/img/post_feat_img_22-320x202.jpg" alt="cards-image">
                    </div>
                    <div class="cards-text">
                        <h2>Donec ornare pretium eget scelisque justo</h2>
                        <p>October 11th, 2015|  Comments Off</p>
                    </div>
                </div>
                <div class="cards flex">
                    <div class="cards-image">
                        <img src="../assets/img/post_feat_img_20-320x202.jpg" alt="cards-image">
                    </div>
                    <div class="cards-text">
                        <h2>Donec ornare pretium eget scelisque justo</h2>
                        <p>October 11th, 2015|  Comments Off</p>
                    </div>
                </div>

            </div>
        </div>
    </article>
    
</template>
  
<script>
export default {
      name: 'Apptutorial',
       
  }
</script>
  
<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

article{
    margin-bottom: 8rem;
}
    .right-cover{
    width: 60%;
    height: 60vh;
    background-image: url(../assets/img/featured_article_1_bg.jpg);
    background-size: cover;
    color: $whiteColor;
    align-items: center;
    text-align: left;
    padding: 5rem;

    & .cover-text h3{
        margin-bottom: 1.3rem;
        font-size: 16px;
        font-weight: 600;
        letter-spacing: 4px;
    }

    & .cover-text h1{
        font-size: 45px;
    }

    & .cover-text p{
        font-size: medium;
        margin: 2.5rem 0;
    }
    .button{
        background-color: $blackColor;
        padding: 1.1rem 1.7rem;
        color: $whiteColor;
        font-size: 1.1rem;
        font-weight: bold;
        border-radius: 6px;
        transition: $transition;

        &:hover{
            background-color: $coralColor;
        }
    }
}

.left-guides{
    width: 40%;
    padding-left: 3rem;  

    & .separator{
        margin-bottom: 1.5rem;
    }
    & h1{
        font-size: 2.5rem;
        margin-bottom: 2rem;
    }

    & .cards{
        margin-top: 1rem;
    }
    & .cards-image{       
        height: 150px;
        & img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: $transition;
            &:hover{
                transform: scale(.85);
            }
        }
    }
    & .cards-text{
        padding-left: 1.5rem;
        & h2{
            font-size: 1.4rem;
            margin-bottom: 1rem;
            transition: $transition;
            &:hover{
                color: $skyblueColor;
            }
        }
    }
}


     
    
</style>
  
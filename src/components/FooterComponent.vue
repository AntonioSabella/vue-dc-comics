<template>
    <footer id="site_footer">
        <div class="footer_top">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="dc_comics">
                            <h4>Dc comics</h4>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>                                
                            </ul>
                        </div>
                        <div class="shop">
                            <h4>Shop</h4>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>                               
                            </ul>
                        </div>
                    </div>
                    <div class="col">
                        <div class="dc">
                            <h4>DC</h4>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li> 
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>                                  
                            </ul>
                        </div>
                    </div>
                    <div class="col">
                        <div class="sites">
                            <h4>Sites</h4>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Characters</a></li>                                 
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer_bottom">
            <div class="container">
                <div class="row">
                    <div class="signUp_button">
                        <button class="sign_up">Sign-Up NOW!</button>
                    </div>
                    <div class="follow_actions">
                        <h3>Follow Us</h3>
                        <div class="social_links">
                            <div><a href="#"><img src="@/assets/img/footer-facebook.png" alt=""></a></div>
                            <div><a href="#"><img src="@/assets/img/footer-twitter.png" alt=""></a></div>
                            <div><a href="#"><img src="@/assets/img/footer-youtube.png" alt=""></a></div>
                            <div><a href="#"><img src="@/assets/img/footer-pinterest.png" alt=""></a></div>
                            <div><a href="#"><img src="@/assets/img/footer-periscope.png" alt=""></a></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>

</script>

<style lang="scss" scoped>
    footer {
     width: 100%;
   }
  
   .footer_top {
       background-image: url("@/assets/img/dc-logo-bg.png");
       background-repeat: no-repeat;
       background-position: right;
       background-image: url("@/assets/img/footer-bg.jpg");
       background-repeat: no-repeat;
       background-position: left top;
       padding: 3rem;
       .container {
           width: 80%;
           margin: auto;
           .row {
               display: flex;
               column-gap: 3rem;
               .col {
                   width: 10%;
                   line-height: 1.2rem;
                   .dc_comics {
                       margin-bottom: 1rem;
                   }
                   h4 {
                       color: white;
                       font-weight: 600;
                       text-transform: uppercase;
                       margin-bottom: 1rem;
                       font-size: 15px;
                   }
                   ul {
                       list-style-type: none;
                   }
                   a {
                       text-decoration: none;
                       font-size: 12px;
                       color: lightgray;
                   }
               }
           }
       }
   }

   .footer_bottom {
       background-color: rgb(51, 50, 50);
       padding: 2rem;
       .container {
           width: 75%;
           margin: auto;
           .row {
               display: flex;
               align-items: center;
               justify-content: space-between;
               .follow_actions{
                   display: flex;
                   align-items: center;
                   column-gap: 1.2rem;
                   h3 {
                       color: rgb(4, 78, 224);
                   }
                   .social_links {
                       display: flex;
                       column-gap: 0.7rem;
                       img {
                           width: 20px;
                       }
                   }
               }
               .sign_up {
                   border: 2px solid rgb(4, 78, 224);
                   background-color: transparent;
                   color: white;
                   font-size: 16px;
                   text-transform: uppercase;
                   padding: 0.7rem;
                   cursor: pointer;
               }
           }
       }
   }
</style>
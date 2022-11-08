<script>
export default{
   name: "AppMain",
    data(){
        return{

        }
    }
}

</script>

<template>  
    <main>
        <div class="contentmenu">
            <div class="container">
                <h2>--> Content goes here </h2>
            </div>
        </div>
        <div class="infodcabout">
            <div class="container">
                <ul>
                    <li>
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
                        <span>DIGITAL COMICS</span> 
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-merchandise.png" alt="comics-merchandise">
                        <span>DC MERCHANDISE</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptionms-comics">
                        <span>SUBSCRIPTION</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="shop-comics">
                        <span>COMIC SHOP LOCATOR</span>
                    </li>
                   
                    <li>
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="dc-power-visa">
                        <span>DC POWER VISA</span>
                    </li>
                </ul>
            </div>
           
        </div>
    </main>
    
</template>


<style lang="scss" scoped>
    .contentmenu{
        display: flex;
        background-color: #1c1c1c;
        min-height: 150px;
        align-items: center;
        h2{
            color: white;
            font-size: 2rem;
        }
    }
    .infodcabout{
        justify-content: center;
        display: flex;
        align-items: center;
        min-height: 170px;
        background-color: #0282f9;
        ul{
            justify-content: space-between;
            display: flex;
            list-style: none;
            li{
                padding: 0 2rem;
                display: flex;
                align-items: center;
                img{
                    width: 50px;
                };
                span{
                    color: white;
                    padding-left: 1rem;
                }
            }
        }
    }
</style>
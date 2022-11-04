<template>
    <section>
 <div class="container">

    <div class="content">
        <h1>Diversify your portfolio.</h1>
        <p>Create an even more impressive portfolio by creating case studies for your projects. Simply follow our step-by-step guide.</p>
        <button>Start Free Trial</button>
    </div>
    <div class="img"></div>
 </div>
    </section>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    section{
        width: 100%;
        height: fit-content;
        display: flex;
        justify-content: center;

    }
    .container{
        width: 80%;
        height: 40rem;
        background-color: var(--blue);
        border-radius: 12px;
        padding-inline: 5rem;
        padding-top: 5rem;
        display: flex;
    }
    .img{
        background-image: url(../assets/Page\ Image.png);
        width: 50%;
        height: 100%;
        background-size: contain;
    }
    .content{
        color: white;
        width: 50%;

        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    h1{
font-size:2.8rem;
    }
    p{
        font-size: 1.2rem;
        font-weight: 300;
        width: 70%;
    }
    button{
  margin-top: 1rem;
      background: none;
        border: none;
        font-size: 1.2rem;
        font-weight: 600;
       
        padding-inline: 1.6rem;
        padding-block: 1rem;
        background: var(--white);
        border-radius: 7px;
        color: var(--blue);
        font-weight: 700;
        width: fit-content;
}
#blue-btn{

        background: var(
          --blue
        );

        color: var(--white);
        
}
</style>
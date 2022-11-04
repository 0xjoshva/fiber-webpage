<template>
    <section>
    <nav>
        <h3>Fiber</h3>
        <div class="links">
            <a href="" class="link">Community</a>
            <a href="" class="link">Pricing</a>
            <a href="" class="link">Features</a>
        </div>
        <div class="buttons">
            <button>Sign In</button>
            <button>Sign Up</button>
        </div>
    </nav>
    </section>
</template>
<script>
export default {
    
}
</script>
<style scoped>
section{
    width: 100%;
    height: 100px;
    display: flex;
    justify-content: center;
   background-color: #FBF8F3;
}
    nav{
        padding-top: 3rem;
        width: 80%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        position: fixed;
        background-color: #FBF8F3;
        padding-bottom: 1rem;
    }
    .links{
        display: flex;
        column-gap: 2rem;
        font-size: 1.1rem;
        

    }
    .link{
        text-decoration: none;
        color: var(--black);
        font-weight: 500;
    }
    nav h3{
        font-size: 1.4rem;
        font-weight: 800;
    }
    .buttons{
        display: flex;
        column-gap: 1rem;
    }
    button{
        background: none;
        border: none;
        font-size: 1.2rem;
        font-weight: 600;
       
        padding-inline: 2rem;
        padding-block: 1rem;
    }
    .buttons button:nth-child(2){
         background: var(--blue);
         color: var(--white);
         border-radius: 6px;
    }
</style>
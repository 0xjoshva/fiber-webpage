<template>
  <section>
    <div class="container">
      <div class="left">
        <div class="rating">
          <div class="stars">
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
          </div>
          <p>Rated 4.8/5 (243 reviews)</p>
        </div>
        <h1>Create your portfolio in minutes.</h1>
        <p id="para">
          With Fiber, you can setup your own personal portfolio in minutes with
          dozens of premade, beautiful templates.
        </p>
        <div class="herobtn">
          <button id="blue-btn">Start Free Trial</button>
          <button>View Examples</button>
        </div>
        <div class="checkdiv">
            <span class="check"><img src="../assets/Checkmark.svg" alt="" id="checkimg"> <p>No Credit Card Required</p></span>
            <span class="check"><img src="../assets/Checkmark.svg" alt="" id="checkimg"> <p>10 Free Templates</p></span>
        </div>
      </div>
      <img src="../assets/hero-Illustration.png" alt="" />
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
section {
  width: 100%;
  height: calc(100vh - 100px);
  display: flex;
  justify-content: center;
  background-color: #FBF8F3;
}
.container {

  display: flex;
  align-items: center;
  justify-content: space-between;
  height: calc(100vh - 100px);
  width: 80%;
  height: fit-content;

}
img {
  width: 50%;
}
.left{
    width:50%;
    height: fit-content;
}
.stars {
  display: flex;
  column-gap: 0.3rem;
}
.rating {
  display: flex;
  align-items: center;
  width: fit-content;
  column-gap: 1.2rem;
font-size: 1.2rem;
font-weight: 500;
margin-bottom: .2rem;
}
.checkdiv{
    display: flex;
    width: 100%;
    column-gap: 1rem;
    font-size: 1.15rem;
   color: var(--text);
   font-weight: 400;
}
.check{
    display: flex;
    justify-content: center;
    align-items: center;
    width: fit-content;
    column-gap: .5rem;
    margin-top: 1rem;
}
#checkimg{
    width: 1.5rem;
    height: auto;
}
h1{
    font-size: 4.2rem;
    line-height: 4.8rem;
    padding-bottom: 1rem;
    width: 90%;
}
button{
  margin-top: 1rem;
      background: none;
        border: none;
        font-size: 1.2rem;
        font-weight: 600;
       
        padding-inline: 1.6rem;
        padding-block: 1rem;
}
#blue-btn{

        background: var(
          --blue
        );

        color: var(--white);
        border-radius: 7px;
}
#para{
  width: 80%;
  font-weight: 400;
  color: var(--text);
  font-size: 1.1rem;
}

button:nth-child(2){
  color: var(--blue);
  text-decoration: 
  underline 2px;
}
</style>

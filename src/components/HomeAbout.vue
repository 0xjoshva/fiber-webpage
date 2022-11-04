<template>
  <section>
    <div class="header">
      <h4>Why Fiber?</h4>
      <h2>A good portfolio means good employability.</h2>
    </div>
    <div class="container">
      <div class="card">
        <img src="../assets/time.svg" alt="" />
        <h6>Build in minutes</h6>
        <p>
          With a selection of premade templates, you can build out a portfolio
          in less than 10 minutes
        </p>
      </div>
      <div class="card">
        <img src="../assets/time.svg" alt="" />
        <h6>Add custom CSS</h6>
        <p>
          With a selection of premade templates, you can build out a portfolio
          in less than 10 minutes
        </p>
      </div>
      <div class="card">
        <img src="../assets/time.svg" alt="" />
        <h6>Responsive</h6>
        <p>
          With a selection of premade templates, you can build out a portfolio
          in less than 10 minutes
        </p>
      </div>
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
section {
  width: 100%;
  height: fit-content;
  background: var(--white);
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 6rem;
  padding-bottom: 4rem;
}
.header {
  width: 80%;
  padding-bottom: 3rem;
}
h4 {
  color: var(--blue);
  font-weight: 700;
  font-size: 1.3rem;
}
h2 {
  font-size: 2.6rem;
  width: 50%;
}

.container {
  display: flex;
  width: 80%;
  column-gap: 2rem;
}
.card{
    display: flex;
    flex-direction: column;
    width: fit-content;
    row-gap: 1rem;
}
.card img{
    max-width: 50px;
}
.card h6{
    font-size: 1.1rem;
}
.card p{
    font-size: 1.2rem;
    color: var(--text);
    width: 75%;
}
</style>

<template>
  <div class="container-fluid p-0 overflow-hidden">
    <div id="card-bg-top" class="row g-0">
      <div
        lc-helper="background"
        class="col-lg-6 order-lg-2"
        style="
          min-height: 45vh;
          background-size: cover;
          background-position: center;
          background-image: url('https://i.imgur.com/TdQgrrF.png&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;auto=format&amp;fit=crop&amp;w=1352&amp;q=80');
        "
      ></div>
      <div id="card-top-left" class="col-lg-6 order-lg-1 my-auto px-5 py-5">
        <div class="lc-block">
          <div editable="rich">
            <h1>Our Vision</h1>
            <p class="lead">
              We aim to redefine the lending landscape, transforming it into a
              space characterized by integrity and trust. Olive Advance is here
              to support small- and mid-sized businesses in their growth journey
              without the stress associated with traditional lenders. When
              traditional banks make the process cumbersome, time-consuming, and
              often reject small business loans, we step in to provide a faster,
              more transparent alternative.
            </p>
          </div>
        </div>
      </div>
    </div>

    <div id="card-bg-bottom" class="row g-0">
      <div
        lc-helper="background"
        class="col-lg-6"
        style="
          min-height: 45vh;
          background-size: cover;
          background-position: center;
          background-image: url('https://i.imgur.com/C9QKf39.png&amp;q=80&amp;fm=jpg&amp;crop=entropy&amp;cs=tinysrgb&amp;w=1080&amp;h=768&amp;fit=crop&amp;ixid=eyJhcHBfaWQiOjM3ODR9');
        "
      ></div>
      <div id="card-bottom-right" class="col-lg-6 my-auto px-5 py-5">
        <div class="lc-block">
          <div editable="rich">
            <h1>Empowering Your Success</h1>
            <p class="lead">
              At Olive Advance, we are invested in your success. Our company
              culture thrives on open communication, ensuring that every voice
              is heard – from team members to executives. We believe that how we
              work together and develop as individuals and as an organization is
              as important as the financial solutions we provide.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OurVision",
};
</script>

<style scoped>
#card-top-left,
#card-bottom-right,
#card-bg-top,
#card-bg-bottom {
  background-color: rgb(24, 59, 84);
}

p,
h1 {
  color: #f7f7f7;
}
</style>

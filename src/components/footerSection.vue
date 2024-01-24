<template>
  <footer class="lg:px-[8rem] px-10 pt-20">
    <section class="flex justify-between flex-wrap">
      <div>
        <div class="flex gap-2">
          <img src="../assets/Group.png" class="w-8 h-7" alt="logo" />
          <span class="text-2xl font-semibold text-[#101828]">Clear Link</span>
        </div>
        <p
          class="text-gray-600 lg:max-w-[25rem] max-w-80 my-5 lg:text-sm text-xs"
        >
          ClearLink is your gateway to effortless, high-quality video
          conferencing. Join us in shaping the future of communication!
        </p>
      </div>
      <div>
        <h2 class="text-gray-500 mb-5">Products</h2>
        <ul>
          <li>Overview</li>
          <li>Features</li>
          <li>Solutions</li>
          <li>Tutorials</li>
          <li>Pricing</li>
        </ul>
      </div>
      <div>
        <h2 class="text-gray-500">Company</h2>
        <ul>
          <li>About us</li>
          <li>Career</li>
          <li>Press</li>
          <li>News</li>
          <li>Contact</li>
        </ul>
      </div>
      <div>
        <h2 class="text-gray-500">Resoruces</h2>
        <ul>
          <li>Blogs</li>
          <li>Events</li>
          <li>Help center</li>
          <li>Tutorials</li>
          <li>Support</li>
        </ul>
      </div>
      <div>
        <h2 class="text-gray-500">Legal</h2>
        <ul>
          <li>Terms</li>
          <li>Privacy</li>
          <li>Cookies</li>
          <li>Licenses</li>
          <li>Contact</li>
        </ul>
      </div>
      <div>
        <h2 class="text-gray-500 get">Get the App</h2>
        <ul>
          <li><img src="../assets/appstore.png" alt="app store" /></li>
          <li><img src="../assets/playstore.png" alt="playstore" /></li>
        </ul>
      </div>
    </section>
    <section class="flex flex-col md:flex-row justify-between py-12 bg-gray-50">
      <p class="text-gray-500">© 2023 ClearLink. All rights reserved.</p>
      <div class="flex gap-4">
        <span><a href=""><img src="../assets/linked.png" alt=""></a></span>
        <span><a href=""><img src="../assets/tt.png" alt=""></a></span>
        <span><a href=""><img src="../assets/fb.png" alt=""></a></span>
        <span><a href=""><img src="../assets/ig.png" alt=""></a></span>
        <span><a href=""><img src="../assets/git.png" alt=""></a></span>
        <span><a href=""><img src="../assets/yt.png" alt=""></a></span>
      </div>
    </section>
  </footer>
</template>
<style scoped>
li {
  margin-bottom: 14px;
  cursor: pointer;
}
h2 {
  margin-bottom: 16px;
  color: var(--Gray-500, #667085);

  font-family: Inter;
  font-size: 16px;
  font-style: normal;
  font-weight: 600;
  line-height: 24px; /* 150% */
}
.get {
  color: var(--Blue-dark-700, #004eeb);
  /* Text md/Semibold */
  font-family: Inter;
  font-size: 16px;
  font-style: normal;
  font-weight: 600;
  line-height: 24px; /* 150% */
}
@media only screen and (max-width: 1000px) {
  li,
  h2,
  .get {
    font-size: 12px;
  }
}
</style>

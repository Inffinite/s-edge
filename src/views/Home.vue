<template>
  <div class="home">
    <Header/>
    
    <div class="landing-area">

    <div class="dets-container">
      <div class="landing-name">
        Welcome to <br>
        <div style="color: #13aa52; margin-top: 10px; font-family: 'sfb';">StartEdge</div>
        <div class="isp-wr">
          <div class="isp-snack">
            <svg class="check" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M6.267 3.455a3.066 3.066 0 0 0 1.745-.723 3.066 3.066 0 0 1 3.976 0 3.066 3.066 0 0 0 1.745.723 3.066 3.066 0 0 1 2.812 2.812c.051.643.304 1.254.723 1.745a3.066 3.066 0 0 1 0 3.976 3.066 3.066 0 0 0-.723 1.745 3.066 3.066 0 0 1-2.812 2.812 3.066 3.066 0 0 0-1.745.723 3.066 3.066 0 0 1-3.976 0 3.066 3.066 0 0 0-1.745-.723 3.066 3.066 0 0 1-2.812-2.812 3.066 3.066 0 0 0-.723-1.745 3.066 3.066 0 0 1 0-3.976 3.066 3.066 0 0 0 .723-1.745 3.066 3.066 0 0 1 2.812-2.812zm7.44 5.252a1 1 0 0 0-1.414-1.414L9 10.586 7.707 9.293a1 1 0 0 0-1.414 1.414l2 2a1 1 0 0 0 1.414 0l4-4z" clip-rule="evenodd"/></svg>
            ISP
          </div>
        </div>
      </div>

      <div class="landing-details-wr">
        <div class="landing-details">
          We provide high bandwidth and reliable internet connection
          at a reasonable price to suit your online needs.
        </div>
      </div>

      <div class="landing-details-wr">
        <button class="landing-btn">
          Subscribe
        </button>
      </div>
    </div>

    <div class="satelite-wr">
        <div class="s-container"></div>
        <img src="https://firebasestorage.googleapis.com/v0/b/fir-edge.appspot.com/o/pexels.png?alt=media&token=0903bacc-0e6c-4364-bbac-84a5ba785df9" class="satelite">
      </div>
    </div>

    <div class="highlights">
      <div class="container">
        <div class="highlight">
          <div class="container">
            <div class="icon-wr pulse">
              <svg class="highlight-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M12 7a1 1 0 1 1 0-2h5a1 1 0 0 1 1 1v5a1 1 0 1 1-2 0V8.414l-4.293 4.293a1 1 0 0 1-1.414 0L8 10.414l-4.293 4.293a1 1 0 0 1-1.414-1.414l5-5a1 1 0 0 1 1.414 0L11 10.586 14.586 7H12z" clip-rule="evenodd"/></svg>
            </div>
          </div>

          <div class="highlight-name">
            More Bandwidth
          </div>

          <div class="highlight-desc">
            High speed internet
          </div>
        </div>
      </div>

       <div class="container">
          <div class="highlight">
            <div class="container">
              <div class="icon-wr pulse">
                <svg class="highlight-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path d="M13 7H7v6h6V7z"/><path fill-rule="evenodd" d="M7 2a1 1 0 0 1 2 0v1h2V2a1 1 0 1 1 2 0v1h2a2 2 0 0 1 2 2v2h1a1 1 0 1 1 0 2h-1v2h1a1 1 0 1 1 0 2h-1v2a2 2 0 0 1-2 2h-2v1a1 1 0 1 1-2 0v-1H9v1a1 1 0 1 1-2 0v-1H5a2 2 0 0 1-2-2v-2H2a1 1 0 1 1 0-2h1V9H2a1 1 0 0 1 0-2h1V5a2 2 0 0 1 2-2h2V2zM5 5h10v10H5V5z" clip-rule="evenodd"/></svg>
              </div>
            </div>

            <div class="highlight-name">
              Reliable
            </div>

            <div class="highlight-desc">
              Dependable connection
            </div>
          </div>
        </div>

        <div class="container">
          <div class="highlight">
            <div class="container">
              <div class="icon-wr pulse">
                <svg class="highlight-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M17.707 9.293a1 1 0 0 1 0 1.414l-7 7a1 1 0 0 1-1.414 0l-7-7A.997.997 0 0 1 2 10V5a3 3 0 0 1 3-3h5c.256 0 .512.098.707.293l7 7zM5 6a1 1 0 1 0 0-2 1 1 0 0 0 0 2z" clip-rule="evenodd"/></svg>
              </div>
            </div>

            <div class="highlight-name">
              Affordable
            </div>

            <div class="highlight-desc">
              We offer solutions to diverse price brackets
            </div>
          </div>
        </div>
    </div>

    <div class="packages">
      <div class="p-title">
        <span class="white">Choose your</span> package
      </div>

      <div class="package-wr">
        <div v-for="(mypackage, i) in packages" :key="i" class="package">
        <div style="justify-content: space-between; display: flex; align-items: center;">
          <div class="package-band">
            <div class="upto">
              up to
            </div>
            {{ mypackage.speed }}
            <div class="mbs">
              Mbps
            </div>
          </div>
          <div class="progress">
            <div class="p-bar not-selected">
              <div style="height: 20%;" class="p-bar-moving selected"></div>
            </div>
            <div class="p-bar not-selected">
              <div style="height: 40%;" class="p-bar-moving selected"></div>
            </div>
            <div class="p-bar not-selected">
              <div style="height: 60%;" class="p-bar-moving selected"></div>
            </div>
            <div class="p-bar not-selected">
              <div style="height: 10%;" class="p-bar-moving selected"></div>
            </div>
          </div>
        </div>

        <!-- <div class="package-deal">
          <svg class="p-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 0 1 0 1.414l-8 8a1 1 0 0 1-1.414 0l-4-4a1 1 0 0 1 1.414-1.414L8 12.586l7.293-7.293a1 1 0 0 1 1.414 0z" clip-rule="evenodd"/></svg>
          Light browsing
        </div> -->

        <div class="container">
          <div style="width: 100%;">
            <div class="p-price">
              KES {{ mypackage.price }} <span class="month"> / mo</span>
            </div>
            <button class="p-btn">
              Buy
            </button>
          </div>
        </div>
      </div>
      </div>
    </div>

    <div class="talk">
      <div class="p-title">
        <span class="white">Testimonials</span>
      </div>
      <div class="t-content-wr">
        <div v-for="(testimonial, i) in testimonials" :key="i" class="t-info">
          <div class="t-name">
            <img :src="testimonial.img" class="t-img">
            {{ testimonial.name }}
          </div>
          <div class="t-message">
            {{ testimonial.message }}
          </div>
        </div>
      </div>

      <div class="container">
        <button class="start">
          Get Started
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'

export default {
  name: 'Home',
  components: {
    Header
  },
  data(){
    return {
      testimonials: [
        {
          name: 'Ella',
          img: 'https://randomuser.me/api/portraits/women/79.jpg',
          message: 'Phenomenal service, reliable in bad weather'
        },
        {
          name: 'Patrice',
          img: 'https://randomuser.me/api/portraits/men/59.jpg',
          message: 'I\'m loving the after-purchase service'
        },
        {
          name: 'Mike',
          img: 'https://randomuser.me/api/portraits/men/55.jpg',
          message: 'Would highly reccomend'
        },
        {
          name: 'Boogie',
          img: 'https://randomuser.me/api/portraits/lego/0.jpg',
          message: 'Not as expensive as the rest'
        },
      ],
      packages: [
        {
          speed: '5',
          price: '2000',
        },
        {
          speed: '7',
          price: '3000',
        },
        {
          speed: '10',
          price: '4000',
        }
      ]
    }
  }
}
</script>

<style scoped>
@import '../styles/home.css';
</style>

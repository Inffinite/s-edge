<template>
  <div class="header">
    <div v-if="contact" @click="closeContact" class="contact-wr">
      <div v-if="contact" class="contact-card">
        <div class="c-title">
          Talk to us
        </div>
        <div @click="copyContact" class="c-tab">
          +254 757 690 940
          <div @click="copyContact" class="copy-btn">
            <svg class="copy-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path d="M9 2a2 2 0 0 0-2 2v8a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2V6.414A2 2 0 0 0 16.414 5L14 2.586A2 2 0 0 0 12.586 2H9z"/><path d="M3 8a2 2 0 0 1 2-2v10h8a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8z"/></svg>
          </div>
        </div>
      </div>
    </div>
    <div class="brand-wr">
      <img src="https://firebasestorage.googleapis.com/v0/b/fir-edge.appspot.com/o/logoo.png?alt=media&token=cbae6181-c173-4c11-8a1d-3b2b227b58e2" alt="P" class="brand-logo">
      <div class="brand-name">
        StarEdge
      </div>
    </div>
    <!-- <svg class="menu-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M3 5a1 1 0 0 1 1-1h12a1 1 0 1 1 0 2H4a1 1 0 0 1-1-1zm0 5a1 1 0 0 1 1-1h12a1 1 0 1 1 0 2H4a1 1 0 0 1-1-1zm6 5a1 1 0 0 1 1-1h6a1 1 0 1 1 0 2h-6a1 1 0 0 1-1-1z" clip-rule="evenodd"/></svg> -->
    <div class="menu-tabs">
      <div @click="openContact" class="m-tab">
        Contacts
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      contact: false
    }
  },
  methods: {
    async copyContact(){
      await navigator.clipboard.writeText('0757690940')
      alert("Copied to clipboard")
    },

    openContact(){
      this.contact = true
    },

    closeContact(){
      this.contact = false 
    }
  }
}
</script>

<style scoped>
@import '../styles/header.css';
</style>

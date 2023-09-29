<template>
    <div>
      <h2>Contact Me</h2>
      <button @click="toggleContact">Show Contact Info</button>
      <div v-if="showContactInfo">
        <p>Name:</p>
        <input v-model="name" placeholder="Name" />
  
        <p>Email:</p>
        <input v-model="email" placeholder="Email" />
  
        <p>Message:</p>
        <textarea v-model="message" placeholder="Message"></textarea>
  
        <button @click="submitForm">Submit</button>
      </div>
      <div v-else>
        <p>Click to show the contact form</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        showContactInfo: false,
        name: '',
        email: '',
        message: '',
      };
    },
    methods: {
      toggleContact() {
        this.showContactInfo = !this.showContactInfo;
      },
      submitForm() {
      },
    },
  };
  </script>
  
  
  



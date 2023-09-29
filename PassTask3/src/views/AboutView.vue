<template>
  <section class="about-me-page" style="text-align: center; align-items: center;">
    <div class="profile-image">
      <img src="https://images.fastcompany.net/image/upload/w_596,c_limit,q_auto:best,f_auto/wp-cms/uploads/2019/02/5-create-fake-people-in-2-seconds-on-this-insane-site.jpg" alt="insert image" class="hover-effect" style="max-width: 20%;">
    </div>
    <div class="about-content">
      <h1>About Me</h1>
      <p>
        Hello I'm me!
      </p>
      <button class="download-btn" @click="downloadFile">Download my Resume</button>
    </div>
  </section>
</template>

<script setup>
import { saveAs } from 'file-saver';

const downloadFile = () => {
  const filePath = '../src/assets/Sample PDF.pdf';

  fetch(filePath)
    .then(response => response.blob())
    .then(blob => {
      saveAs(blob, 'Sample PDF.pdf');
    });
};
</script>

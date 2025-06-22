---
layout: single
title: "Image Fusion Book"
permalink: /imagefusionbook/
author_profile: false
sidebar: false
---

<style>
.book-section {
  margin-top: 40px;
  padding: 20px;
  background: #f4f4f4;
  border-radius: 10px;
}
.download-button {
  display: inline-block;
  background-color: #007acc;
  color: white;
  padding: 10px 20px;
  border-radius: 6px;
  text-decoration: none;
  font-size: 16px;
  margin-top: 15px;
}
.download-button:hover {
  background-color: #005fa3;
}
</style>

<div class="book-section">
  <h2> Image Fusion Book</h2>

  <p>This book introduces core concepts, methods, and applications in image fusion, including multimodal fusion, evaluation, and downstream tasks.</p>

  <a class="download-button" href="/files/ImageFusionBook.pdf" onclick="countDownload()" download>
    📥 Click here to download PDF
  </a>

  <p style="margin-top: 20px;">This PDF has been downloaded <strong><span id="downloadCounter">...</span></strong> times.</p>
</div>

<!-- Firebase SDK -->
<script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-database.js"></script>

<script>
  // TODO: Replace with your actual Firebase config
	  const firebaseConfig = {
	  apiKey: "AIzaSyB19A68eFKpNSgID_ZqkIxXOxtj0uIqHv8",
	  authDomain: "imagefusion-book-download.firebaseapp.com",
	  databaseURL: "https://imagefusion-book-download-default-rtdb.firebaseio.com",
	  projectId: "imagefusion-book-download",
	  storageBucket: "imagefusion-book-download.firebasestorage.app",
	  messagingSenderId: "671210950650",
	  appId: "1:671210950650:web:29a7c67c612427c07dde43",
	  measurementId: "G-B5BGW0945J"
	};

  // Initialize Firebase
  firebase.initializeApp(firebaseConfig);

  // Reference to download count
  var countRef = firebase.database().ref("downloadCount");

  // Show count on page
  countRef.on('value', function(snapshot) {
    document.getElementById('downloadCounter').innerText = snapshot.val();
  });

  // Increase count on download
  function countDownload() {
    countRef.transaction(function(current) {
      return (current || 0) + 1;
    });
  }
</script>

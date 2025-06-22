---
layout: single
title: "Image Fusion Book"
permalink: /imagefusionbook/
author_profile: false
sidebar: false
---

<style>
.book-section {
  margin-top: 20px;
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
  <h2>Image Fusion Book</h2>
  <p>This book introduces core concepts, methods, and applications in image fusion, including multimodal fusion, evaluation, and downstream tasks.</p>

  <a id="downloadBtn" class="download-button" href="#">
    📥 Click here to download PDF
  </a>

  <p style="margin-top: 20px;">This PDF has been downloaded <strong><span id="downloadCounter">...</span></strong> times.</p>
</div>

<!-- Firebase SDK -->
<script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-database.js"></script>

<script>
  // Firebase 配置
  const firebaseConfig = {
    apiKey: "AIzaSyB19A68eFKpNSgID_ZqkIxXOxtj0uIqHv8",
    authDomain: "imagefusion-book-download.firebaseapp.com",
    databaseURL: "https://imagefusion-book-download-default-rtdb.firebaseio.com",
    projectId: "imagefusion-book-download",
    storageBucket: "imagefusion-book-download.appspot.com",
    messagingSenderId: "671210950650",
    appId: "1:671210950650:web:29a7c67c612427c07dde43",
    measurementId: "G-B5BGW0945J"
  };

  // 初始化 Firebase
  firebase.initializeApp(firebaseConfig);

  // 引用数据库中的 downloadCount
  const countRef = firebase.database().ref("downloadCount");

  // 实时更新页面上显示的下载次数
  countRef.on('value', function(snapshot) {
    document.getElementById('downloadCounter').innerText = snapshot.val() || 0;
  });

  // 动态绑定下载事件
  window.addEventListener('DOMContentLoaded', function () {
    const downloadBtn = document.getElementById("downloadBtn");

    if (downloadBtn) {
      downloadBtn.addEventListener("click", function (e) {
        e.preventDefault();  // 阻止默认跳转

        countRef.transaction(function(current) {
          return (current || 0) + 1;
        }, function(error, committed) {
          if (error) {
            console.error("❌ Failed to update download count", error);
            // 出错也允许下载
            window.location.href = "/files/ImageFusionBook.pdf";
          } else if (committed) {
            console.log("✅ Count updated, starting download");
            window.location.href = "/files/ImageFusionBook.pdf";
          }
        });
      });
    }
  });
</script>

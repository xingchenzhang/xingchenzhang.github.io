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

  <a id="downloadBtn" class="download-button" href="/files/ImageFusionBook.pdf">
    📥 Click here to download PDF
  </a>

  <p style="margin-top: 20px;">This PDF has been downloaded <strong><span id="downloadCounter">...</span></strong> times.</p>
</div>

<script>
  const namespace = "xingchenzhang";  // 可换成你主页地址中的唯一前缀
  const key = "imagefusionbook_download";  // 可换成其他唯一键

  function updateCounter() {
    fetch(`https://api.countapi.xyz/get/${namespace}/${key}`)
      .then(res => res.json())
      .then(data => {
        document.getElementById("downloadCounter").innerText = data.value;
      });
  }

  document.addEventListener("DOMContentLoaded", function () {
    const downloadBtn = document.getElementById("downloadBtn");
    if (downloadBtn) {
      downloadBtn.addEventListener("click", () => {
        fetch(`https://api.countapi.xyz/hit/${namespace}/${key}`)
          .then(() => updateCounter());
      });
    }
    updateCounter(); // 初始化加载次数
  });
</script>

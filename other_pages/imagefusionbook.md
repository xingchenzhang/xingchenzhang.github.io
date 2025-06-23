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
  const counterUrl = "https://counterapi.com/api/v1/";
  const counterNamespace = "xingchenzhang";  // 可改为你的用户名或站点标识
  const counterKey = "imagefusionbook";      // 可自定义唯一key

  function updateDownloadCount() {
    fetch(`${counterUrl}get/${counterNamespace}/${counterKey}`)
      .then(response => response.json())
      .then(data => {
        document.getElementById("downloadCounter").innerText = data.count ?? 0;
      })
      .catch(() => {
        document.getElementById("downloadCounter").innerText = "N/A";
      });
  }

  document.addEventListener("DOMContentLoaded", function () {
    const downloadBtn = document.getElementById("downloadBtn");

    // 初始化显示下载次数
    updateDownloadCount();

    // 每次点击下载按钮就 +1
    if (downloadBtn) {
      downloadBtn.addEventListener("click", function () {
        fetch(`${counterUrl}hit/${counterNamespace}/${counterKey}`)
          .then(() => updateDownloadCount());
      });
    }
  });
</script>

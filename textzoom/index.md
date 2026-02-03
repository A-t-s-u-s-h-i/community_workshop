---
title: Grok Modal Test
---

<style>
/* モーダルのスタイル */
.modal {
  display: none;
  position: fixed;
  z-index: 1000;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
}

.modal-content {
  background-color: white;
  margin: 15% auto;
  padding: 20px;
  border-radius: 10px;
  width: 80%;
  max-width: 600px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
  transform: translateZ(0); /* ハードウェアアクセラレーション */
}

.close {
  color: #aaa;
  float: right;
  font-size: 28px;
  font-weight: bold;
  cursor: pointer;
}

.close:hover,
.close:focus {
  color: #000;
}

.open-modal-btn {
  padding: 10px 20px;
  font-size: 16px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.open-modal-btn:hover {
  background-color: #0056b3;
}

.textarea-small {
  font-size: 0.8rem;
}

.textarea-medium {
  font-size: 1.0rem;
}
</style>

<!-- モーダルを開くボタン -->
<button onclick="openModal()">Open Modal</button>

<!-- モーダルウィンドウ -->
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close" onclick="closeModal()">&times;</span>
    <h2>Modal Window</h2>
    <label for="modal-story">Tell us your story (0.8rem):</label>
    <textarea id="modal-story" name="modal-story" class="textarea-small" rows="5" cols="33" placeholder="14px text area in modal"></textarea>
  </div>
</div>

<br><br>

<label for="story2">Tell us your story (1.0rem):</label>

<textarea id="story2" name="story2" class="textarea-medium" rows="5" cols="33" placeholder="16px text area">
</textarea>

<script>
function openModal() {
  document.getElementById("myModal").style.display = "block";
}

function closeModal() {
  document.getElementById("myModal").style.display = "none";
}

// モーダル外をクリックしたら閉じる
window.onclick = function(event) {
  var modal = document.getElementById("myModal");
  if (event.target == modal) {
    closeModal();
  }
}

// Escキーでモーダルを閉じる
document.addEventListener('keydown', function(event) {
  if (event.key === 'Escape') {
    closeModal();
  }
});
</script>
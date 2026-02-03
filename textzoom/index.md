---
title: The text zoom text page
---

<style>
label,
textarea {
  letter-spacing: 1px;
}

textarea {
  padding: 10px;
  max-width: 100%;
  line-height: 1.5;
  border-radius: 5px;
  border: 1px solid #ccc;
  box-shadow: 1px 1px 1px #999;
}

label {
  display: block;
  margin-bottom: 10px;
}

.textarea-small {
  font-size: 0.8rem;
}

.textarea-medium {
  font-size: 1.0rem;
}

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
  margin: 10% auto;
  padding: 20px;
  border-radius: 10px;
  width: 80%;
  max-width: 600px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
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
</style>

<!-- モーダルを開くボタン -->
<button class="open-modal-btn" onclick="openModal()">Open Modal (0.8rem text area)</button>

<br><br>

<label for="story1">Tell us your story (0.8rem):</label>

<textarea id="story1" name="story1" class="textarea-small" rows="5" cols="33" placeholder="14px text area">
</textarea>

<br><br>

<label for="story2">Tell us your story (1.0rem):</label>

<textarea id="story2" name="story2" class="textarea-medium" rows="5" cols="33" placeholder="16px text area">
</textarea>

<br><input type="text" style="font-size: 16px;" placeholder="16px text box">

<!-- モーダルウィンドウ -->
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close" onclick="closeModal()">&times;</span>
    <h2>Modal Window</h2>
    
    <label for="modal-story">Tell us your story (0.8rem in modal):</label>
    <textarea id="modal-story" name="modal-story" class="textarea-small" rows="5" cols="33" placeholder="14px text area in modal">
    </textarea>
  </div>
</div>

<script>
function openModal() {
  document.getElementById('myModal').style.display = 'block';
}

function closeModal() {
  document.getElementById('myModal').style.display = 'none';
}

// モーダル外をクリックしたら閉じる
window.onclick = function(event) {
  var modal = document.getElementById('myModal');
  if (event.target == modal) {
    closeModal();
  }
}
</script>
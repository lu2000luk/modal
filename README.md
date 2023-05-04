# Modal
A simple modal with js and css

Reserve the functions `openModal([id])` and `closeModal([id])`

Example:

```html
<button id="open-modal-button">Open Modal</button>
<div class="modal" id="my-modal">
  <div class="modal-overlay" id="my-modal-overlay">
    <div class="modal-content" id="my-modal-content">
      <div class="modal-header">
        <h2 class="modal-title">Modal Title</h2>
        <button class="modal-close" id="my-modal-close">×</button>
      </div>
      <p>Modal content goes here.</p>
    </div>
  </div>
</div>```

```javascript
// Show the modal when the user clicks the "Open Modal" button
document.getElementById('open-modal-button').addEventListener('click', () => {
  openModal('my-modal');
});

// Close the modal when the user clicks the "X" button
document.getElementById('my-modal-close').addEventListener('click', () => {
  closeModal('my-modal');
});
```

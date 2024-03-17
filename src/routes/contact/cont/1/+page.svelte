<svelte:head>
    <title>Связь</title>
</svelte:head>

<div class="container">
    <h1>Связь со мной</h1>
    <form action="action_page.php">
  
      <label for="fname">Ваше имя</label>
      <input type="text" id="fname" name="firstname">
  
      <label for="lname">Фамилия</label>
      <input type="text" id="lname" name="lastname">
  
      <label for="country">Страна</label>
      <select id="country" name="country">
        <option value="russia">Russia</option>
        <option value="belarus">Belarus</option>
        <option value="china">China</option>
      </select>
  
      <label for="subject">Ваши предложения</label>
      <textarea id="subject" name="subject" style="height:100px"></textarea>
  
      <a href="./1/2" class="but">Отправить</a>
  
    </form>
  </div>

  <style>
    input[type=text], select, textarea {
  width: 100%; 
  padding: 12px; 
  border: 1px solid #ccc; 
  border-radius: 4px; 
  box-sizing: border-box; 
  margin-top: 6px; 
  margin-bottom: 16px; 
  resize: vertical 
}

.but {
  background-color: #aa0473;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.but:hover {
  background-color: #455da0;
}
.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}
  </style>
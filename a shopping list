<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Shopping list example</title>
    <style>
      li {
        margin-bottom: 10px;
      }

      li button {
        font-size: 8px;
        margin-left: 20px;
        color: #666;
      }
    </style>
  </head>
  <body>

    <h1>My shopping list</h1>

    <div>
      <label for="item">Enter a new item:</label>
      <input type="text" name="item" id="item">
      <button>Add item</button>
    </div>

    <ul>

    </ul>

    <script>
      const input = document.querySelector('input');
      const addItemBtn = document.querySelector('button');
      const list = document.querySelector('ul');

      addItemBtn.onclick = function(){
        let myItem = input.value;
        input.value = '';

        const listItem = document.createElement('li');
        const listText = document.createElement('span');
        const deleteItemBtn = document.createElement('button');

        listItem.appendChild(listText);
        listText.textContent = myItem;
        listItem.appendChild(deleteItemBtn);
        deleteItemBtn.textContent = 'Delete';
        list.appendChild(listItem);

        deleteItemBtn.onclick = function(e){
        list.removeChild(listItem);
        }
         
      input.focus();
      }
     </script>
  </body>
</html>

```javaScript
let AllMenu = document.querySelector('#allMenu').children;
let searchBtn = document.querySelector('#searchBtn');
let inputValue = document.querySelector('#inputValue');

export function checkSearchPanel(){
      if(searchBtn.style.display === 'none' && inputValue.style.display === 'none'){
        inputValue.style.display = 'flex';
        searchBtn.style.display = 'flex';
      }else{
        inputValue.style.display = 'none';
        searchBtn.style.display = 'none';
        showAllMenu();
      }
  }
```

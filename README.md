# Todolist

## `addEventListener` 함수를 이용해 `클릭이벤트`로 투두리스트 구현😀

```javascript
inputButton.addEventListener('click', addTodo); //클릭이벤트 후

function addTodo(){

 //input에 입력한 todo
 const todo = document.querySelector('.todoItem').value
 
if (todo === '' || todo === null) {
    alert('할일 리스트를 입력해주세요.');
    document.querySelector('.todoItem').value = '';
    document.querySelector('.todoItem').focus(); //사용자 편의성, => ui
    return;

  } else if (todo !== '' || todo !== null) {
    alert('할일 리스트가 추가되었습니다.');
    todoArray.push(todo);
    document.querySelector('.todoItem').value = '';
    document.querySelector('.todoItem').focus(); //사용자 편의성, => ui
    console.log(todo);
  }
}

```

자바스크립트에서 `const todoArray= [];` 로 리스트를 배열로 선언   


---

<div>
<img src="https://user-images.githubusercontent.com/56811978/200451772-35459f36-d4a4-415e-8b46-48628bc39918.jpg" width="500">
</div>

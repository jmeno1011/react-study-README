# 리덕스 해보기

## 액션

상태 변화가 일어날때 생기는 액션을 하나의 객체로 표현함  
그래서 어떤 변화가 있을때 마다 액체 객체를 만들어야하는 번거로움이 있어 함수로 만들어 놓고 관리한다.  
여기서 액체 객체란 아래와 같은 내용이다.

```javascript
{
  type: "액션 내용", 데이터;
}
```

・예시

```javascript
const addTodo = (data) => {
  return {
    type: "ADD_TODO",
    data,
  };
};

// return 안쓸경우 ()로 처리
const chagneInput = (text) => ({
  type: "CHANGE_INPUT",
  text,
});
```

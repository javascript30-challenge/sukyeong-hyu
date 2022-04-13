## 3일차: CSS 조절하기 🎨

> range바 값을 JS에서 받아와서 css에 변화를 주는 코드 구현입니다.

<br>

---

### 기능 정리 ⚙️

1. spacing, blur, base color 를 조절하는 input을 전부 js에서 불러옵니다.
2. 이벤트 핸들러를 사용해서 input의 변화하는 값들을 받아옵니다.
3. style 속성을 사용해서 변화하는 값들을 해당 css에 적용해줍니다.

<br>

---

### 새로 알게 된 내용 ✨

1. <code>input type=range</code> 에서 이벤트를 핸들링하는 경우, <code>onchange</code>를 사용하면 가장 마지막 값만 반영되고, <code>oninput</code>을 사용하면 바가 움직일 때 변하는 모든 값을 반영합니다.

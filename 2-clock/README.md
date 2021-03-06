## 2일차: 시계 만들기 🕰

> transform의 rotate 속성을 이용해서 현재 시각을 나타내는 코드 구현입니다.

<br>

---

### 기능 정리 ⚙️

1. 시침 / 분침 / 초침을 각각 알맞은 사이즈로 조정합니다.
2. 각각의 침들이 회전에도 중심축을 벗어나지 않도록 설정합니다.
3. new Date()로 현재 시각을 받아온 뒤, 시침 / 분침 / 초침을 알맞은 위치로 각도를 조절합니다.
4. setInterval을 이용해서 매초마다 초침을 회전합니다.
5. 초침의 숫자가 60이 되었을 때, 분침은 6도만큼, 시침은 0.5도만큼 움직여주고, 초침 숫자를 초기화해줍니다.

<br>

---

### 새로 알게 된 내용 ✨

1. 시침과 분침의 크기를 줄이면, 오른쪽이 줄기 때문에 중심축을 벗어납니다. 이를 방지하기 위해는 position: absolute에 top: 50%, right: 50% 를 주어야 합니다.
2. getElementByClassName은 **HTMLCollection 이라는 배열**을 반환하고, querySelector은 parameter랑 매치되는 가장 첫번째 **element**를 반환합니다.
3. setInterval 함수는 바로 사용하면 되고, clearInterval 을 사용한다면 setInterval 을 변수에 저장하면 됩니다.
4. JS에서 css를 제어할 때는 아래와 같은 방식으로 사용할 수 있고, 값은 string으로 작성합니다.
   `document.querySelector('.hello').style.fontSize = '50px'`

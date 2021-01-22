# flexbox 
## flexbox의 종류
1. flex-container(부모)  
2. 플렉스 아이템들(자식)  

### 플렉스 컨테이너(부모)
## 1. `justify-content`: 주축을 기준으로 아이템 정렬
### 값들
center: 중앙정렬
start:그냥 왼쪽 정렬 같음
space-between: 양끝 가장자리에 자동으로 맞춰서 정렬
space-around: 여백을 자동으로 맞춰서 중앙으로 균등정렬됨
등이 들어갈 수 있다.

## 2. `align-items`: 서브축을 기준으로 아이템 정렬, center, start, end
## 3. `flex-direction`: row가 디폴트값, colunm으로 정렬 시 서브축과 메인축 바뀜, colunm-reverse도 있음
## 4. `align-content`: 원래있던 요소들과의 *간격*을 어떻게 배치할건지
## 5. ☆★`flex-wrap: nowrap(기본-안떨굼), wrap(떨굼);`: 너비값 안에서 너비가 줄어들 때, 자식들을 어떻게 배치할건지
## 6. `flex-flow: wrap row;` : 속기형, flex-wrap(떨구기) + flex-direction(방향)을 한번에 설정할수 있음.
## 7. `display:inline-flex`: flex를 자식이 차지한 너비만큼 부모 너비가 결정됨. ex.gnb에서 활용가능
### 값들
flex-start: 왼쪽에 붙어서 정렬(float:left처럼)
flex-end: 오른쪽에 붙음(float:right처럼)
inline-flex: 자식이 차지한 너비만틈 부모너비가 결정.

```css
/* 부모 요소들*/
.parent{
    display:flex;
    justify-content:center;
    align-items:center;
    flex-direction:row;
    align-content: space-between;
    flex-wrap: wrap;
    flex-flow: wrap row;
}
```


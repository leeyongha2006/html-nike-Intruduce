# html-nike-Intruduce
나이키 소개 사이트
자바 스크립트 애니메이션 및 현재 시간
# 전체화면
![image](https://github.com/leeyongha2006/html-nike-Intruduce/assets/126844590/706a61bd-f104-4ac7-8d99-a8ba6e364761)
---
자바 스크립트 현재 시간

``` javascript
    let now = new Date();
    let year = now.getFullYear();
    let month = now.getMonth();
    let date = now.getDate();
    let hour = now.getHours();
    let minute = now.getMinutes();
    let second = now.getSeconds();
        
     console.log(now);
    month = month < 10 ? `0${month}` : month
    date = date < 10 ? `0${date}` : date
    hour = hour < 10 ? `0${hour}` : hour
    minute = minute < 10 ? `0${minute}` : minute
    second = second < 10 ? `0${second}` : second
    
    todayDiv.textContent = hour + "시 " + minute + "분 " + second + "초";
}
setInterval(getTime, 1000)
```
#### 1. new Date()를 사용하여 현재 시간 정보를 얻습니다.
#### 2. getYear(), getMonth(), getDate(), getHours(), getMinutes(), getSeconds() 메서드를 사용하여 현재 년도, 월, 일, 시간, 분, 초를 추출합니다.
#### 3. 각 시간 구성 요소(월, 일, 시, 분, 초)가 한 자릿수인 경우 앞에 0을 추가하여 두 자릿수로 만듭니다.=
#### 4. todayDiv.textContent를 사용하여 HTML 문서 내의 특정 요소(여기서는 todayDiv)에 현재 시간을 문자열로 설정합니다. 시간은 "시", "분", "초"로 구분되어 표시됩니다.

#### 5. setInterval(getTime, 1000)을 사용하여 getTime 함수를 1초마다 호출하여 실시간으로 시간을 업데이트합니다.


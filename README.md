# html-nike-Intruduce
나이키 소개 사이트
자바 스크립트 애니메이션 및 현재 시간

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
전체화면
![image](https://github.com/leeyongha2006/html-nike-Intruduce/assets/126844590/706a61bd-f104-4ac7-8d99-a8ba6e364761)

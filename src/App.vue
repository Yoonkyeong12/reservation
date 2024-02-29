<template>
  

  <header>
  <h1>개금고등학교</h1>
  <nav>
    <a href = localhost:80/index.php>개금고 홈페이지</a>
    <a href ="https://web-schedule-17xco2nlt08ahbu.sel5.cloudtype.app/">개금고 청원사이트</a>
    
  </nav>
</header>

  <h3 style ="red">체육관/운동장 예약하기</h3>
  <form method="get" action="form_app.js">
      <fieldset>
        <legend>예약자 정보</legend>
        <label for ="sub">대표 예약자명</label>
        <input type ="text" name = "person" id = "sub" placeholder="홍길동"><br><br>
        <label for = "phone"> 휴대폰</label>
        <input type ="tel" name = "tell" id ="phone" placeholder = "연락할 수 있는 전화번호"><br><br>
        <label for ="sub">총 사용 인원수</label>
        <input type ="text" name = "person" id = "sub" placeholder="n명"><br><br>
          
      </fieldset>

      <fieldset>
        <legend>일자 선택 및 시간 선택</legend>
        <label for ="date">날짜</label>
        <input type = "date" name = "reservation_date" id="date"><br><br>
        <label for ="start_time">시작시간</label>
        <input type = "time" name = "reservation_time" min="09:00" max="20:00" id ="start_time"><br><br>
        <label for ="end_time">마감시간</label>
        <input type = "time" name = "reservation_time" min="09:00" max="20:00" id ="end_time"><br><br>
        <a>* 최대 4시간까지 대관 가능합니다</a><br><br>
        <label for = "position">위치 :</label>
        <input type = "radio" name = "site" id="position" value="yes">금학관(강당)
        <input type = "radio" name = "site" value="no">운동장
      </fieldset>
      <br>
      <input type="submit" value="예약">
      <input type="reset" value="취소">
      
  </form>
</template>

<script>


export default {
  name: 'App',
  components: {
   
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#sub {
  position: fixed;
  
}

header a {
  color: white;
  padding : 10px
}

header {  
  height: 75px;
  padding: 1rem;
  color: white;
  background: teal;
  font-weight: bold;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>

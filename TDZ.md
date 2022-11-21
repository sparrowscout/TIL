# TDZ (일시적 비활성 구역, Temporal Dead Zone)
var는 정의 되기 전에 접근(참조)할 수 있지만, let과 const는 정의되기 전에 접근할 수 없음<br/>
var, let, const는 모두 호이스팅됨. 즉, 코드가 실행되기 전에 처리되고, 해당 스코프 상단으로 올라감
<p>let, const는 호이스팅되지만, 정의되기 전에 접근할 수 없기 때문에 <br/>
<strong>스코프 시작 후 ~ let, const 정의 전까지 일시적으로 TDZ에 있게 됨.</strong></p>

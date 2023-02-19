## 입출력

. 입력은 Buffered Reader를 사용
(Scanner로 입력 받을 수 있지만 시간초과될 수 있음)
```Java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
```
. Text File을 생성 후 Text File에서 입력받을 수 있다.<br>
이는 테스트 케이스로 검증 시 계속해서 입력할 수고를 줄여준다.<br>
```Java
BufferedReader br = new BufferedReader(new FileReader(new File("src/input.txt")));
```
### BufferedReader
. BufferReader란 입력값을 Buffer에 한번에 저장해주는 명령어이다.
```Java
br : 버퍼 객체
br.readLine() // 버퍼의 자료를 한줄씩 읽는다.
```

### StringTokenizer
. Buffer의 입력값을 한줄씩 읽어 st 객체에 저장한다.<br>
```Java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
StringTokenizer st = new StringTokenizer(br.readLine());

// 정수형
int c;
c = Integer.parseInt(st.nextToken());

// String
String str;
str = br.readLine();
for(int j=0; j<str.length(); j++){
    if(str.charAt(j) == 'X'){
        break;
    }
}
```

## 자료형
. 아래만 기억해도 충분하다<br>
|자료형|크기|bit|비고|
|-|-|-|-|
|int|-2^31 ~ 2^31|32bit||
|long|-2^64 ~ 2^64|64bit||
|float||32bit|소수점|
|double||64bit|소수점|
|char||16bit|문자|
|boolean||1bit|TRUE OR FALSE|

## 배열
. 1차원 배열


## 자료구조
https://wikidocs.net/206 <br>
https://velog.io/@jinmin2216/%EC%9E%90%EB%A3%8C%EA%B5%AC%EC%A1%B0-2.-JAVA-Collection







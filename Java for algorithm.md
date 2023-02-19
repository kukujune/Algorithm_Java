## 입출력

. 입력은 Buffered Reader를 사용
(Scanner로 입력 받을 수 있지만 시간초과될 수 있음)
```Java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
```
. Text File을 생성 후 Text File에서 입력받을 수 있다.<br>
이는 테스트 케이스로 검증 시 계속해서 입력할 수고를 줄여준다.
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
. Buffer의 입력값을 한줄씩 읽어 st 객체에 저장한다.
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


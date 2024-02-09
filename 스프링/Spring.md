>>StringBuilder와 StringBuffer의 차이
문자열 연산으로 객체의 공간이 부족해지는 경우, 기존의 버퍼 크기를 늘려 유연하게 동작한다. 이는 String과 다른 기본적인 차이점이다.
StringBuilder와 StringBuffer의 차이는, 동기화의 여부이다. StringBuffer는 메서드별로 동기화 키워드가 존재합니다.
멀티스레드 환경에서도 동일한데 반면에, StringBuilder는 동기화를 보장하지 않습니다.

String은 짧은 문자열들을 더할 경우에 사용합니다.
StringBuffer는 스레드에 안전한 서비스가 필요할 때, 개발 중인 시스템이 스레드에 어떤 영향을 미칠지 모를 때 사용하면 좋습니다.
StringBuilder는 스레드에 관계 없는 서비스를 개발할 경우 사용하는 것이 좋습니다.
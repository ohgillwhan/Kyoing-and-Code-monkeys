# @Override 애너테이션을 일관되게 사용하라

## 핵심정리

```
재정의한 모든 메서드에 @Override 애너테이션을 달면 실수 했을 때 컴파일러가 바로 알려줄 것이다. 예외는 한 가지뿐. 구체 클래스에서 (extends나 implements 받는) 상위 클래스의 추상 메서드를 재정의한 경우에는 이 애너테이션을 달지 않아도 된다.
```

```
구체 클래스에서 추상메서드를 재정의하는 경우에는 굳이 애너테이션을 달지 않더라도 재정의 하지 않으면, 컴파일 에러를 뿜기 때문에 메소드 구현을 강제해야함을 보장받을 수 있고 이로인해 안정성을 보장 받을 수 있다고 생각한다. 근데 통일성을 위해서라면 모든 재정의를 하는 메소드에는 @Override 애너테이션을 다는 것이 좋지 않을까? 라는 생각이 들고 IDE툴을 이용 하기 때문에 모 어느정도는 당연히 알아서 보장되는 문제라는 생각이 든다.
```

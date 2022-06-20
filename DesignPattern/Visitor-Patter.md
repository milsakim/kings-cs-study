# Visitor Pattern

## Visitor Pattern이란?
* 어떤 객체에 수행할 작업을 별도의 클래스로 정의하여 분리한다. 작업들을 정의한 클래스를 `visitor`라고 하며, 객체에 새로운 작업을 수행하고 싶으면 해당 객체의 클래스를 변경할 필요 없이 새로운 `visitor`를 정의하면 된다.  

## Visitor Pattern의 구조
![CleanShot 2022-06-20 at 17 00 37@2x](https://user-images.githubusercontent.com/46441723/174553825-994a5b8e-e8f3-402b-ab8c-7dfe449e49c4.png)
**Visitor**  
* `ConcreteElement`의 클래스들을 방문(visit)해서 수행할 작업을 정의한다.  

**ConcreteVisitor**  
* `Visitor`에 정의된 작업들을 실제로 구현하는 클래스이다.  

**Element**  
* `Visitor`를 argument로 받는 `Accept` operation을 정의한다.  

**ConcreteElement**  
* `Element`에서 정의해놓은 `Accept` operation을 실제로 구현한다.  

**ObjectStructure** 
* element들을 열거할 수 있다.  
* 자신의 element들을 visitor가 방물할 수 있도록 하는 high-level interface를 제공할 수 있다.  
*  composite 형태거나 list나 set과 같은 collection이다.  

## 예시(Swift)

## Reference
https://brownbears.tistory.com/575

# 인프런 스프링 입문 강의

**MVC 패턴 흐름 순서**
controller → service → repository (jpa interface 생성)


## Annotation

- `@Controller`</br>
    View를 반환하기 위해 사용.

- `@RestController`</br>
    @Controller의 역할을 수행하지만 View가 아닌 JSON과 같은 데이터를 반환하는 용도로 사용.

- `@Entitiy`</br>
    JPA가 관리하는 것이라고 알림.</br>

    - `@Id`</br>
        해당 column이 PK인 것을 알림
    
    - `@GeneratedValue`</br>
        Auto Increment 설정
    
    - `@Column()`
        컬럼의 속성 설정

- `@Configuration`

- `@Bean`

## 

`Optional`</br>
    자바 8에 들어간 기능.
    데이터를 가져올 때 null인 경우를 생각하여 null을 그대로 반환하지 않고 Optional을 감싸서 반환.

`EntityManager`</br>
    JPA는 EntityManager로 모든 것이 돌아감.</br>
    build.gradle에서 implementation 'org.springframework.boot:spring-boot-starter-data-jpa'을 했을 때 자동으로 EntitiyManager를 생성해준다.

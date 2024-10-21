# 의미
Relational Database에서 Data를 검색하고 조작하는 수학적 Query Language

# 기본 연산자
## 1. Select : $\rm \sigma$
- 특정 조건을 만족하는 Tuple(Row, Record)만 선택하는 연산
$$\rm \sigma_{A ~ = ~ B ~ \wedge ~  D ~ > ~ 5}$$

## 2. Project : $\rm \Pi$
- 테이블에서 특정 Column(Attribute)만을 선택하는 연산
- 중복된 행을 제거
$$\rm \Pi_{A, ~ C}(r)$$

## 3. Union : $\rm \cup$
- 두 Relation에서 중복을 제거하고 모든 Tuple을 결합
    - 두 Relation은 동일한 Attribute을 가져야 함
$$\rm r_1 ~ \cup ~ r_2$$

## 4. Set Difference : $\rm-$
- 첫 번째 Relation에서 두 번째 Relation과 겹치지 않는 Tuple을 반환
$$\rm r_1 ~ - ~ r_2$$

## 5. Cartesian Product : $\rm\times$
- 두 Relation의 모든 Tuple을 모든 가능한 조합으로 결합하는 연산
- 대부분 의미가 없는 연산인 경우가 많음
- 곱집합
$$\rm r_1 ~ \times ~ r_2$$

## 6. Rename : $\rm \rho$
- Relational Algebra 표현식의 결과를 이름 붙이는 연산
    - Relation을 하나 이상의 이름으로 부를 수 있게 함

> Relation $\rm E$에 대해서 $\rm \rho_x(E)$는 $\rm E$라는 Relation을 $\rm X$라는 새로운 이름으로 변경

> Relation $\rm E$에 대해서 $\rm \rho_{x(A_1, ~ A_2, ~ \cdots, ~ A_n)}(E)$는 Relation $\rm E$의 이름을 $\rm X$로 변경하고 Relation $\rm E$의 Key들의 이름을 $\rm A_1, ~ A_2, ~ \cdots, ~ A_n$로 변경

# 추가 연산자
## Natural Join : $\rm \bowtie$
![Natural Join example](./img/Natural_Join.svg)

### Left Outer Join
Natural Join과 유사하나 앞의 Relation에 해당하는 행이 없을 경우 Null 값을 삽입하는 연산
![Left Outer Join example](./img/Left_Outer_Join.svg)

### Right Outer Join
Natural Join과 유사하나 뒤의 Relation에 해당하는 행이 없을 경우 Null 값을 삽입하는 연산
![Right Outer Join example](./img/Right_Outer_Join.svg)

### Full Outer Join
Natural Join과 유사하나 모든 Relation에 해당하는 행이 없을 경우 Null 값을 삽입하는 연산
![Full Outer Join example](./img/Full_Outer_Join.svg)
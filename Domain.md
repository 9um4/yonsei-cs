# 의미
- 각 Attribute들이 가질 수 있는 값들의 범위 혹은 집합
- 특정 Attribute가 가질 수 있는 유효한 값들의 Type과 Constraints를 정의하는 개념

# 종류 (Postgresql)
1. char(n)
- 고정된 길이(n)의 string
2. varchar(n)
- 최대 길이가 n으로 정해져 있는 string
3. int
- 정수 (machine-dependent)
4. smallint
- `int`보다 작은 값을 가지는 정수 (machine-dependent)
5. numeric(p, d)
- 총 길이가 $\rm p$이고 소수점 이하의 $\rm d$의 길이를 갖는 실수
6. real, double precision
- 일반적인 실수 (각각 Floating Point, Double-Precision Floating Point) (machine-dependent)
Visual Studio 2019에서는 scanf함수가 먹히지 않아
`#define _CRT_SECURE_NO_WARNINGS` 이 코드를 상단에 작성해도 에러가 뜸
프로젝트 - 속성 - C/C++ - 고급 - 특정 경고 사용 안 함 옆에 6031 적어줘도 
수행 안됨. 결국 scanf 를 scanf_s로 해주었다. 
scanf_s 를 사용할땐 반드시 뒤에 &변수명 적어줄것.
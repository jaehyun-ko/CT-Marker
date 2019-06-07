# 컴퓨팅사고력 조교를 위한 채점 프로그램

![](./capture.PNG)

## 소개

컴퓨팅사고력 조교를 위한 체점 프로그램 CT marker입니다.

학생들의 답안 코드를 한번에 체점하고, 미제출 리스트, 런타임 에러 리스트, 오답 리스트 출력을 지원합니다.

또한 오답코드는 difflib.differ() 를 이용하여 차이점을 분석하여 출력해줍니다.



## 요구사항

#### python3

#### openpyxl

```shell
pip install openpyxl
```

#### pyqt5

```
pip install pyqt5
```

#### student_info.xlsx

```
학생들의 이름, 학번이 적힌 액셀 파일
이름은 B3셀부터 열 방향으로
학번은 C3셀부터 열 방향으로 추가되어야 합니다.

서강대학교 조교 페이지에서는 수강생 메뉴에서 엑셀로 정보 가져오기를 통해 받으실 수 있습니다.
이 때에는 .xls파일을 내려받게 되는데, '다른 이름으로 저장'을 통해 .xlsx파일로 바꾸어주셔야 합니다. 
이 외의 경우 직접 엑셀 파일을 양식에 맞추어 만들어야 합니다

이 때 CTmarker.py에서 num_std 를 엑셀 파일의 학생 수에 맞게 수정해주세요
```

#### solution.py

```
정답 코드
```

## 기타 설정할 사항

#### 파일명 양식

```
{id}는 학번으로, {name}은 이름으로 파싱됩니다.
입력한 파일명과 일치하는 파일을 체점하는 것이 아니라
입력한 파일명을 포함하는 파일을 체점합니다.

더 엄격한 파일명 검사는 아직 지원하지 않습니다.
```

## 주의

```
채점 결과에 대해 어떠한 책임도 지지 않습니다.

이 채점 프로그램은 보조용입니다.
직접 학생들의 코드를 한번 더 확인해주시기 바랍니다.
저 또한 보조용으로 사용하고 있으며, 모든 학생들의 코드를 다시 확인하고 있습니다.
```

### 참고한 사이트
PyQt5 tutorials : https://wikidocs.net/21952

Python regex : http://pythonstudy.xyz/python/article/401-%EC%A0%95%EA%B7%9C-%ED%91%9C%ED%98%84%EC%8B%9D-Regex

git init : git 생성하기
git clone git_path : 코드가져오기
git checkout branch_name : 브랜치 선택하기
git checkout -t remote_path/branch_name : 원격 브랜치 선택하기
git branch branch_name : 브랜치 생성하기
git branch -r : 원격 브랜치 목록보기
git branch -a : 로컬 브랜치 목록보기
git branch -m branch_name change_branch_name : 브랜치 이름 바꾸기
git branch -d branch_name : 브랜치 삭제하기
git push remote_name — delete branch_name : 원격 브랜치 삭제하기 ( git push origin — delete gh-pages )
git add file_path : 수정한 코드 선택하기 ( git add * )
git commit -m “commit_description” : 선택한 코드 설명 적기 ( git commit -m “내용”)
git push romote_name branch_name : add하고 commit한 코드 git server에 보내기 (git push origin master)
git pull : git서버에서 최신 코드 받아와 merge 하기
git fetch : git서버에서 최신 코드 받아오기
git reset — hard HEAD^ : commit한 이전 코드 취소하기
git reset — soft HEAD^ : 코드는 살리고 commit만 취소하기
git reset — merge : merge 취소하기
git reset — hard HEAD && git pull : git 코드 강제로 모두 받아오기
git config — global user.name “user_name ” : git 계정Name 변경하기
git config — global user.email “user_email” : git 계정Mail변경하기
git stash / git stash save “description” : 작업코드 임시저장하고 브랜치 바꾸기
git stash pop : 마지막으로 임시저장한 작업코드 가져오기
git branch — set-upstream-to=remote_path/branch_name : git pull no tracking info 에러해결


markdown 문법

제목 Headers

#으로 시작하는 텍스트.
#은 하나부터 여섯개까지 쓸 수 있고, #이 늘어날때마다 제목의 수준은 내려간다.
(보통 글씨 크기가 작아진다.)



# h1
## h2
### h3
#### h4
##### h5
###### h6

h1
===

h2
—

인용 Blockquotes

>으로 시작하는 텍스트

> 인용문	
>> 인용문안의 인용문

코드 블럭 Code Blocks

``` 혹은 ~~~ 코드 첫 줄과 마지막 줄에 Back quote ( ` ) 또는 물결( ~ ) 3개 삽입


```
이것은
코드 블럭
입니다
```

~~~
이것은 
코드 블럭
입니다
~~~

인라인 코드 Inline Code Blocks
`(Back quote)로 감싸진 텍스트

`인라인 코드 블럭`

강조 Emphasis

기울여 쓰기(italic) : * 또는 _로 감싼 텍스트
굴게쓰기(bold) : ** 또는 __로 감싼 텍스트

마크다운	
*기울여쓰기(italic)*
_기울여쓰기(italic)_

**굵게쓰기(bold)**
__굵게쓰기(bold)__	기울여쓰기(italic)
기울여쓰기(italic)


수평선 Horizontal Rules

- 또는 * 또는 _ 을 3개 이상 작성
(단, -을 사용할 경우 header로 인식할 수 있으니 이 전 라인은 비워두어야한다.)

마크다운
---	
***	
___	

링크 Links
외부 링크 External Links
[링크](http://example.com "링크 제목") 인라인 링크
[링크1][1] [1]: http://example1.com/ "링크제목1" 참조 링크
<example.com/> <example@example.com> url 링크

마크다운	
인라인 링크
[Google](http://www.google.co.kr “구글”)


참조 링크 
[Google][1]
[Naver][2]
[1]: http://google.com/ “구글”
[2]: http://naver.com/ “네이버”	

URl 링크
<http://google.com/>
<example@gmail.com/>	

내부 링크 Internal (Anchored) Links
[링크](#id) 내부 링크

마크다운	
[목차](#index)	
리스트 Lists
순서 있는 리스트 Ordered Lists
No. 숫자 다음 .을 찍는다. (적힌 숫자랑 상관없이 순서대로 번호가 매겨진다.)

마크다운	
1. list item 1
1. list item 2
2. list item 3
0. list item 4
3. list item 5	

순서 없는 리스트 Unordered Lists
*, +, - 으로 시작

마크다운	
* list item 1
    * list item 1-1
    * list item 1-2

+ list item 1
    + list item 1-1
    + list item 1-2

- list item 1
    - list item 1-1
    - list item 1-2

테이블 Tables
마크다운	
테이블 생성
Header 1 | Header 2
--------- | ---------
Content 1 | Content 3
Content 2 | Content 4	

테이블 정렬
| Header 1 | Header 2 | Header 3 |
| :-------- | :--------: | --------: |
| Left | Center | Right |	

이미지 Adding Images
마크다운	실행결과
인라인 이미지
![alt text](/test.png )

링크 이미지
![alt text](image_URL)


각주 Footnotes
각주입니다[^id]
[^id]: 각주에 대한 설명.



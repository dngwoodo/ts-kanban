# ts-kanban

## 칸반 


Todo {
아이디(required),
내용(required),
완료여부(required),
카테고리(required),
태그들(optional),
}

Kanban {
아이디(required),
제목(required),
할일들: Todo[],
}


CREATE
칸반을 추가할 수 있다.
추가시 제목이 필요하다
READ
항상 칸반은 전체 조회된다.
가장 우측에는 Archive 칸반이라는 지정되지 않은 할 일 보관소가 상시 존재한다
초기에는 ID를 기반으로 칸반이 가로 정렬된다.
모든 할 일이 제거되더라도 기존 칸반이 제거되지는 않는다.
UPDATE
칸반의 가로 순서를 변경할 수 있다.
칸반의 제목을 변경할 수 있다.
칸반이 가지고 있는 할 일을 1개씩 다른 칸반으로 옮길 수 있다.
DELETE
ID를 기반으로 특정 칸반을 1개씩 삭제할 수 있다.
삭제된 칸반의 기존 할 일은 모두 Archive칸반으로 이동한다.

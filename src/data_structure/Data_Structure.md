# 자료구조

## Linked List
- 일렬로 연결된 데이터를 저장할 때 사용된다.  
- 데이터를 저장할 수 있는 공간이 있으면 그 안에 다음 데이터의 주소를 가지고 있는 구조

> 메모리 상에서의 상태

> Array List
> - 같은 엘리먼트들이 메모리상에 실제 붙어있음

> Linked List
> - 엘리먼트들이 흩어져있다. 하지만, 연결되어 있음.
![img.png](img.png)
> - `Data field`는 저장되는 값이 들어가 있는 변수필드 
> - `Link field`는 다음 노드를 가리키는 변수필드
> - `node vertex`는 노드를 뜻하고, Data와 Link가 합쳐진 형태이다.
![img_1.png](img_1.png)
> - `노드 생성 후 첫번째로 만드는 방법`
> - `Vertext temp = new Vertext(input)`으로 노드를 생성
> - `temp.next = head`로 temp의 다음 값을 현재 리스트의 첫번재 값으로 지정한다.
> - `head = temp`로 시작이 되는 노드가 우리가 생성한 temp라고 설정을 한다. 
![img_2.png](img_2.png)
> - `노드 삭제 방법`
> - `Vertex cur = head`
> - `while (--k!=0)`로 k값이 0이 아닐 때까지 반복 (k는 입력된 인덱스, 여기는 2)
> - `cur = cur.next` k가 0이 아닐때 동안 노드를 가리키는 변수 cur을 다음 노드로 이동
> - `Vertext tobedeleted = cur.next` k가 0일때, 삭제할 노드를 tobedeleted에 담음
> - `cur.next = cur.next.next`로 cur의 다음 노드를 다다음 노드로 가리킴
> > tobedeleted만이 다음노드를 알기 때문에, 이 행위가 먼저임
> - `delete tobedeleted`로 tobedeleted 삭제
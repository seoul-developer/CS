# 배열(Array)
배열은 생성 후에 크기가 고정되며, 데이터들이 연속적인 메모리 공간에 저장된다.  
인덱스를 알고 있다면 O(1)로 빠르게 해당 원소로 접근 가능하다. (random access)  
삽입 및 삭제 후, 배열의 연속적인 특성을 유지하기 위해 최대 O(n)이 소요된다.  

## 자바의 ArrayList
ArrayList는 배열의 크기가 동적으로 확장될 수 있는 자료구조이다.  
내부적으로 Object 배열을 사용하며, 디폴트 capacity는 10이다.  
새로운 요소를 추가하면서 현재 크기(size)가 capacity를 초과할 경우, 현재 capacity를 늘린다.
```
int newCapacity = oldCapacity + (oldCapacity >> 1);
```

# 연결리스트(LinkedList)
연결리스트는 노드들이 연결된 자료 구조이며, 개별 노드는 해당 데이터 값과 다음 노드를 가리키는 주소를 저장한다.  
데이터들이 연속적인 메모리 공간에 저장되지 않고 서로 떨어져 있을 수 있다.  
인덱스를 알아도 원하는 노드까지 노드를 순차적으로 타고가며 최대 O(n)으로 접근한다. (sequential access)  
특정 위치의 삽입 및 삭제는 O(1)이다. 단, 삽입, 삭제할 해당 위치를 찾기 위해 최대 O(n)의 시간이 필요하다.  

연결리스트의 종류
- 단순 연결 리스트(Singly linked list)
- 원형 연결 리스트(Circular linked list)
- 이중 연결 리스트(Doubly linked list)

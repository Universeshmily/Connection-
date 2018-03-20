# Connection-
public boolean add(Object e)
public boolean addAll(Collection c)
public void clear()
public boolean remove(object e)
public boolean removeAll(Collection c)
public boolean retainAll(Collection c)//保留在集合参数c中的元素 删除其他所有元素
public int size()
public boolean isEmpty()
public boolean contains(Object e)//对象e是否在集合中


List
List的实现类有ArrayList:实际上是元素的对象数组
            LinkedList:实际上是双向链表
            
Set
Set集合继承Collection集合其特点是采用add()方法时能判别不添加重复的元素
   其实现类有HashSet类
           TreeSet类 不仅可以禁止重复的元素，还能采用Comparable接口来判断对象的关系，除了判断对象相等还能比较对象的大小。它实现了SortedSet接口
           能够对其元素进行排序，如果对该集合中的元素进行遍历，则提供升序遍历
           通过遍历器Iterator的方法
            public Iterator iterator();//返回集合元素的遍历器对象
            
            public boolean hashNext();／／当前遍历器，如果还有未遍历的对象，则返回true
            public Object next();／／返回下一个遍历对象
            public void remove();／／删除集合中刚遍历的对象，很少使用这个方法

Map
Map是一个由关键字映射到值的对象集合，不允许键重复但允许值重复
public void clear();
pubilc Set keySet();获得所有键
public Collection values();返回集合中的所有值
public Object get(Object key);
public Object put(Object key,Object value);
public Object remove(Object key);
public int size();返回集合中键值对的数量

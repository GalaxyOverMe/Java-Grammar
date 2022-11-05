# String [] -> List&lt;String>
```
String [] array = {"1", "2", "3"};
List<String> list = Arrays.asList(array);
```
# List&lt;String> -> String []
```
List<String> list = Arrays.asList("1", "2", "3");
String[] array = list.toArray(new String[0]);
```
# int [] -> List &lt;Integer>
```
int[] array = {1, 2, 3};
List<Integer> list = Arrays.stream(array).boxed().toList();
```
# List&lt;Integer> -> int []
```
List<Integer> list = new ArrayList(Arrays.asList(1, 2, 3));
int[] array = list.stream().mapToInt(i->i).toArray();
```
# int [] -> Integer []
```
int [] intArray = {1, 2, 3};
Integer [] IntArray = Arrays.stream(intArray).boxed().toArray(Integer[]::new);
```
# Integer [] -> int []
```
Integer [] IntArray = {1, 2, 3};
int [] intArray = Arrays.stream(IntArray).mapToInt(i->i).toArray();
```


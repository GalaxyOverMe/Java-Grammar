# String [] -> List&lt;String>
<pre>
String [] array = {"1", "2", "3"};
List&ltString> list = Arrays.asList(array);
</pre>
# List&lt;String> -> String []
<pre>
List&ltString> list = Arrays.asList("1", "2", "3");
String [] array = list.toArray(new String[0]);
</pre>
# int [] -> List &lt;Integer>
<pre>
int [] array = {1, 2, 3};
List&ltInteger> list = Arrays.stream(array).boxed().toList();
</pre>
# List&lt;Integer> -> int []
<pre>
List&ltInteger> list = new ArrayList<>(Arrays.asList(1, 2, 3));
int [] array = list.stream().mapToInt(i->i).toArray();
</pre>
# int [] -> Integer []
<pre>
int [] intArray = {1, 2, 3};
Integer [] IntArray = Arrays.stream(intArray).boxed().toArray(Integer[]::new);
</pre>
# Integer [] -> int []
<pre>
Integer [] IntArray = {1, 2, 3};
int [] intArray = Arrays.stream(IntArray).mapToInt(i->i).toArray();
</pre>


# String [] -> List&lt;String>
<pre>
String [] sArray = {"1", "2", "3"};
List&ltString>  sList = Arrays.asList(sArray);
</pre>
# List&lt;String> -> String []
<pre>
List&ltString> sList = new ArrayList<>(Arrays.asList("1", "2", "3"));
String [] sArray = sList.toArray(new String[0]);
</pre>
# int [] -> List &lt;Integer>
<pre>
int [] intArray = {3, 2, 1};
List&ltInteger> IntList = Arrays.stream(intArray).boxed().toList();
</pre>
# List&lt;Integer> -> int []
<pre>
List&ltInteger> IntList = new ArrayList<>(Arrays.asList(3, 2, 1));
int [] intArray = IntList.stream().mapToInt(i->i).toArray();
</pre>
# int [] -> Integer []
<pre>
int [] intArray = {3, 2, 1};
Integer [] IntArray = Arrays.stream(intArray).boxed().toArray(Integer[]::new);
</pre>
# Integer [] -> int []
<pre>
Integer [] IntArray = {3, 2 ,1};
int [] intArray = Arrays.stream(IntArray).mapToInt(i->i).toArray();
</pre>


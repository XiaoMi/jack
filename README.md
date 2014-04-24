What is JACK
=============

JACK是一个粘合zookeeper与thrift的框架，可以简单地让你的thrift server更简单地做到高可用。

开源计划
---------

 代码还在整理中，将尽快开源。

原理
----

<pre><code>

        |  thrift cluster service/TCP |
        |_____________________________|
        |          |        |         |
        |  JACK    |  JACK  |  JACK   |
        |__________|________|_________|
        |          |        |         |
        |  JACK    |   ZK   |  JACK   |
        |__________|________|_________|
        |          |        |         |
        |  JACK    |  JACK  |  JACK   |
        |__________|________|_________|

</code></pre>



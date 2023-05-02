Download Link: https://assignmentchef.com/product/solved-coen79-homework-4
<br>
<ol>

 <li>The node class is defined as follows:</li>

</ol>




<ol>

 <li><strong>class</strong> node {</li>

 <li><strong>public</strong>: // TYPEDEF</li>

 <li>typedef <strong>double</strong> value_type;</li>

 <li>// CONSTRUCTOR</li>

 <li>node(<strong>const</strong> value_type&amp; init_data = value_type(), node* init_link = NULL) {</li>

 <li>data_field = init_data;               link_field = init_link;  }  9.</li>

 <li>// Member functions to set the data and link fields:</li>

 <li><strong>void</strong> set_data(<strong>const</strong> value_type&amp; new_data) { data_field = new_data; }       <strong>void</strong> set_link(node* new_link) { link_field = new_link;  }</li>

 <li></li>

 <li>// Constant member function to retrieve the current data:  15.     value_type data() <strong>const</strong> { <strong>return</strong> data_field; }</li>

 <li></li>

 <li>// Two slightly different member functions to retreive the current link:</li>

 <li><strong>const</strong> node* link() <strong>const</strong> { <strong>return</strong> link_field; }       node* link() { <strong>return</strong> link_field; }</li>

 <li></li>

 <li><strong>private</strong>:</li>

 <li>value_type data_field;</li>

 <li>node* link_field;</li>

 <li>};</li>

</ol>




Implement the following function. (Note: <em>No toolkit function is available</em>. Only the node class is available.)




<ol>

 <li><strong>void</strong> list_copy (<strong>const</strong> node* source_ptr, node*&amp; head_ptr, node*&amp; tail_ptr) 2. // Precondition: source_ptr is the head pointer of a linked list.</li>

 <li>// Postcondition: head_ptr and tail_ptr are the head and tail pointers for a new list that</li>

 <li>// contains the same items as the list pointed to by source_ptr</li>

 <li>{</li>

</ol>




<ol start="2">

 <li>Please justify why the linked list toolkit functions are not member functions of the node class?</li>

</ol>














































<ol start="3">

 <li>In the following function, why cursor has been declared as a const variable? What happens if you change it to a non-const variable?</li>

</ol>




<ol>

 <li>size_t list_length (<strong>const</strong> node* head_ptr)</li>

 <li>// Precondition: head_ptr is the head pointer of a linked list.</li>

 <li>// Postcondition: The value returned is the number of nodes in the // linked list.</li>

 <li>{</li>

 <li>const<strong> node* cursor; </strong><strong> </strong></li>

 <li>size_t answer;</li>

 <li>answer = 0;</li>

 <li><strong>for</strong> (cursor = head_ptr; cursor != NULL; cursor = cursor – &gt; link())</li>

 <li>++answer;</li>

 <li><strong>return</strong> answer;</li>

 <li>}</li>

</ol>










<ol start="4">

 <li>We are interested in implemented the back and forward arrow functionality in a mobile app. When back arrow is touched, the previous screen is shown, and when forward arrow is pressed (if applicable), then the forward screen is shown. Please justify what type of data structure you would use.</li>

</ol>




























<ol start="5">

 <li>Why does our node class have two versions of the link member function?

  <ol>

   <li>One is public, the other is private.</li>

   <li>One is to use with a const pointer, the other with a regular pointer.</li>

   <li>One returns the forward link, the other returns the backward link.</li>

   <li>One returns the data, the other returns a pointer to the next node.</li>

  </ol></li>

</ol>
















<ol start="6">

 <li>What are the <em>iterator invalidation rules</em> for a data structure that stores items in a <em>linked list</em>?</li>

</ol>




























<ol start="7">

 <li>What are <em>the iterator invalidation rules</em> for STL’s vector class?</li>

</ol>


































<ol start="8">

 <li>What are the features of a <em>random access iterator</em>? Present the name of two STL data structures that offer random access iterators.</li>

</ol>








































<ol start="9">

 <li>The bag class is defined as follows:</li>

</ol>













<ul>

 <li>This class implements the following functions to create iterators:</li>

</ul>



















<ul>

 <li>Please complete the implementation of the following iterator:</li>

</ul>






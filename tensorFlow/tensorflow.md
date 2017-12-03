### [Tensorflow](https://www.tensorflow.org/programmers_guide/tensors)


#### [For noobs](https://www.tensorflow.org/get_started/get_started)
* The central unit of data in TensorFlow is the tensor. A tensor consists of a set of primitive values shaped into an array of any number of dimensions. A tensor's rank is its number of dimensions.
* TensorFlow provides a utility called TensorBoard that can display a picture of the computational graph.
* A graph can be parameterized to accept external inputs, known as placeholders. A placeholder is a promise to provide a value later.
* Building the graph and running the graph.
* A computational graph is a series of TensorFlow operations arranged into a graph of nodes. 
* To actually evaluate the nodes, we must run the computational graph within a session. A session encapsulates the control and state of the TensorFlow runtime.
* Build more complicated computations by combining Tensor nodes with operations (Operations are also nodes)
* A graph can be parameterized to accept external inputs, known as placeholders. A placeholder is a promise to provide a value later.
* Variables allow us to add trainable parameters to a graph. They are constructed with a type and initial value
* To initialize all the variables in a TensorFlow program, you must explicitly call a special operation as follows:
> init = tf.global_variables_initializer()
> sess.run(init)
* 

##### tf.train API



* TensorFlow, as the name indicates, is a framework to define and run computations involving tensors. A tensor is a generalization of vectors and matrices to potentially higher dimensions. Internally, TensorFlow represents tensors as n-dimensional arrays of base datatypes.

* Each element in the Tensor has the same data type, and the data type is always known. The shape (that is, the number of dimensions it has and the size of each dimension) might be only partially known. Most operations produce tensors of fully-known shapes if the shapes of their inputs are also fully known, but in some cases it's only possible to find the shape of a tensor at graph execution time.

* Each element in the Tensor has the same data type, and the data type is always known. The shape (that is, the number of dimensions it has and the size of each dimension) might be only partially known. Most operations produce tensors of fully-known shapes if the shapes of their inputs are also fully known, but in some cases it's only possible to find the shape of a tensor at graph execution time.

* The rank of a tf.Tensor object is its number of dimensions. Synonyms for rank include order or degree or n-dimension. Note that rank in TensorFlow is not the same as matrix rank in mathematics. As the following table shows, each rank in TensorFlow corresponds to a different mathematical entity:

* The shape of a tensor is the number of elements in each dimension. TensorFlow automatically infers shapes during graph construction. These inferred shapes might have known or unknown rank. If the rank is known, the sizes of each dimension might be known or unknown.

* There are two ways of accessing the shape of a tf.Tensor. While building the graph, it is often useful to ask what is already known about a tensor's shape. This can be done by reading the shape property of a tf.Tensor object. This method returns a TensorShape object, which is a convenient way of representing partially-specified shapes (since, when building the graph, not all shapes will be fully known).

* It is also possible to get a tf.Tensor that will represent the fully-defined shape of another tf.Tensor at runtime. This is done by calling the tf.shape operation. This way, you can build a graph that manipulates the shapes of tensors by building other tensors that depend on the dynamic shape of the input tf.Tensor.

* The shape of a tensor is the number of elements in each dimension. TensorFlow automatically infers shapes during graph construction. These inferred shapes might have known or unknown rank. If the rank is known, the sizes of each dimension might be known or unknown.

* Once the computation graph has been built, you can run the computation that produces a particular tf.Tensor and fetch the value assigned to it. This is often useful for debugging as well as being required for much of TensorFlow to work.

* Tensor.eval returns a numpy array with the same contents as the tensor.


#### Links
2. 

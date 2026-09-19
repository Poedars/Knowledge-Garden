1.medical projects

Notes:
1.Attention is a communication mechanism. can be seen as nodes in a directed graph looking at each other and aggregating the information via a weighted sum from all the nodes that point to it,with data-dependent weights

2.There is no notion of space so attention simply acts over like a set of vectors in this graph. so these nodes have no idea where they are positioned in the space, and that's why we need to encode them positionally and give them some information that is anchored to a specific position so that they know where they are.

3.Each example across batch dimension is of course processed completely independtly and never "talk" to each other.

4.In an "encoder" attention block just delete the single line that does masking with tril,allowing all tokens to communicate. here is called a "decoder" attention block because it has triangular masking, and is usually used in autoregressive settings,

5."self-attention" just means that the keys and values are produced from the same source as queries. In "cross-attention",the query get produced from x, but the keys and values come from some other,external source(e.g. an encoder module)
# Literature Review: Discrete Mathematics Concepts in Programming Languages and LLMs
Kevin Huang
## Overview

This literature review explores the intersection of discrete mathematics and programming languages, focusing on how concepts from discrete mathematics, such as formal languages and combinatorics, are applied in the context of programming languages and large language models (LLMs). The review addresses the roles of tokenization, formal languages, and recursive relations in both fields.

## References

- **Chomsky, N. (1956).** *Three Models for the Description of Language*. IRE Transactions on Information Theory, 2(3), 113-124.
- **Sennrich, R., Haddow, B., & Birch, A. (2016).** *Neural Machine Translation of Rare Words with Subword Units*. Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (ACL 2016), 1715-1725.
- **Aho, Alfred V. "Teaching the compilers course." ACM SIGCSE Bulletin 40.4 (2008): 6-8.
- **Hopcroft, J. E., Motwani, R., & Ullman, J. D. (2001).** *Introduction to Automata Theory, Languages, and Computation (2nd ed.)*. Addison-Wesley.


## Relevant Concepts

- [Formal Languages](https://en.wikipedia.org/wiki/Formal_language)
- [Tokenization](https://en.wikipedia.org/wiki/Tokenization_(data_security))
- [Combinatorics](https://en.wikipedia.org/wiki/Combinatorics)
- [Recurrence Relations](https://en.wikipedia.org/wiki/Recurrence_relation)
- [Automata Theory](https://en.wikipedia.org/wiki/Automata_theory)
- [Graph Theory](https://en.wikipedia.org/wiki/Graph_theory)
- [Set Theory](https://en.wikipedia.org/wiki/Set_theory)

## Formal Languages

## Tokenization

## Questions and Answers

### Question 1: Outlining the Presence of Discrete Mathematics in LLMs

**How does formal languages (and other discrete math concepts) relate to GPT's LLM tokenization process?**

- **Formal Languages and Tokenization**: Formal languages are used to define the rules for tokenization. Tokenization involves breaking down text into tokens based on these rules, similar to how formal grammars define valid sequences of symbols.
  - *Reference*: Chomsky, N. (1956). *Three Models for the Description of Language*. IRE Transactions on Information Theory, 2(3), 113-124.
- **Tokenization**: GPT’s tokenizer, based on Byte Pair Encoding (BPE), converts natural language into tokens by splitting text into frequently occurring subwords. This process is influenced by combinatorial principles to balance vocabulary size and represent diverse texts.
  - *Reference*: Sennrich, R., Haddow, B., & Birch, A. (2016). *Neural Machine Translation of Rare Words with Subword Units*. Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (ACL 2016), 1715-1725.
- **Combinatorics and Token Vocabulary**: Combinatorics helps in understanding the structure of the token vocabulary and the infinite number of possible token sequences that can be represented.

### Question 2: Outlining the Presence of Discrete Mathematics in Programming Languages

**How does formal languages and tokenization show up in programming languages?**

- **Formal Languages in Programming Languages**: Programming languages are formal languages with specific alphabets and grammars. The syntax and structure of programming languages are defined by formal rules.
- **Tokenization in Programming Languages**: Tokenization breaks source code into meaningful units like keywords, operators, and literals. Regular expressions are used to define patterns for these tokens.
- **Parsing and Abstract Syntax Trees (ASTs)**: After tokenization, parsing analyzes token sequences according to the language’s grammar, generating an abstract syntax tree (AST) that represents the hierarchical structure of the code.

### Question 3: Diving Deeper into Tokenization in Both LLMs and Programming Languages

**How does a compiler or LLM know that a token is valid in their vocabulary? How is this related to discrete math sets and recursive relations?**

- **Compilers**: Compilers use lexical analysis to validate tokens against a predefined set of valid tokens. Unknown tokens trigger error reporting and recovery strategies, and recursive parsing strategies are used for managing syntax errors.
  - *Reference*: Aho, A. V., Lam, M. S., Sethi, R., & Ullman, J. D. (2006). *Compilers: Principles, Techniques, and Tools (2nd ed.)*. Addison-Wesley.
- **LLMs**: LLMs handle unknown tokens by breaking them into known subword units or using special tokens. Techniques like BPE involve recursive merging of subwords to build a vocabulary that can effectively handle unknown tokens.
- **Discrete Math Sets and Recursive Relations**: In both cases, discrete mathematics concepts like sets are used to define token vocabularies, and recursive relations play a role in managing and representing complex token structures.

### Question 4: How do concepts of automata theory apply to the design and functioning of LLMs and compilers?

**Automata Theory in Compilers**

Automata theory, particularly finite automata, is foundational in the design and implementation of compilers. Here’s how it applies:

1. **Lexical Analysis**
   - **Finite Automata**: In lexical analysis, finite automata are used to implement lexical analyzers or scanners. These automata recognize patterns in the source code (like keywords, operators, and identifiers) and help in tokenizing the input text. Regular expressions used in defining tokens are typically converted into finite automata for efficient pattern matching.
   - **Deterministic Finite Automata (DFA)**: For each regular expression pattern, a DFA can be constructed to recognize valid sequences of characters. The lexical analyzer uses this DFA to scan through the source code, identifying tokens and their types.

**Automata Theory in LLMs**

While LLMs use more complex models compared to traditional automata, automata theory still influences their design and functioning:

1. **Tokenization**
   - **Finite State Machines**: Tokenization in LLMs often involves finite state machines to handle text segmentation and normalization. These machines process sequences of characters into tokens, such as splitting text into words or subwords.
     - *Reference*: Hopcroft, J. E., Motwani, R., & Ullman, J. D. (2001). *Introduction to Automata Theory, Languages, and Computation (2nd ed.)*. Addison-Wesley.
   - **Byte Pair Encoding (BPE)**: The BPE algorithm used in tokenization can be understood in terms of automata theory as it builds a vocabulary based on frequent patterns, akin to constructing a finite automaton for pattern recognition.

2. **Language Modeling**
   - **N-grams and Finite State Models**: In simpler language models, n-gram models (which can be represented as finite state machines) are used to predict the next word based on the previous n-1 words. While modern LLMs like GPT use more complex neural architectures, the foundational idea of modeling sequences can be traced back to finite state models.
   - **Sequence Modeling**: The principles of automata theory, especially regarding sequences and transitions, influence how LLMs process and predict sequences of text.

3. **Parsing and Understanding**
   - **Grammar Induction**: Techniques for inducing grammars from data can be informed by automata theory, especially in understanding how sequences are structured and how rules can be derived.

### Question 5: How are graph theory concepts used in the optimization of neural network architectures and compiler design?

**Graph Theory in Neural Network Optimization**

1. **Neural Architecture Search (NAS)**
   - **Search Space as a Graph**: In Neural Architecture Search (NAS), the search space of possible architectures is represented as a graph. Each node represents a specific architecture configuration, and edges represent possible transitions between configurations. Graph-based search algorithms explore this space efficiently to find optimal architectures.
   - **Optimization via Graph Traversal**: Graph traversal techniques (e.g., breadth-first search, depth-first search) and algorithms like evolutionary search or reinforcement learning are used to optimize the neural network structure by exploring different topologies and configurations.

2. **Graph-Based Pruning and Compression**
   - **Pruning Networks**: Graph theory is applied to prune unnecessary nodes (neurons) and edges (connections) from neural networks. Pruning reduces the number of parameters, improving both inference speed and memory usage. This can be achieved by analyzing the connectivity patterns and removing redundant or less important components.
   - **Graph Partitioning**: When training large neural networks across multiple devices, graph partitioning algorithms divide the network into smaller subgraphs. These subgraphs can be processed in parallel, improving efficiency and reducing communication overhead between devices.

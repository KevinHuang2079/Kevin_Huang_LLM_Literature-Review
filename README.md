Literature Review: Discrete Mathematics Concepts in Programming Languages and LLMs
Overview
This literature review explores the intersection of discrete mathematics and programming languages, with a focus on how concepts from discrete mathematics, such as formal languages and combinatorics, are applied in the context of programming languages and large language models (LLMs). The review addresses the role of tokenization, formal languages, and recursive relations in both fields.

Relevant Concepts
Formal Languages: Formal languages consist of sets of strings defined by rules of a formal grammar. In both programming languages and LLMs, formal languages are used to define valid sequences of symbols or tokens.
Tokenization: Tokenization is the process of breaking down text or code into smaller, meaningful units called tokens. This process is critical in converting natural language or source code into a format that can be processed by models or compilers.
Combinatorics: This branch of discrete mathematics helps in understanding the structure of token vocabularies and the possible sequences or combinations of tokens.
Recursive Relations: Recursive relations and parsing strategies are used in both programming languages and LLMs to handle complex syntactic structures and unknown tokens.
Questions and Answers
Question 1: Outlining the Presence of Discrete Mathematics in LLMs
How does formal languages (and other discrete math concepts) relate to GPT's LLM tokenization process?

GPT-4:

Formal Languages and Tokenization: Formal languages are used to define the rules for tokenization. Tokenization involves breaking down text into tokens based on these rules, similar to how formal grammars define valid sequences of symbols.
Tokenization: GPT’s tokenizer, based on byte pair encoding (BPE), converts natural language into tokens by splitting text into frequently occurring subwords. This process is influenced by combinatorial principles to balance vocabulary size and represent diverse texts.
Combinatorics and Token Vocabulary: Combinatorics helps in understanding the structure of the token vocabulary and the infinite number of possible token sequences that can be represented.
Question 2: Outlining the Presence of Discrete Mathematics in Programming Languages
How does formal languages and tokenization show up in programming languages?

GPT-4:

Formal Languages in Programming Languages: Programming languages are formal languages with specific alphabets and grammars. The syntax and structure of programming languages are defined by formal rules.
Tokenization in Programming Languages: Tokenization breaks source code into meaningful units like keywords, operators, and literals. Regular expressions are used to define patterns for these tokens.
Parsing and Abstract Syntax Trees (ASTs): After tokenization, parsing analyzes token sequences according to the language’s grammar, generating an abstract syntax tree (AST) that represents the hierarchical structure of the code.
Question 3: Diving Deeper into Tokenization in Both LLMs and Programming Languages
How does a compiler or LLM know that a token is valid in their vocabulary? How is this related to discrete math sets and recursive relations?

GPT-4:

Compilers: Compilers use lexical analysis to validate tokens against a predefined set of valid tokens. Unknown tokens trigger error reporting and recovery strategies, and recursive parsing strategies are used for managing syntax errors.
LLMs: LLMs handle unknown tokens by breaking them into known subword units or using special tokens. Techniques like BPE involve recursive merging of subwords to build a vocabulary that can effectively handle unknown tokens.
Discrete Math Sets and Recursive Relations: In both cases, discrete mathematics concepts like sets are used to define token vocabularies, and recursive relations play a role in managing and representing complex token structures.

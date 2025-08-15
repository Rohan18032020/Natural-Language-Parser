# Natural Language Parser

This Python project implements a natural language parser using NLTK (Natural Language Toolkit) for processing and analyzing sentences based on a predefined context-free grammar (CFG). The parser can identify noun phrase chunks in sentences and generate parse trees for syntactic analysis.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/AKKI0511/Natural-Language-Parser.git
   cd Natural-Language-Parser
   ```

2. Run the parser:

   ```bash
   python parse_sentence.py "Your sentence.txt here."
   ```

   Replace `"Your sentence.txt here."` with the text file you want to parse.

## Grammar Rules

The grammar for parsing sentences includes terminals (words) and nonterminals (syntactic categories). Here are some examples:

- Terminals (words): "country," "smile," "in," "red," etc.
- Nonterminals (syntactic categories): `S` (sentence), `NP` (noun phrase), `VP` (verb phrase), `N` (noun), `V` (verb), etc.

## Sentence Parsing

The parser processes input sentences by tokenizing them into words, converting to lowercase, and filtering out non-alphabetic words. It then attempts to parse the sentence using a context-free grammar.

## Functions

- `preprocess(sentence)`: Pre-processes the input sentence by converting to lowercase and filtering out non-alphabetic words.
- `np_chunk(tree)`: Identifies noun phrase chunks in the parse tree.
- `main()`: Reads input sentence and performs parsing and noun phrase chunking.

## Dependencies

- NLTK (Natural Language Toolkit)

Install NLTK and download required resources using:

```bash
pip install nltk
python -m nltk.downloader punkt
```

## Output

The parser prints the parse trees for the input sentence and identifies noun phrase chunks within the trees.
`Example Output`:

![image](https://github.com/AKKI0511/Natural-Language-Parser/assets/120317569/e89168a3-5a70-44d2-a77b-735fbdc35e33)

## Acknowledgements

This project uses NLTK's parsing capabilities and demonstrates how to analyze sentence structure and identify noun phrase chunks in natural language sentences.

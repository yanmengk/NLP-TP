## Speech and Language Processing 3rd edition Learning Notes

### Chapter-2：Regular Expressions, Text Normalization, Edit Distance

**ELIZA**: an early natural language processing system that could carry on a limited conversation with a user by imitating the responses of a Rogerian psychotherapist[^1];**pattern-based method**。

**text normalization**: normalizing text means converting it to a more convenient, standard form.

- tokenization[^2]

lemmatization：determining that two words have the same root, despite their surface differences.

 + stemming：refers to a simpler version of lemmatization in which we mainly just strip sufﬁxes from the end of the word.
 + sentence segmentation

**edit distance**: measures how similar two strings are based on the number of edits (insertions, deletions, substitutions). Edit distance is an algorithm with applications throughout language processing, from spelling correction to speech recognition to coreference resolution.

#### Regular expressions

**Regular experssion**: Formally, a regular expression is an algebraic notation for characterizing a set of strings.

Basic operations in regular expressions include concatenation of symbols, disjunction of symbols ([], |, and .), counters (*, +, and {n,m}), anchors (ˆ, $) and precedence operators ((,)).



#### Words

**Word type**: Types are the number of distinct words in a corpus.

**Word token**: Tokens are the total number N of running words.



#### Corpora

Perhaps the most important dimension of variation is the language. 

Another dimension of variation is the genre.

And ﬁnally, time matters too.



#### Text normalization

At least three tasks are commonly applied as part of any normalization process:

1. Segmenting/tokenizing words from running text
2. Normalizing word formats(Lemmatization and Stemming)
3. Segmenting sentences in running text.

**Lemmatization** algorithms can be complex. For this reason we sometimes make use of a simpler but cruder method, which mainly consists of chopping off word-ﬁnal afﬁxes. This naive version of morphological analysis is called **stemming**.



#### Minimum edit distance

**the minimum edit distance** between two strings is deﬁned as the minimum number of editing operations (operations like insertion, deletion, substitution) needed to transform one string into another.

**The Levenshtein distance** between two sequences is the simplest weighting factor in which each of the three operations has a cost of 1. Levenshtein also proposed an alternative version of his metric in which each insertion or deletion has a cost of 1 and substitutions are not allowed. (This is equivalent to allowing substitution, but giving each substitution a cost of 2 since any substitution can be represented by one insertion and one deletion).

Knowing the minimum edit distance is useful for algorithms like ﬁnding potential spelling error corrections. It can also provide the minimum cost alignment between two strings.







------



[^1]: 精神、心理治疗师
[^2]: 分词




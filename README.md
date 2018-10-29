# Language-Detection
This system automatically detects language of a web-page using Improved N-Gram algorithm.   

# ABSTRACT
Language identification is predominantly used in numerous NLP systems as a seeding step to determine the language in which a web page is written. A huge amount of work has already been done in this area. This paper uses N-Gram approach to detect the language of a web page and uses WiLi-2018 (Wikipedia Language Identification dataset) [4] to detect the content of the text of European languages, in which they are inscribed.

# Keywords
Language Detection, Language Identification, Natural Language Processing, N-Grams.

# INTRODUCTION
The basis of this paper comes under the category of identification of European languages using WiLI 2018 dataset. Language detection can be achieved using Computational or Non-Computational technique. Statistical approaches can be divided into training and testing steps. In train step dataset is taken and corpus is created using feature extraction while in Classification step similarity between the training and the testing language profile is estimated and the most alike language is returned as the language of the given text. Non-Computational techniques require extensive knowledge about the particular language in advance, such as the character combinations, most frequent words used, etc. This paper uses n-gram approach, a statistical technique to detect the language of a given web page.
N-gram is a probabilistic language model which is used to detect the item in a sequence in the form of (n-1) Markov model. N-grams [2] typically refer to the sequence of words. A unigram is one word, a bi-gram is a progression of two words, a tri-gram is a sequence of three words. [3] One important point to consider is that the items within n-gram may not necessarily have any kind of relationship between them apart from the certainty that the word appears next to one another.

# RELATED WORK
Cavnar and Trenkle Approach [2]
Cavnar and Trenkle (1994) used N-Gram based distance measure to accurately categorize the small documents and news articles. Distance measure was calculated between the language profile of training set data and the target document. This approach was 
primarily dedicated only towards the languages directly representable in ASCII.

## Suzuki Algorithm [3]
Suzuki (2002) taken into account two predetermined values UB and LB to check the response of identification on the target text. Matching rate, a list of shift codons was calculated using Tri-Grams and compared to shift codons of the training set and the language for which the matching rate of training text is higher than the UB was assumed to be the target texts’ language. This method was able to identify English, German, Portuguese and Romanian languages with high accuracy.

## Language Identification of Web Pages [5] 
In Bruno Martins (2005), automatic language identification of a given web page was achieved using the N-gram based algorithm and complemented it with a more efficient similarity measure and heuristics to handle the web pages in a better way. In this approach 23 different language models were constructed and tested upon 12 different languages, like, Danish, Dutch, English, French, German achieving an accuracy of 91.25%.

## Language Identification of Web Pages Based on Improved N-gram Algorithm [6]
Choong et al. (2011) proposed a two-step process. Tri-Grams were used in combination with two heuristics namely byte-sequence HTML parsing and HTML character translation of web pages to obtain an accuracy of 94.04% for non-Latin (Asian and African) languages.

## Graph-Based N-Gram Approach [8]
In Erik Tromp (2011), graph-based N-Gram approach was proposed for short and ill-written texts. A graph model was developed to predict the language of a text referencing to some previously unseen text. This approach was not applicable to multilingual documents.

## The WiLI Benchmark Dataset for Written Language Identification [4]
In Martin Thoma(2018), open source dataset of short text extracts for 235 languages has been explained. It is a well-balanced 
classification dataset (with test–train split) that can be effectively used for language identification techniques.


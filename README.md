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

# METHODOLOGY
The approach presented by Choong et al [6] for N-gram generation only considered Tri-Grams for the detection of languages. Moreover, it typically focuses on Non-latin(Asian and African) languages. In our approach, we have considered Mono, Bi and Tri-Grams and tried to extend the N-gram approach to identify the European languages or Latin languages precisely.

A typical language identification system calculates language profiles from training texts of various language schemes using N-Grams(Figure-1). In a similar manner, the language profile for the target text is generated. The system then evaluates the matching rates of N-Grams between training and target profile. The matching rate is calculated as the average of match factors(mi) whenever an N-gram in target profile matched with a N-gram in the training corpus. Then the language with the highest match rate is returned as the language of a target web page given that the match rate is not lesser than the lower bound(LB). We have taken the value of LB as 0.5.
This paper uses the updated version of the famous WiLI-2018 dataset [4]. WiLI-2018 benchmark dataset is created from Wikipedia web pages written in multiple languages and publicly available. The dataset consists of a total of 235 languages and more than 0.1M web pages of different languages. We have targeted 34 European Languages amounting to 18000 web pages from this dataset.


# RESULTS AND DISCUSSION
https://github.com/tausy/language-detection-n-gram/blob/master/ML_Research_Assignment2.pdf


## REFERENCES

[1] Ali Selamat , Nicholas Akosu.Word length algorithm for language identification of under-resourced languages.
    
[2] W. B. Cavnar and J. M. Trenkle. N-gram-based text categorization. In Proceedings of SDAIR-94, the 3rd Annual Symposium on     Document Analysis and Information Retrieval, pages 161.175, Las Vegas, Nevada, U.S.A 1994.

[3] Izumi Suzuki, Yoshiki Mikami, Ario Ohsato, Yoshihide Chubachi. "A language and character set determination method based on     N-gram statistics." ACM Transactions on Asian Language Information Processing (TALIP), 2002: 269-278.

[4] Martin Thoma, The WiLI benchmark dataset for written language identification arXiv:1801.07779v1 [cs.CV] 23 Jan 2018
    
[5] Bruno Martins, Mário J. Silva. Language identification in web pages. 2005 ACM symposium on Applied computing Santa Fe: ACM     New York, NY, USA, 2005.76-768.

[6] Yew Choong Chew, Yoshiki Mikami, Robin Lee Nagano, Language Identification of Web Pages Based on Improved N-Gram Algorithm     IJCSI International Journal of Computer Science issues, Vol. 8, Issue 3, No. 1, May 2011 ISSN (Online): 1694-0814        
    www.IJCSI.org.
    
[7] Chew Y. Choong,Yoshiki Mikami, C. A. Marasinghe and S.T. Nandasara. Optimizing n-gram Orderof an n-gram Based Language         Identification Algorithm for 68 Written Languages. The International Journal on Advances in ICT for Emerging Regions 2009     02 (02) : 21 - 28.

[8] Erik Tromp, Mykola Pechenizkiy. Graph-Based N-gram Language Identification on Short Texts. Department of Computer Science,     Eindhoven University of Technology P.O. Box 513, 5600 MB, Eindhoven, The Netherlands.

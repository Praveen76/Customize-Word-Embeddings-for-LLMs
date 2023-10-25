# Customize-Word-Embeddings-for-LLMs



Problem definition:
We'll use NQ (Natural Questions) dataset from the Google.


# **Data:**
The Natural Questions corpus represents a question-answering dataset, comprising 307,373 training examples, 7,830 development examples, and 7,842 test examples. Each instance consists of a query originating from google.com and an associated Wikipedia page. Within each Wikipedia page, there is an annotated passage, often referred to as the "long answer," which serves as a potential response to the query. Additionally, one or more short spans from this annotated passage contain the actual answer to the query. However, it is important to note that the long and short answer annotations may be left empty. When both the long and short answer annotations are empty, it indicates that no answer is available on the page. If the long answer annotation is non-empty but the short answer annotation remains empty, it suggests that the annotated passage provides a response to the question, yet no explicit short answer can be identified. Lastly, approximately 1% of the documents include a passage annotated with a short answer of "yes" or "no" instead of a list of short spans.




* 1. Data prep
    * transforming prepared data
      * negative sampling
        * i. Weak Negatives
        * ii. Hard Negatives

* 2. Word Embeddings:
    * How to get embeddings
    * Visualizing Embeddings
      * Queries and Passages in Latent Space

* 3. Model Training:
  * motivating example
  * performance before training
    * training
      * Training setup explanation
      * Explaining the 'Model' being trained
        
* 4. Model performance after training
  * visualizing before/after
    * Queries and Passages in Latent Space

# MovieSentimentClassification 📺
About **movie sentiment classification**: Trained a simple RNN model on 'transformer generated embeddings. 

## Summary
- The dataset used was [IMDB Review](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews), which is a balanced dataset comprising of **~50k** movie reviews.
**Note**: The encoder generated embeddings through its self text cleaning mechanisms. 
- The dataset was transformed into meaningful word embeddings of `(384, )` dimensions using `SetenceTransformer`'s `all-MiniLM-L6-v2` (which is a distilled version of `BERT`), then partitioned into training and test sets.
- A `SimpleRNN` architecture was used with `Drouput` layers at rate **0.2**.
- The model was trained for 50 epochs.

## Conclusion
- The accuracy achieved was **~90%**, along with `val_accuracy` **~82%**
- The model can be found live [here](https://abhinandan12345-simplemoviesentimentpredictor.hf.space/?__theme=system&deep_link=MfRyFAgZHP4). 

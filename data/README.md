# Download

The origional package can be downloaded by hand from [Kaggle](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge).
The origional bill text _can_ be downloaded by hand from [congress.gov](https://www.congress.gov).
For convience, we keep a 2nd copy of all the data gzip'ed in [releases][releases].
We need to source the data localy for everyone because GitHub has storage limits that we don't want to cross.

## Steps

1. Retrieve the dataset _by hand_.
   Click on the [download](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge/download) link, saving the file to `~/data/raw`
2. Extract the data in-place
   1. right click the file, select '7-zip', select 'Extract Here'
3. Extract the meta-data.
   [Code instructions](../code/README.md) (script 1)
3. Convert the raw JSON files into the nomal folder corpus format.
   [Code instructions](../code/README.md) (script 2)


## Shortcuts

[GitHub](https://github.com) has some issues when dealing with [large files](https://help.github.com/en/articles/working-with-large-files).
The [recomended method](https://help.github.com/en/articles/distributing-large-binaries) for dealing with large files is to store them in [releases][releases].
You can find the gzip'ed versions of the below there.
Any of the steps can be skipped by downloading the correct file from [releases][releases] and proceding from that point forward.

[releases]: https://github.com/HarrisburgUniversityPhd/VoteAnalysis/releases

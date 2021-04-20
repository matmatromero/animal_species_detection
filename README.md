# Call of the Forest: Detection of Animal Species in Tropical Soundscapes
by: Dennis Diego, Jason Dolorso, Cymon Marcaida, and Matmat Romero

## Executive Summary

The presence or absence of certain animal species in an environment indicates the health of the ecosystem. It is one measurement, among many others of how human activities impact our natural environment. We can look back to the United States in the 1950s where the constructions of canals and levees atlerted the flow of water in the everglades which caused negative impact to the environment. This resulted to an anual decline of wading birds nesting in the area due to the dwindling population of prey.

Identifying the presence or absence of bird species in an area is one of the ingishgtful measure of environmental impact. Unfortulately in most cases, hearing the sound of the birds are easier than seeing them. This is especially true on dense forests where the horizon is covered by the thick canopies of trees and the forest trail is full of leaves, branches, and tall grasses which makes it hard for humans to traverse. With these challenges in specie identification in tropical rainforests, we look into the capabilities of audio identification to identify the species. Specifically we want to know how can we determine the biodiversity of a rainforest by classifying the sounds of the species that are heard in the forest audio recording?

Using data from an ongoing kaggle competition whose goal is to identify 24 birds and frog species using audio files, we cleaned and processed data using amazon web service architecture and dask library to handle large amount of data. From the audio files, we generated a mel spectrogram image of the a specific animal specie in the audio recording which we then used as input to our deep learning model.

We achieved an 85% accuracy using resnet-50 to classify and identify the specie of a specific mel-spectrogram. The result was achieved by averaging five iterations of training using a stratified 5 fold train-test split. The resulting model was then used to infer specific specie on a raw audio file. The inference methodology resulted to a high of 52.2% score in the kaggle leaderboards. ALthough the inference methodology resulted in a low score, many improvements could be done to increase its performance.

**Important Note**: Main .Pickle file is excluded from this repository due to file size. Please send me an email at matmat.romero@gmail.com to request for it.

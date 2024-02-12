# Finding Zeke

## Scenario

Zeke an adorable dog who has gone missing for weeks and does not have a microchip identifier. The owners are reaching out to nearby dog shelters to see if he has been found by any of them.

Images provided by dog shelters are in ./images/collection directory.
Zeke's photo is available in ./images/test directory

### Image Embeddings for Similarity Analysis

Image embeddings for similarity analysis involve transforming images into a set of numbers that represent the features of the images, sort of like a fingerprint for each picture. These numerical fingerprints are designed so that images with similar content will have similar fingerprints.

By comparing these fingerprints, computers can quickly and accurately identify images that are visually similar to each other, just as you might sort objects based on their shapes or colors.

### How to run the code

1. You may have to install [Miniconda](https://docs.anaconda.com/free/miniconda/index.html) if you do not have conda installed. Miniconda is a free minimal installer for conda.

2. Create a Conda environment.

- `conda create --name findingzeke python==3.10 --yes`
- `conda activate findingzeke`
- `conda install notebook ipykernel --yes`
- `ipython kernel install --name findingzeke --display-name "Python 3.10 (findingzeke)" --user`

3. Install libraries.

- `pip install torch`
- `pip install requests matplotlib python-dotenv`
- `pip install transformers`

4. Rename .env_template file to .env, update values in .env file.

5. Run the code in notebooks within ./notebooks directory.

- Notebook 01 demonstrates Azure AI Vision embeddings.
- Notebook 02 uses CLIP embedding model from Hugging Face.

### What else is required

- An Azure Subscription with Azure AI services multi-service account provisioned.
- Visual Studio Code.

### References

- Azure AI Services – Image Analysis (AI Vision Embeddings)
  - https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/how-to/image-retrieval
  - https://learn.microsoft.com/en-us/rest/api/computervision/image-retrieval/vectorize-image
- Hugging Face – CLIP
  - https://huggingface.co/docs/transformers/model_doc/clip

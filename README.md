# 🔭StorySeeker

This repository contains data, a codebook, and other resources for the detection of storytelling in online communities.

<br><br>

## Preprint

**Where do people tell stories online? Story Detection Across Online Communities**    
Maria Antoniak, Joel, Mire, Maarten Sap, Elliott Ash, Andrew Piper (2023)   

You can read our preprint [here](https://github.com/maria-antoniak/storyseeker/blob/main/2023_preprint_where_stories.pdf).

<br><br>

## 🔭StorySeeker Dataset

This dataset includes 502 texts annotated with story- and event-spans.

You can view the data annotations [here](https://github.com/maria-antoniak/storyseeker/blob/main/storyseeker_data.csv).

We sampled Reddit posts and comments from the [Webis-TLDR-17](https://huggingface.co/datasets/webis/tldr-17) dataset. You must "rehydrate" the data by linking to the original dataset using the `id` column in our CSV.

We assign each of the top 500 subreddits in the dataset to a thematic category. These 33 categories can be found [here](https://github.com/maria-antoniak/storyseeker/blob/main/subreddit_categories.csv).

<br><br>

## 🔭StorySeeker Codebook

Our definition of storytelling and our full codebook can be found [here](https://github.com/maria-antoniak/storyseeker/blob/main/codebook.md).

<br><br>

## 🔭StorySeeker Models

The document classification model is available [here](https://huggingface.co/mariaantoniak/storyseeker) and can be accessed via Hugging Face.

Example code coming soon...

<br><br>

## Citation

If you use our data, codebook, or models, please cite the following preprint.

[Where do people tell stories online? Story Detection Across Online Communities]()  
Maria Antoniak, Joel Mire, Maarten Sap, Elliott Ash, Andrew Piper  


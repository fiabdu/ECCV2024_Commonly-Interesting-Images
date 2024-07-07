# Commonly Interesting Images
The _FlickrUser_ dataset is introduced as part of the _Commonly Interesting Images_ research work, which is authored by Fitim Abdullahu and Helmut Grabner. This dataset was presented at the European Conference on Computer Vision 2024 (ECCV 2024).

## Dataset
The _FlickrUser_ dataset contains 500k images from close to 2.5k users of the popular photo-sharing platform Flickr. The download link provides the file _FlickrUser.csv_, which contains detailed information about the users and the images.

### Download Link
[FlickrUser.csv](https://drive.google.com/uc?id=1Q2IJi_xn2cbUTcmtJ26rLPvKcjWT1bsb&export=download)

### CSV Columns Description
The _FlickrUser.csv_ file includes the following columns:

| Column Name                         | Description                                                                                 |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| **user**                            | Unique user ID                                                                              |
| **img_id**                          | Unique image ID                                                                             |
| **img_url**                         | Image URL for download                                                                      |
| **views**                           | Total number of views on the image                                                          |
| **favorites**                       | Total number of favorites on the image                                                      |
| **comments**                        | Total number of comments on the image                                                       |
| **upload_date**                     | Upload date of the image                                                                    |
| **user_gender**                     | Gender of the user                                                                          |
| **user_timezone_label**             | Timezone label of the user                                                                  |
| **user_timezone_id**                | Timezone ID of the user                                                                     |
| **img_owner_ispro**                 | Indicates if the image owner is a Flickr PRO user                                           |
| **img_owner_pro_badge**             | Shows which PRO badge the image owner has                                                   |
| **img_owner_occupation**            | Shows the occupation of the image owner                                                     |
| **set**                             | Indicates which images have been used to define the CI score (train or test)                |
| **ci_score**                        | CI score of the image, indicating its level of interest                                     |
| **cluster_label**                   | Cluster label of the image used for partitioning                                            |
| **partition**                       | Partition of the image                                                                      |
| **group**                           | Indicates the group in which the image is categorized (0: commonly interesting, 1: interplay, 2: subjective interesting) |
| **photographic styles & aesthetic score** | Computed using the [VILA](https://arxiv.org/abs/2303.14302) model, includes various photographic style such as complementary colors, duo tones, HDR, etc. |
| **emotions**                        | Computed using [CLIP](https://arxiv.org/abs/2103.00020), includes emotion_score, emotions, and emotion_category     |

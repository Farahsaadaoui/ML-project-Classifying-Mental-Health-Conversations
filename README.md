# README: Mental Health Subreddit Post Dataset

## 1. Dataset Description
This dataset contains posts scraped from the subreddit `/r/mentalhealth`, using the Reddit API via Python's PRAW library. Each post provides insights into discussions around mental health, making it a valuable resource for classification tasks related to mental health topics. 

- **Number of Posts**: 2000
- **Date of Collection**: September 29, 2024
- **Source**: Subreddit `/r/mentalhealth`

## 2. Data Collection Method
The data was collected using Python and the Reddit API (via the PRAW library). Filters were applied to ensure the relevance and length of posts, allowing for more meaningful classification:
- Only posts that were of sufficient length to support classification were included.
- Posts with a minimum of 8 comments were selected, prioritizing those that engaged more community responses.

## 3. Dataset Format
The dataset is stored in CSV format. Each row represents a single post from the subreddit. The following fields are included:

| **Field**    | **Description**                                       |
|--------------|-------------------------------------------------------|
| **Title**    | The title of the post, as submitted by the user.       |
| **Content**  | The main content of the post.                          |
| **Upvotes**  | Number of upvotes the post received.                   |
| **Comments** | Number of comments the post has.                       |

## 4. Estimated Time for Annotation
- **Short posts**: 5-10 seconds.
- **Longer posts**: 30 seconds to 1 minute, depending on complexity.

## 5. Potential Missing Data
There may be some posts with incomplete data (e.g., posts with low engagement or short, irrelevant content). These posts were filtered out during the data collection process to ensure higher-quality samples for classification.

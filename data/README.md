# Twibot-22 Sample Dataset

This folder contains a subset of the Twibot-22 dataset, sampled to include 1,000 users due to the original dataset's large size. Twibot-22 is a benchmark dataset for graph-based Twitter bot detection, originally introduced by Feng et al. (2022). The full dataset and details can be found in the paper:

> Feng, Shangbin, Zhaoxuan Tan, Herun Wan, Ningnan Wang, Zilong Chen, Binchi Zhang, Qinghua Zheng et al.  
> "Twibot-22: Towards graph-based twitter bot detection."  
> *Advances in Neural Information Processing Systems*, 35 (2022): 35254-35269.

### Files
- **`user_sample.json`** – Contains user profile information.
- **`label_sample.csv`** – Includes bot/human labels for users.
- **`edge_sample.csv`** – Represents relationships between users.

### Data Dictionary

| File               | Column             | Description |
|--------------------|-------------------|-------------|
| user_sample.json  | created_at         | Account creation date |
|                   | description        | User bio |
|                   | entities           | Embedded links/media info |
|                   | id                 | Unique user ID |
|                   | location           | User location |
|                   | name               | Display name |
|                   | pinned_tweet_id    | Pinned tweet ID |
|                   | profile_image_url  | Profile picture URL |
|                   | protected          | Whether the account is private |
|                   | public_metrics     | Follower, following, tweet count, etc. |
|                   | url                | Profile URL |
|                   | username           | Twitter handle |
|                   | verified           | Verification status |
|                   | withheld           | Withheld regions (if any) |
| edge_sample.csv   | source_id          | Source user ID |
|                   | relation           | Type of relationship (e.g., follow, retweet, quote, post, like) |
|                   | target_id          | Target user ID |
| label_sample.csv  | id                 | User ID (matching user_sample.json) |
|                   | label              | human, bot |

This dataset serves as a basis for evaluating Twitter bot detection models. 

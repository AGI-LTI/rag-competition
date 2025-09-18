---
layout: page
title: Static Submission Guidelines
permalink: /static-submission/
---

This page provides instructions for **Option 1: Static Evaluation on the Validation Set**. This participation option is for teams who wish to benchmark their models on the public validation set and are eligible for non-cash prizes.

## Submission Process

Once a team is registered, the organizers will contact you via your registered email with the following:

1.  **Team ID**
2.  A **Google Drive folder** for uploading your results for the specific track you have registered for (either Text-to-Text or Text-to-Video).

Teams will also receive an unseen validation set approximately one week before the competition deadline (~ October 6th, 2025).

* This unseen validation set will contain query text only.

* No reference answers will be provided (unlike the public validation set).

* Teams must generate responses (text or video) for this unseen set and submit them in the same format as described below.

This ensures a more reliable measure of model generalization beyond the publicly available validation queries.

You should upload your results to your assigned Google Drive folder and then fill out the [submission form](https://forms.gle/wRVKH7YfZXaM5QS1A).


⚠️ Note: Submission of validation set generations entitles you to a chance to win **non-cash prizes only**. These submissions are **not eligible for cash prizes**.

<br>

## Submission Format and Requirements

### Track A: Text-to-Text Generation

For Text-to-Text submissions, you must provide a .jsonl file where each line is a JSON object containing your system’s generated response to a query.

Each JSON object must include the following keys:

* `query_id` (string): The identifier of the query from the validation/test set.

* `generated_response` (string): Your system’s generated text response.

* `cited_passages` (array of objects, optional): Passages from sources used to justify the response, if your system supports citation. Each passage may include:

  * `text` (string): the cited passage.

  * `source` (string): the source of the passage.

⚠️ Note: `cited_passages` is **optional** — you only need to provide it if your system is capable of producing citations. Providing citations is considered an additional plus, but not including them will not hurt your placement.

#### Example entry
Do note that the example is generated for demonstration purposes only (non-factual). 
```json
{
  "query_id": "71c2b9e5f4d84b3dbb92711f50c12abc",
  "generated_response": "The Great Fire of London began on September 2, 1666, in a bakery on Pudding Lane. Fanned by strong winds, the fire spread rapidly across wooden buildings, ultimately destroying a large portion of the city. Although much property was lost, official records suggest relatively few deaths. The fire also prompted major rebuilding efforts and changes to fire safety regulations in London.",
  "cited_passages": [
    {
      "text": "The fire started in Thomas Farriner's bakery on Pudding Lane on September 2, 1666, and spread quickly due to strong winds.",
      "source": "Johnson, P. (2017). Disasters in History: The Great Fire of London. Historical Review."
    },
    {
      "text": "Despite destroying thousands of homes and buildings, the Great Fire of London caused relatively few recorded deaths.",
      "source": "Smith, L. (2019). London Rebuilt: Urban Planning After the Great Fire. City Press."
    }
  ]
}

```
<br>

### Track B: Text-to-Video Generation
For Text-to-Video submissions, you must provide a compressed folder containing:
* The generated video files.
* A .jsonl file mapping queries to the generated video files.

Each JSON object in the .jsonl file must include the following keys:

* `query_id` (string): The identifier of the query from the validation/test set.
* `generated_video_fname` (string): The filename of the generated video in the compressed folder.

#### Example entry

```json
{
  "query_id": "c4a8e9d7f2b4410f9b381c1d2a673def",
  "generated_video_fname": "great_fire_london.mp4",
}
```

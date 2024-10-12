# Fixed URL IOTD

This GitHub repository contains a workflow that automatically fetches the Bing Image of the Day and stores it in the repository. The latest image is saved as `image-of-the-day.jpg` in the root folder, and archived images are stored in the `iotd/` folder, named by their corresponding ISO date (e.g., `iotd/2024-10-12.jpg`).

## Features

- **Frequent updates**: The repository updates frequently, fetching the latest Bing Image of the Day.
- **Image comparison**: If the image has not changed, no commit is made, avoiding unnecessary commits.
- **Archival system**: Each image is archived in the `iotd/` folder with the filename as the current date (in `YYYY-MM-DD` format).

## Workflow

The repository uses GitHub Actions to automate the process. Here's how the workflow operates:

1. **Fetching the image**: The workflow runs to fetch the Bing Image of the Day from the Bing API.
2. **Comparing the image**: It compares the newly downloaded image with the previous day's image (`image-of-the-day.jpg`). If they are identical, no changes are committed.
3. **Committing changes**: If the image is new or different from the previous image, it is saved in the `iotd/` folder using the current date as the filename, and also updates `image-of-the-day.jpg`. The changes are then committed and pushed to the repository.

## How to Use

You can access the latest Bing Image of the Day directly via the following fixed URL:

**[Latest Image of the Day](https://wawhatt.github.io/fixed-url-daily-image/image-of-the-day.jpg)**

This URL will always point to the most recent image updated by the workflow.

### Embed the Image in Your Website

To embed the Bing Image of the Day into your website or project, you can use the following HTML code:

```html
<img src="https://wawhatt.github.io/fixed-url-daily-image/image-of-the-day.jpg" alt="Bing Image of the Day">
```

## Latest Image Preview

Here is the current Bing Image of the Day:

![Latest Image of the Day](https://wawhatt.github.io/fixed-url-daily-image/image-of-the-day.jpg)

# VSM builder and game

A single-page tool for building a value stream map (VSM) of a process, such as sales to tender, and playing a short game to find the bottleneck and test improvement ideas.

## What it does

- Records your current-state steps: owner, process time, wait time, and %C&A
- Calculates process time, lead time, flow efficiency, and rolled %C&A
- Lets you add improvement ideas, each tagged with the waste it targets (TIMWOODS)
- Runs a two-round game: find the biggest bottleneck, then pick the ideas that raise flow efficiency the most
- Draws a full value stream map for the current or future state, with queue triangles, a timeline ladder, and kaizen bursts
- Exports the map as SVG or PNG, and the flow as Mermaid code

## How to use it

1. Open `index.html` in a browser, or visit the published page.
2. Enter your steps and improvement ideas, or start from the sample tender process.
3. Press **Start game**, pick the bottleneck, then choose your ideas.
4. Switch the value stream map to **Future state** to see the result.
5. Use **Save file** to keep your work and **Load file** to restore it.

All times are in hours, and a working day is counted as 8 hours.

## Your data

The tool runs entirely in your browser. Nothing is uploaded or sent anywhere. Your work autosaves in your own browser for the web address you use, so it will not appear on another device or link. Use **Save file** and **Load file** to move it.

Do not add confidential company data to the repository itself. The file contains only a sample process.

## Run it locally

No install or build step is needed. Download `index.html` and open it in any modern browser.

## Publish with GitHub Pages

1. Go to **Settings > Pages** in the repository.
2. Under Source, choose **Deploy from a branch**, then select the `main` branch and the `/ (root)` folder.
3. Save. The page appears at `https://<username>.github.io/<repository>/` after a minute or two.

## Customize

The sample steps and improvement ideas are defined in the `sample()` function near the top of the script. Edit them to change the starting data, or enter your own in the page and save the file.

# Chrome2Tana

Here's a really basic implementation of a Chrome extension that uses the Tana API. It's pretty ugly, but it works!

## Instructions to install

1. Download the two files `Send to Tana.crx` and `Send to Tana.pem` to a folder named `Tana extension`, in any directory you wish.
2. Open up Chrome and navigate to your Extensions page (ie. `chrome://extensions/`)
3. Toggle "Developer Mode" to switch it on (found in the top right of your page).
4. Click `Load unpacked` on the top left corner of the page and a prompt will ask you which folder to use.
5. Select the folder containing the crx and pem files.
6. Done!

## Configuration

1. Click your extension button (the jigsaw logo) and scroll down until you see the Tana icon. Feel free to Pin it for easier use.
2. Click on the Tana icon and go to the Settings page.
3. You will need to fill in three things here:
  A. API Token
    1. Click on the Gear icon in Tana (as of now, it should be in the bottom left hand corner of your Tana page in the sidebar), and select API Tokens.
    2. If you do not have any Tokens, click Create. Once done, click `Copy`.
    3. Go back to the Settings page of the Tana chrome extension and paste it into the API Token field.
  B. Endpoint URL
    1. As of now, enter in "https://europe-west1-tagr-prod.cloudfunctions.net/addToNodeV2". This might be subject to change in future.
  C. Tags
    1. You will need to add a tag for sure, and unfortunately as of now I have not coded it to leave it blank, although I am thinking of doing it in future. A tag consists of a label (you can specify any name that makes sense for you) and a value.
    2. To get the value of the tag, you need to go to your Tag customisation page in Tana.
    3. On the tag page, click on the name (e.g. `#example`) and hit `Ctrl-K` and type in `Show API schema`.
    4. A scary looking popup should appear, but all you need to look for is the `id` value next to `supertags`. Copy this.
    5. Go back to your settings page and paste it in the field on the right, next to your specified tag label.
4. Remember to click "Save Settings". Then close the window. This is the only time you need to set the settings, and you're done.

## Enjoy!
Enjoy the extension? Join our subreddit at http://reddit.com/r/TanaInc for more community fun :)

## Maybe To Dos

- [ ] Highlights on the page
- [ ] Automatically pull in Youtube transcripts
- [ ] Automatically fill in Twitter
- [ ] Send to specific nodes
- [ ] Fill children fields

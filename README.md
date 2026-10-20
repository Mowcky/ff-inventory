# Foundation First Inventory website

- `index.html` – the website: office dashboards, QR cards, item lists, adding/editing/transferring/archiving, sticker printing
- `data.json` – the inventory data
- `publish.html` – optional: import Excel files (replaces everything)

## One-time setup

1. On github.com choose **New repository**, name it `ff-inventory`, keep it **Public**, and create it.
2. Choose **uploading an existing file**, drop in the three files, and **Commit changes**.
3. **Settings → Pages**: Source **Deploy from a branch**, Branch **main**, folder **/ (root)**, **Save**. After a minute your address appears, like `https://yourname.github.io/ff-inventory/`.
4. Open the address, go to an office, and scan a card with your iPhone camera to test.

## Turning on editing (once per computer or phone you edit from)

1. Go to https://github.com/settings/personal-access-tokens/new
2. Name it "FF Inventory", pick an expiration (up to a year), choose **Only select repositories** and pick `ff-inventory`.
3. Under **Repository permissions**, set **Contents** to **Read and write**. Generate the token and copy it.
4. On the website choose **Settings & backup → Connect GitHub** and paste it. Username and repository fill in automatically.

After that, every change shows an **Unsaved changes** bar. Choose **Save to GitHub** and the public site updates within a minute or two. Anyone who only scans stickers never needs a token.

## Everyday use

- **New purchase:** open the person, **Add item**.
- **Move an item:** tap it, **Transfer**, choose who it goes to, then swap the sticker.
- **Broken, lost or disposed:** tap it, **Archive**. It moves to that person's History, where **Restore** puts it back.
- **Someone leaves:** open their page, **Person leaving**. Keep the position (becomes VACANT, items stay) or archive the whole position.
- **New hire:** on a VACANT position choose **Assign new person**, or on an office page choose **Add person**.
- **Quarterly check:** **Settings & backup → Download backup** and **Export to Excel**.

## Item requests

1. On the website, open **Settings & backup → Item requests**, enter the email address requests should go to, choose **Save request settings**, then **Save to GitHub**.
2. Staff open their page (scan their sticker or bookmark it) and choose **Request an item**. They paste the link, add the quantity, price and reason, and choose **Send request**. Their email app opens with everything filled in, addressed to you.
3. The email has a link at the bottom. Open it on a device connected to GitHub and choose **Add as Pending**.
4. On their page, choose **Approve** or **Not approved** (a reason is required, and staff can see it). Then **Mark ordered**, and when it arrives, **Received: add to inventory**, which adds it to their list with the details already filled in.
5. Open requests show on the home page, on each office card and in the Excel export (Requests tab).

Staff never need a GitHub account. Without a token, the site hides the editing buttons and only shows **Request an item**.

## Privacy

Anyone with the address can view the site, and `data.json` is public. Ask Claude to add a passcode later; stickers will not need reprinting.

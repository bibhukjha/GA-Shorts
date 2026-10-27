# CA Shorts

Swipeable current-affairs flashcards (Inshorts-style) for exam revision. Upload your daily PDFs, and the app turns them into cards with key facts and images.

- **No server, no database to host.** Everything is stored on your device in the browser (IndexedDB).
- **One file:** `index.html`. Hosted free on GitHub Pages.
- **Your PDFs and cards are never uploaded to GitHub.** Only the extracted text is sent to the AI provider you choose, using your own API key.

## 1. Put it on GitHub Pages (free)

1. Create a GitHub account, then a **new repository** (e.g. `ca-shorts`). Make it **Private** if you want. Pages on private repos needs a paid plan, so use **Public**. The repo only contains the app code, never your PDFs or data.
2. Click **Add file → Upload files**, drop in `index.html` and `README.md`, then **Commit**.
3. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and **Save**.
4. After about a minute your app is live at `https://YOUR-USERNAME.github.io/ca-shorts/`.

## 2. Get a free AI key (Google Gemini)

1. Open https://aistudio.google.com/apikey and sign in.
2. Click **Create API key** and copy it.
3. In the app tap **＋ → AI settings**, keep provider as **Google Gemini**, and paste the key.

The key is saved only in your browser's localStorage. If you prefer Claude, choose **Anthropic Claude** and paste an Anthropic API key (paid). Model names can be changed in the Model box if a default stops working.

## 3. Use it on iPhone Safari

1. Open your GitHub Pages link in Safari.
2. Tap **Share → Add to Home Screen**. This gives you an app icon, and iOS is much less likely to clear its storage than for a normal tab.
3. Every morning: **＋ → select the day's PDFs (several at once) → Make cards**. Then swipe up to study.

## 4. Protect your data

- Safari can delete site data if you don't use a website for about 7 days, unless it's added to the Home Screen. Do the Home Screen step.
- Tap **＋ → Export backup** now and then. It saves a `.json` file with all cards and images. **Import backup** restores it, including on a new phone.
- Don't use Private Browsing, since nothing is saved there.

## Notes

- Free Gemini keys have rate limits. If it says "waiting", the app retries automatically.
- Text-based PDFs work. Scanned image-only PDFs have no text to read.
- Word files (.docx) give text cards only, without images.
- Use your subscribed PDFs for personal study only. Don't publish them or the exported backups publicly.

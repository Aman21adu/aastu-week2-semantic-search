# Week 2 — Final upload steps (GitHub + Google Colab)

## Step 1 — Download/extract

Download the provided ZIP and extract it. Keep all files visible inside the folder.

## Step 2 — Create GitHub repository

1. Sign in to https://github.com/Aman21adu
2. Open https://github.com/new
3. Repository name: **aastu-week2-semantic-search**
4. Visibility: **Public**
5. Leave "Add a README", license and .gitignore **unchecked** (they are included).
6. Click **Create repository**.

## Step 3 — Upload the files

1. In the empty repository choose **uploading an existing file**. If needed choose **Add file → Upload files**.
2. From the **unzipped folder**, upload these six files: `Week2_Mini_Semantic_Search.ipynb`, `faqs.csv`, `README.md`, `requirements.txt`, `.gitignore`, `SUBMISSION_STEPS.md`. **Do not upload the ZIP itself.**
3. If `.gitignore` is hidden by your file browser, enable showing hidden files; otherwise create that file from GitHub's Add file interface.
4. Enter commit message: `Add Week 2 semantic search lab`.
5. Click **Commit changes**.

Your GitHub submission link should now be:
https://github.com/Aman21adu/aastu-week2-semantic-search

## Step 4 — Open the GitHub notebook in Colab

After the GitHub repository exists, open:
https://colab.research.google.com/github/Aman21adu/aastu-week2-semantic-search/blob/main/Week2_Mini_Semantic_Search.ipynb

If that address does not open, go to https://colab.research.google.com/ and select **File → Open notebook → GitHub**, then paste your repository URL.

## Step 5 — Run and verify

1. Choose **Runtime → Run all** (allow Google to connect to its hosted Python runtime).
2. First execution installs libraries and downloads the MiniLM model; internet is required.
3. Confirm no code-cell exceptions and check **16 clean FAQs**, **17 chunks**, and the **top 3 matches** for all five test queries.
4. If Colab asks to restart after installation, **Runtime → Restart session**, then **Run all** again.

## Step 6 — Save the executed notebook and make a second genuine Git commit

1. Choose **File → Save a copy in Drive** so you own a Drive notebook with the output cells.
2. Use **File → Download → Download .ipynb** to get the executed notebook (menu wording can vary).
3. In your GitHub repository open `Week2_Mini_Semantic_Search.ipynb`, then use **Add file → Upload files** to replace it with the executed version. If the interface does not offer replacement, open the file, use the file's editing/upload workflow, or use Colab's `File → Save a copy in GitHub` if offered. The result must be a committed update to that file.
4. Commit message: `Save executed Week 2 search results`.

## Step 7 — Copy your Colab sharing link

In your **Drive copy** of the notebook click **Share → General access**. Set viewer access according to your instructor's requirements. Click **Copy link**.

### Paste into assignment spreadsheet

**Week-2 GitHub:** https://github.com/Aman21adu/aastu-week2-semantic-search

**Week-2 Colab:** Use the copied Drive-share URL (recommended; your executed outputs will be visible). The GitHub-backed Colab URL above is a valid alternative once the repo and notebook exist.

## Final check

- [ ] GitHub repo opens publicly and has the Week 2 files
- [ ] Colab notebook link opens for instructor
- [ ] Whole notebook ran without code-cell exceptions
- [ ] Chroma was populated and search output shows top 3 matches
- [ ] Executed notebook outputs are saved
- [ ] README and requirements.txt are present
- [ ] `.venv/` / generated vector database not committed
- [ ] Commit history shows initial upload and an actual notebook update

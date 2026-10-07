# `jobsearch` 🔍

An AI assistant for your job search. It runs in the terminal, on your own computer.

## What `jobsearch` does

- **Finds jobs.** It searches the Adzuna job API. It can also read your LinkedIn job-alert emails (note: currently a personal Gmail account does not work for this part - Coming Soon!). A search shows only the jobs that are new to you.
- **Gets the full posting.** For each job, it looks for the employer's own posting and keeps the full text.
- **Ranks the jobs.** It compares each job with your resume and gives a fit score with the reasons. It marks a work mode or an amount of travel that you do not accept.
- **Helps you apply.** It writes a draft cover letter and a draft message to the recruiter. With a "resume as code" repository, it also makes a resume for 1 job.
- **Helps you prepare.** A search report gives a learning plan for your skill gaps, interview questions, and career advice.
- **Takes your corrections.** When the model says something wrong about you, you mark it and correct it.
- **Keep your keys secret**. `jobsearch` keeps them in the macOS Keychain or the Linux Secret Service.

`jobsearch` never sends an application, an email, or a message for you. You stay in control.

## What to prepare

You need these things to use `jobsearch`:

1. A Mac or a Linux computer. Windows is not part of this test (but WSL will work).
2. [Homebrew](https://brew.sh/). Homebrew installs `jobsearch` and the Python that it needs.
3. Access to an LLM, initially tested with (either will do):
   - A Claude plan that includes Claude Code (for example Pro, Max, or Team). Install Claude Code, run `claude`, and log in with `/login`. jobsearch uses your own login. Do not share it.
   - An AWS account with Bedrock access to the Claude models, and a Bedrock API key.
4. Adzuna API keys. [Sign up for free](https://developer.adzuna.com/) to get an App ID and an API key.
5. Your resume as a PDF or DOCX file.

These items are optional:

- An [Exa](https://exa.ai/) API key. `jobsearch` uses Exa to find the employer's own posting.
- LinkedIn job alerts in a Google Workspace mailbox. `jobsearch` reads them through a Google Workspace service account, with read access only. Only an admin of the Workspace can set that up.
- A "[resume as code](https://github.com/nathanfox/resume-as-code)" repository, for tailoring resumes per job.

## How to test `jobsearch`

1. Tell Rowena that you want to join, and let her know your GitHub user name.
2. She will send you the install steps. The install takes a few commands.
3. Use `jobsearch` for your real job search, or for a practice search.
4. Tell Rowena what breaks, what is not clear, and what you want to see.

## Your data privacy

- Your found jobs, notes, settings, and documents (cover letters/resumes) stay in folders on your computer. `jobsearch` has no analytics, reporting, callbacks, or even a hosted server at all. You remain in control of where your data is sent.
- `jobsearch` sends job description/title/pay range text and resume text to the LLM model that you choose. It sends search words to Adzuna and to Exa.

---

*(Content added by Kenzie, LLM-based artificial assistant, on behalf of Rowena Day.)*

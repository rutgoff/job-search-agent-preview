# `jobsearch` 🔍

An AI assistant for your job search. It runs in the terminal, on your own computer.

## What `jobsearch` does

- **Finds jobs.** You add a job from the link of its posting. It can also read the LinkedIn job alerts in your personal Gmail, and search the Adzuna job API. A search shows only the jobs that are new to you.
- **Gets the full posting.** For each job, it keeps the full text of the employer's own posting. With an Exa API key, it looks for the posting by itself.
- **Ranks the jobs.** It compares each job with your resume and gives a fit score with the reasons. It marks a work mode or an amount of travel that you do not accept.
- **Helps you apply.** It writes a draft cover letter and a draft message to the recruiter. It also makes a tailored resume for 1 job. It keeps your resume in a "[resume as code](https://github.com/nathanfox/resume-as-code)" repository, and it sets up that repository from your resume file.
- **Helps you prepare.** A search report gives a learning plan for your skill gaps, interview questions, and career advice.
- **Takes your corrections.** When the model says something wrong about you, you mark it and correct it.
- **Keeps your keys secret.** `jobsearch` keeps them in the macOS Keychain or the Linux Secret Service.

`jobsearch` never sends an application, an email, or a message for you. You stay in control.

## What to prepare

You need these things to use `jobsearch`:

1. A Mac (Apple silicon or Intel) or a Linux computer. Windows is not part of this test. Linux in WSL 2 can work, but nobody has tested it yet.
2. [Homebrew](https://brew.sh/). Homebrew installs `jobsearch` and the Python that it needs.
3. A download key from Rowena: 32 letters, digits, `-` or `_`. She sends it to you in a private message. The key is for you only.
4. A Claude plan that includes Claude Code, for example Pro, Max, or Team. `jobsearch` uses your plan through Claude Code, with your own sign-in. Do not share your sign-in.
5. Your resume as a PDF, a DOCX, or a text file (`.txt` or `.md`).
6. git, pandoc, and Google Chrome (on Linux, Chromium also works). git keeps your resume files. pandoc and Chrome make the PDF of your resume. The [tester guide](https://github.com/rutgoff/homebrew-jobsearch-agent/blob/main/GUIDE.md) shows how to install them.
7. About 30 minutes and 4 GB of free disk space for the first setup. On an Intel Mac, allow 20 minutes more: Homebrew can build Python from source there.

These items are optional:

- A personal Gmail address that gets LinkedIn job alerts. `jobsearch` reads the alerts with an app password, with read access only. Your Google account needs 2-Step Verification for the app password.
- Adzuna API keys: an App ID and an API key. [Sign up for free](https://developer.adzuna.com/). With the keys, `jobsearch` can also search the Adzuna job API.
- An [Exa](https://exa.ai/) API key. With the key, `jobsearch` looks for the employer's posting by itself, with at most 40 Exa searches a day. Without the key, you add the link or the text of the posting yourself.

## How to test `jobsearch`

1. Tell Rowena that you want to join. You do not need a GitHub account.
2. She sends you an invite email with the links to the [install steps](https://github.com/rutgoff/homebrew-jobsearch-agent#install) and the [tester guide](https://github.com/rutgoff/homebrew-jobsearch-agent/blob/main/GUIDE.md). Your download key comes in a separate private message. The install takes a few commands.
3. Use `jobsearch` for your real job search, or for a practice search.
4. Tell Rowena what breaks, what is not clear, and what you want to see.

## Your data privacy

- Your found jobs, notes, settings, and documents (cover letters/resumes) stay in folders on your computer. `jobsearch` has no analytics, reporting, callbacks, or even a hosted server at all. You remain in control of where your data is sent.
- `jobsearch` sends job description/title/pay range text and resume text to Claude, through your own Claude plan. With the optional keys, it also sends your search words to Adzuna. Exa gets only the job title and the company.

---

*(Content added by Kenzie, LLM-based artificial assistant, on behalf of Rowena Day.)*

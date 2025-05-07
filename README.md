
## Steps I Took
Instructions: 
I generated an SSh key with this command in Mac Terminal: ssh-keygen -t ed25519 -C "anglofnew@gmail.com"
Pressed Enter to accept the difault path, not setting a passphrase
Saved my private keys:
Private key: ~/.ssh/id_ed25519

Public key: ~/.ssh/id_ed25519.pub

Then i registered in pico using: ssh pico.sh
The first time, I was asked if I trust the host. I typed yes and pressed Enter.
I followed the on-screen instructions to choose a username (aggelostestepikast).
(After registration, pico.sh opens a dashboard. You don’t need to do anything there; just exit with Ctrl+C or close the window.)

HTML File download:
I visited https://www.karl.berlin/simplicity.html in my browser.

Right-clicked the page and selected Save As.

Saved the file as simplicity.html in my home directory (~/simplicity.html).

Uploading the html file to pico.sh:
Command: rsync -v ~/simplicity.html pgs.sh:/aggelostestepikast


Result:
My website is now available at:
https://aggelostestepikast.pgs.sh/simplicity.html




Then I created a GitHub Repository and Upload Files
Steps:

Went to GitHub.com and created a new repository named pico-sh-assignment.

Clicked Add file > Upload files and uploaded:

simplicity.html

My public SSH key (~/.ssh/id_ed25519.pub) inside a new folder called InfoUsed

Created a file README.md (this document) to explain my process, decisions, and the prompts I used.



So in summary:
- I generated an SSH key using the command from the pico.sh FAQ.
- I registered on pico.sh and set up my username.
- I downloaded the required HTML file from the given link.
- I uploaded the HTML file to pico.sh using `rsync`.
- I created a GitHub repository and uploaded all required files.

## Decisions
- I used a Mac OS terminal. On Linux, the steps are identical. On Windows, you may need to use Git Bash or WSL.
- I followed the pico.sh documentation closely.
- I used rsync for uploading because it was recommended.

## Prompts Used

Prompts Used with LLM (AI)
(I used Perplexity and uploaded the pdf file along with the links provided to me via email)

-" Take all the files I will give you and carefully make a guide on how to solve this project. I'm young, so teach me; I know nothing about code."
- Explain me what each command does so i cannot just complete the task but also understand it completely
  
- + some basic queries where I stuck with the code in terminal. But basically the above prompts helped me solve it.

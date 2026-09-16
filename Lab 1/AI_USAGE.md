# AI Usage - Benjamin Wilson

For this assignment, I used generative AI to understand some of the processes involved with creating a reproducible set-up, the difference between conda and mamba, etc. THe primary usage I had was to diagnose errors and to have the AI recommend fixes. 

## Critical Error Number 1

One critical error I had was when my computer had two separate miniforge installations. I asked ChatGPT-5.6 Luna what the error was and how to fix it, along with pasting my error message. It told me about the two separate miniforge installations, and asked me to identify which executables I was using. Seeing as this was an exploratory process, I entered the diagnostics into my terminal. The fix involved me switching from miniforge_x86 to miniforge3, which was preferred. After making the switch, I verified the architecture, which returned miniforge3. After this, I could run the mamba environment and run the analyze.py file.

## Critical Error Number 2

While working on the R portion of this assignment, I noticed the the snapshot function would tell me that I was trying to use the function in a project that had not been activated yet. This was strange, since I had created analyze.R despite the environment being in a consistent state. GPT-5.6 Luna recommended to activate the project in the console and use the project library. After verifying with a google search, I implemented this fix, and the snapshot function worked properly.

## Critical Error Number 3

When doing a final sanity check a week later, renv.status informed me that I had no packages installed. I used the restore function, and it gave me the same message that the project had not been activated yet. Using the same fix restarted my R session, but then restored successfully. However, the dplyr package was not installed, so I asked Luna how to add dplyr to my renv. I checked that the command was successful, and then verified that dplyr was in the lockfile.
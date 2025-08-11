# Instagram Unfollow All Non-Mutuals Bot
This Python script uses PyAutoGUI to automatically:

Detect and click "Following" buttons for accounts you follow

Skip mutual accounts (your friends who follow you back)

Confirm unfollows

Scroll through your following list until everyone who isn’t mutual is unfollowed
# 1️⃣ Requirements
Python 3.8+

Windows, Mac, or Linux

pyautogui installed:

```bash
pip install pyautogui
```
# 2️⃣ Settings
You can tweak these variables at the top of the script:
```bash
CONFIDENCE = 0.75   # Image match accuracy (0.0–1.0)
LOAD_WAIT = 8       # Seconds to wait after scrolling for new items to load
```
Lower CONFIDENCE if it’s not detecting the buttons.
Increase LOAD_WAIT if Instagram is loading slowly.

# 3️⃣ How to Use
Log into Instagram in your browser.

Open your profile and click Following to open the list of accounts you follow.

Make sure the window is fully visible and not minimized.

Open Command Prompt (Windows) or Terminal (Mac/Linux) in the folder where your script is saved.

Run:
```bash
python script.py // or you can just click it in file explorer
```
The bot will:

Detect blue mutuals and skip them

Detect grey non-mutuals and click them

Click Unfollow in the pop-up

Scroll down and repeat

Stop the bot:
Press Enter Or Exit Manually in the Terminal/Cmd. The script will finish the current loop and exit.


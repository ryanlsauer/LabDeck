# LabDeck

Your MLS study app. Everything runs in your browser; there is no server.

## Where your data lives
- On each device, in the browser's storage for this website (IndexedDB plus a second copy in localStorage).
- Optionally, in a private GitHub gist if you turn on sync in Settings. That keeps your phone and computer in step.
- Your data is never inside these files, so replacing them never touches your progress.

## Getting an update from Claude
1. Ask Claude for the change. You'll get a new `index.html` (and sometimes other files).
2. In your GitHub repository, click **Add file > Upload files**, drop the new files in, and click **Commit changes**.
3. Wait about a minute, then reopen LabDeck. Your decks and progress stay exactly as they were.

Starting a new chat with Claude? Upload your current `index.html` so it edits the latest version.

## Safety net
Settings > Download backup saves everything, including images and review history, to one file.

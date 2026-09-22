# Privacy Policy

**Last updated:** 2026-09-22

These OAuth applications are personal tools. They run only on my own computers, for my own Google account. I do not offer them to other people.

**Contact:** pgrondagarrigues@gmail.com

## gdrive-sync

**gdrive-sync** backs up files I choose to my Google Drive with [rclone](https://rclone.org/drive/).

- It accesses only my Google Drive.
- Data moves between my computer and Google. I do not send that data to anyone else.
- The OAuth token stays on my computer.

## gmail-organizer

**gmail-organizer** adds labels to my own Gmail. It uses the `gmail.modify` scope so it can read messages and add labels. It does not delete mail, and it does not remove labels I already set.

- The OAuth token and a local cache of labeling decisions stay on my computer (`token.json`, `classifications.sqlite`).
- To choose a label, the tool sends the sender, subject, date, snippet, and a truncated body to [DeepSeek](https://www.deepseek.com/) (`api.deepseek.com`). DeepSeek returns a label choice. That is the only reason the text is sent.
- When I create a new Gmail label, the tool may send the label name plus the sender, subject, and a short snippet from a few messages already filed under it, so it can write a labeling rule. That text also goes only to DeepSeek, for that purpose.
- I do not sell this data, use it for advertising, or give it to anyone other than Google and DeepSeek as described above.

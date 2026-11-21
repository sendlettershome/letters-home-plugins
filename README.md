# Letters Home plugins

Bring the emails, photos, and posts you want to keep into a [Letters Home](https://sendlettershome.com) collection. Pick the helper for your source, then tell your assistant what you want to save.

| Where your memories are | Helper to install |
| --- | --- |
| Gmail | **Mail Export** helps you download selected messages with Google Takeout. **Email Import** helps you pick which correspondence to add from that download. |
| Outlook.com or Hotmail | **Email Import** helps you save and upload the messages you choose. |
| Instagram | **Instagram Import** helps you download and add selected photo posts. |

## What to ask your assistant

- **Gmail:** “Help me save the emails my daughter sent during her mission.” The helper can guide you through Google Takeout, then help you select original letters or include both sides of the conversation.
- **Outlook or Hotmail:** “Help me bring my Hotmail emails into my Letters Home collection.” The helper walks you through downloading the messages you choose, one at a time. Outlook calls each saved email an **EML file**. You can upload one saved email or group several in a ZIP file and upload them together. Full mailbox backups in PST or OLM format are unsupported.
- **Instagram:** “Help me add selected Instagram photo posts to my Letters Home collection.”

You choose what to keep and which collection receives it. Your assistant can help in the browser when it has browser and file access. It can also give you steps to follow yourself.

## Install the helper you need

Install directly from the Letters Home GitHub repository. In each example, the `marketplace add` command tells your assistant where to find the plugins on GitHub. Then run the install command for each helper you want and restart your assistant. See the [setup guide](GUIDE.md) for details, including the Node.js 24+ requirement for the local Gmail archive filter. In order to install, just copy these snippets and paste them into your chat with your agent and it will do the rest of the work!

### Codex

```sh
codex plugin marketplace add sendlettershome/letters-home-plugins --ref main
codex plugin add letters-home-mail-export@letters-home
codex plugin add letters-home-email-import@letters-home
codex plugin add letters-home-instagram-import@letters-home
```

### Claude Code

```sh
claude plugin marketplace add sendlettershome/letters-home-plugins
claude plugin install letters-home-mail-export@letters-home
claude plugin install letters-home-email-import@letters-home
claude plugin install letters-home-instagram-import@letters-home
```

## Before you upload

Sign in on the provider's website and keep your password out of chat. Review the chosen files and collection before approving an upload. Gmail filtering happens on your computer. Check the results if you asked for originals only, since some replies can slip through. For Outlook and Hotmail, you choose each message yourself. A saved reply can still contain earlier messages quoted inside it.

Read the [setup and privacy guide](GUIDE.md) for supported files, browser access, limits, and updates.

[Support](https://sendlettershome.com/contact) · [Privacy](https://sendlettershome.com/privacy-policy) · [Terms](https://sendlettershome.com/terms-of-use)

First-party contents retain their copyright; no open-source license is granted. Bundled dependencies retain their [licenses](plugins/letters-home-email-import/THIRD-PARTY-NOTICES.txt).

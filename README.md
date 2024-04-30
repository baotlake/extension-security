# [⚠️ Monica Extension is Leaking your Data](https://ext-security.onrender.com/monica-extension-is-leaking-your-data)

[▶️ Online demo](https://ext-security.onrender.com/monica-extension-is-leaking-your-data)

Malicious websites can steal your chat data in Monica Extension without your knowledge.

Monica Extension can open a Sidebar within the page, displaying various user information such as usernames, avatars, and chat histories. However, they haven't implemented very effective isolation measures to protect user privacy, allowing any malicious webpage to access private data.

## How Monica users can protect their privacy

Before Monica fixes this issue, you can protect your privacy by:

1. Temporarily uninstalling or disabling the Monica extension.
2. Setting Site Access to "On Click" and using Monica only on trusted websites: Right-click on the Monica Extension icon > This can read and change site data > When you click the extension.

## How Monica should fix this issue

This problem arises from personal user data leaking into the external DOM. There are several ways Monica can fix this issue:

1. Use Chrome's Sidepanel (`chrome.sidepanel` API) instead of opening a Sidebar within the page.
2. Use `<iframe>` to isolate user data from the external DOM.
3. Use Closed Shadow DOM to isolate user data from the external DOM.

## Recommended Extensions

### [Anything Copilot - Any AI Copilot, Unlimited, Privacy, No Account Needed](https://ziziyi.com/copilot)

Unlock AI Insights on the Fly: Open Any AI Site in a Popup or Sidebar for Instant Access and Enhanced Productivity!

This is a unique AI Copilot extension, unique because we do not directly provide an AI model; however, you can open almost any website in a sidebar or popup, like ChatGPT, Gemini, Microsoft Copilot, Kimi, and more.

<a href="https://www.buymeacoffee.com/baotlake1" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

# bungo-bot (kotenseki-labs)
AI Tutor for Premodern Japanese

**System Prompt for Premodern Japanese Tutoring.**

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Gemini Gem Ready](https://img.shields.io/badge/Gemini_Gem-Ready-blue.svg)](https://gemini.google.com/gem/d807a82ae779)

## 📖 Overview

**Bungo-bot** is not an app, but a specialized **System Prompt** designed to transform a standard LLM (specifically Gemini Gems) into an "active leraning" tutor for premodern forms of Japanese.

This project implements the pedagogical framework described in the white paper *"What LLMs Must Forget to Teach Effectively"* (Stilerman, 2026).

## 📂 Repository Structure

* `system_prompt.xml` - **The Core File.** Copy the contents of this file into your AI instructions. (COMING SOON!)
* `What_LLMs_Need.pdf` - Background on the pedagogical design + one example.
* `examples/` - Sample conversations showing the tutor in action. (COMING SOON!)

## 🚀 How to Use (Gemini Gems)

**Click on the link in the file [Try_BungoBot.md](Try_BungoBot.md)**

## 🚀 How to Fork (Gemini Gems)

You do not need to install Python or run any code. Follow these steps to create your own tutor:

1.  **Open Gemini:** Go to [gemini.google.com](https://gemini.google.com).
2.  **Create a Gem:** Click on "Gem manager" $\to$ "New Gem".
3.  **Name It:** Give it a name like "Bungo Tutor" or "Kotenseki Assistant".
4.  **Copy the Prompt:**
    * Open the [`system_prompt.xml`](system_prompt.xml) file in this repository.
    * Copy the entire text.
5.  **Paste Instructions:** Paste the text into the "Instructions" field of your new Gem.
6.  **Save & Chat:** Click "Create". Your tutor is now ready to use for you and your students!

## 🧠 Customizing the Tutor

The prompt is written in natural language wrapped in XML tags. You can modify the behavior by editing the text before you paste it:

* **Adjusting Strictness:** Look for the `<throttling>` tag.
    * *Current:* "Ask one question at a time."
    * *Change to:* "Ask up to three questions" (if you want a faster pace or options for the student to pick from).
* **Changing Tone:** Look for the `<persona>` tag.
    * You can add instructions like "Be strict but encouraging" or "Use simple modern Japanese for explanations."

## 🤝 How to Contribute

We use GitHub to version-control the system prompt of BungoBot. Here is how you can help:

* **Fork & Clone:** Fork this repo and create a new branch for your feature or fix.
* **Edit Instructions:** Make changes to the system prompt in `system_prompt.xml`
* **Test Locally:** Copy the system prompt from `system_prompt.xml` into your own [Gemini Gem](https://gemini.google.com/gems/create) and test intesively to verify the tutor behaves as expected and doesn't crash.
* **Submit a PR:** Push your changes and open a Pull Request. Please include:
    * **The Change:** What specific instructions or features did you add/remove?
    * **The "Why":** Did the tutor performance improve? How?
    * **Example Output:** (Optional) A screenshot or text snippet of the tutor's response using the new system prompt.

## 📄 License

This project is licensed under the **GNU General Public License v3.0** - see the [LICENSE](LICENSE) file for details. This ensures the project remains free and open for all students and scholars. Any modifications or derivative versions that you distribute must also be open source.


---

*Maintained by Ariel Stilerman @ Stanford University.*

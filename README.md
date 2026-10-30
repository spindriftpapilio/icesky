<div align="center">
  <img src="assets/icesky-butterfly.svg" width="160" height="160" alt="IceSky butterfly with translucent blue and lilac wings in drifting snow">
  <h1>IceSky</h1>
  <p>A browser-based toolkit for multimodal prompt injection testing.</p>
  <p>
    <a href="README.md">English</a>&nbsp;&nbsp;&nbsp;
    <a href="README.zh-CN.md">简体中文</a>
  </p>
  <p>
    <a href="https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide"><img src="https://img.shields.io/badge/Wiki-User_Guide-315b8a?style=flat-square" alt="User guide"></a>
    <a href="https://github.com/spindriftpapilio/icesky/issues"><img src="https://img.shields.io/github/issues/spindriftpapilio/icesky?style=flat-square&amp;color=315b8a" alt="GitHub issues"></a>
    <a href="https://github.com/spindriftpapilio/icesky/stargazers"><img src="https://img.shields.io/github/stars/spindriftpapilio/icesky?style=flat-square&amp;color=315b8a" alt="GitHub stars"></a>
  </p>
  <p>
    <a href="#quick-start">Quick start</a>&nbsp;&nbsp;&nbsp;
    <a href="#features-and-documentation">Features</a>&nbsp;&nbsp;&nbsp;
    <a href="#deployment">Deployment</a>&nbsp;&nbsp;&nbsp;
    <a href="#community">Community</a>
  </p>
</div>

IceSky is a browser-based prompt injection toolkit for AI security testing. Edit test payloads, transform and encode text, embed hidden content, arrange multi-turn conversations, and generate document, image, audio, email, web, MCP, and Agent-rule samples.

For complete instructions, see the [English Wiki](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide). Review the [legal notice and authorized-use requirements](#legal-notice-and-authorized-use-requirements) before testing a target system.

## Interface preview

<p align="center">
  <a href="https://raw.githubusercontent.com/wiki/spindriftpapilio/icesky/images/manual-en/01-workbench.png"><img src="https://raw.githubusercontent.com/wiki/spindriftpapilio/icesky/images/manual-en/01-workbench.png" width="100%" alt="IceSky English workspace with a Base64 conversion"></a>
</p>

## Quick start

This repository publishes ready-to-deploy static files. You do not need Node.js, a dependency installation, or a build step.

```bash
git clone https://github.com/spindriftpapilio/icesky.git
cd icesky
python3 -m http.server 8080
```

Open <http://localhost:8080> in your browser. Click **EN** in the top-right header to switch to English. The button changes to **中文**, which switches back to Chinese. Your language preference is saved locally when browser storage is available.

Text transformations, steganography, and local sample generation work without a model connection. AI rewriting and translation require [model API configuration](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#model-apis-ai-rewriting-and-translation).

<details>
<summary>Language switching and built-in examples</summary>

Built-in examples and untouched default fields follow the interface language. Edited input and uploaded content are preserved. For unchanged built-in file samples with a current result, language switching also refreshes the preview and downloadable artifact. The injection generator has its own template-language selector. Original reference material and Chinese-specific writing features retain their intended language.

</details>

## Features and documentation

### Text and conversations

Text tools cover [transformations and decoding](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#text-transformations-and-decoding), [mutation and comparison](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#input-mutation-and-comparison), and [hidden text, emoji, and character mapping](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#hidden-text-emoji-and-character-mapping). Start with the [prompt injection generator](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#generating-prompt-injection-samples), arrange [multi-turn dialogues](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#multi-turn-dialogue), build [individual or batch samples](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#sample-builder-and-batch-export), and save [experiment notes](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#saving-experiment-notes).

### Multimodal files

File tools support [images and QR codes](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#images-and-qr-codes), [PDFs](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#pdf-generation-and-text-comparison), [Word documents, spreadsheets, and slides](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#word-spreadsheets-and-slides), [audio and subtitles](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#audio-and-subtitles), [web pages, rich text, and email](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#web-pages-rich-text-and-email), and [MCP definitions and Agent configurations](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#mcp-definitions-and-agent-configurations).

### Workspace and results

See [workspace navigation](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#the-workspace) for search, pinned tools, and keyboard shortcuts. Additional utilities are covered under [token analysis and other tools](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#token-analysis-and-other-tools). For stale results, API connections, and extraction differences, see [troubleshooting](https://github.com/spindriftpapilio/icesky/wiki/English-User-Guide#saving-results-and-troubleshooting).

## Deployment

Upload the repository's static files to GitHub Pages, Cloudflare Pages, Netlify, Vercel, S3, or another static web host. Preserve the relative locations of `index.html`, `js/`, `css/`, and the other runtime assets. Local text processing and sample generation require no backend.

The public repository contains the built release. Serve its root directory directly rather than looking for a separate `dist/` directory.

## Community

<p align="center">
  <img src="group.png" width="240" alt="IceSky community group QR code">
</p>

## Legal notice and authorized-use requirements

<details>
<summary>Read the full terms of use</summary>


### Purpose

IceSky is intended for academic AI and cybersecurity research, authorized security testing, internal risk assessment, and education. Its prompt injection, steganography, file-carrier, and Agent-rule features create test material for evaluating input handling and security controls.

Using this tool does not grant permission to test a third-party system. Obtain authorization independently of downloading the tool, generating samples, reading public research, or acquiring an API key.

### Authorization

Before testing, obtain lawful written authorization from the system owner or another authorized party. Agree on the target, schedule, methods, data scope, resource limits, and stopping conditions. Stay within that authorization and comply with applicable laws and service agreements.

### Prohibited misuse

Do not use IceSky to distribute illegal or malicious material, conduct fraud or phishing, steal information, damage systems, or deploy attack samples into third-party environments without permission. Do not induce models or Agents to disclose credentials, personal information, or other unauthorized data, or to perform unauthorized commands, file operations, or external requests.

Unauthorized bulk testing, harassment, unlawful commercial activity, and interference with other people's services or resources are prohibited. Do not bypass access controls for illegal purposes or engage in activities that threaten network security, public order, or the rights of others.

### Risks and responsibility

The tool is provided as is. To the extent permitted by applicable law, its authors, maintainers, and contributors make no guarantees about accuracy, completeness, fitness for a particular purpose, availability, or test effectiveness.

Review input material, generated files, API endpoints, and target environments before use. Evaluate risks including data disclosure, API charges, resource use, file compatibility, and service interruption. Successful sample generation or a working local preview establishes neither authorization nor safe behavior in a target system.

Users assume the risks and consequences of using, modifying, or distributing the tool and its generated samples. To the extent permitted by law, the developers, maintainers, and contributors accept no liability for resulting losses, disputes, or legal claims.

### Compliance and enforcement

Understand the laws that apply to your location, the target system, and the testing activity. Retain authorization and necessary test records, and handle data according to the agreed terms. Confirm that you are entitled to send any material to an external model provider. Do not submit personal information, trade secrets, or other protected data without permission.

Maintainers may decline assistance for unlawful or abusive use and may adjust distribution or maintenance arrangements where law and licensing permit. Evidence of misuse received through reports or public sources may be retained and reported as legally appropriate. These provisions do not describe remote monitoring or a mechanism to revoke downloaded copies.

Read these terms and confirm authorization before testing. Illegal misuse is prohibited, and responsibility for illegal activity rests with the person carrying it out.

</details>

## Star history

[![Star History Chart](https://api.star-history.com/svg?repos=spindriftpapilio/icesky&type=Date)](https://star-history.com/#spindriftpapilio/icesky&Date)

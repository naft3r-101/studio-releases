# Studio — releases

Downloads for **Studio**, a design and layout application for print and screen.

This repository holds **only the built installers** and the `latest.yml` that
Studio's updater reads. There is no source code here — it lives in a separate
private repository.

## Install

Grab the latest `Studio-Setup-<version>.exe` from
[Releases](../../releases/latest) and run it.

Windows will show a SmartScreen warning the first time, because the installer is
not signed with a code-signing certificate. Choose **More info → Run anyway**.

Studio installs per-user, so it needs no administrator rights — and neither do
its updates.

## Updating

Studio checks only when you ask it to. Open it and press **Check for updates**
in the top bar. Nothing downloads or installs on its own, and nothing restarts
until you say so.

## Why the installers are here and the code is not

Automatic updates from a private GitHub repository require an access token
embedded in the shipped application, where anyone who installs it can recover
it. Publishing the binaries to a public repository instead means the updater
needs no credentials at all.

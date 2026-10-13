# Flyde file-move demo

[Play the 21-second checkpoint demo](flyde-demo.mp4).

This is a montage of three actual native VS Code screenshots captured during a successful automated extension-host scenario, with subtitle captions. It is not a continuous recording and contains no synthesized editor UI.

- 0–7 seconds: the visual panel has saved its first edit; the YAML reference is `./Child.flyde`, and the real loader resolves `Child`.
- 7–14 seconds: a real `WorkspaceEdit.renameFile` moves the dependency to `parts/Child.flyde`. The reference changes to `./parts/Child.flyde`; the same panel renders `Child`, and the loader resolves it.
- 14–21 seconds: another visual edit in that panel adds the third instance. The moved reference persists, and the loader still resolves `Child`.

Native Computer Use captured the screenshots. FFmpeg encoded the checkpoint montage; the editor screenshots were not manipulated. Runtime verification used macOS/local file URIs. Executing/debugging a moved flow, Windows, and remote providers were not exercised.

OpenAI Codex agents authored and checked the implementation and validation on behalf of `dappweb`; another Codex agent reviewed the final changes. Human review, maintainer acceptance, bounty availability, and payment are not claimed.

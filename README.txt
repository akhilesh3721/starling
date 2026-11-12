Starling 0.8.0 + worldmap 0.6.0

1. Fork starling-client/starling, check out tag v0.8.0.
2. In the repo root:  git apply starling-0.8.0-worldmap-client-apis.patch
3. Copy native-mods/worldmap into the repo's native-mods/ folder.
4. Commit and push. Run the "android" workflow with native_mods = worldmap.

The patch adds native_client_state, native_client_entities, native_set_mod_key and
native_send_chat (ported from upstream Horizon), which worldmap calls and 0.8.0 lacks.
Not compiled by me: send the build log if anything still fails.

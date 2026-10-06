# kong-workshop

Insomnia v5 export of the **Kong AI Gateway Workshop** collection. The requests and the step notes live in `kong-ai-gateway-workshop.yaml`. This repository is separate from the local `kong-shubham-workshop` notes.

## Open it in Insomnia 13

1. Create a project and set **Type** to **Git Sync**.
2. Clone `https://github.com/asynchronos/kong-ai-gateway-workshop.git`, or choose **Import** and select `kong-ai-gateway-workshop.yaml`.
3. On another machine, pull before editing, then commit and push from the branch menu at the bottom of the left pane.

## Environment template

`local-env.template` is in the collection and in `local-env.template.yaml`. It is not private, so it stays in git. These values are empty:

- `KONNECT_TOKEN`
- `OPENAI_API_KEY`
- `my-secret-key`
- `Mcp-Session-Id`
- `mcp_tools_json`
- `prev_assistant_response`
- `final_messages_json`

After import, copy the template into a private environment and fill the secret values there. Requests read the API key from `{{ _['my-secret-key'] }}`. Leave the template empty in git.
